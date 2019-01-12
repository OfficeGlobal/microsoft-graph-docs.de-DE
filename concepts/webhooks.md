---
title: Einrichten von Benachrichtigungen für Änderungen der Benutzerdaten
description: Die Microsoft Graph-API verwendet einen Webhook-Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der eine eigene URL zum Empfangen von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um bei Änderungen ihren Status zu aktualisieren.
author: piotrci
localization_priority: Priority
ms.openlocfilehash: e6cd96f155ad88fa858c9c494538af8c31afa919
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818508"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a>Einrichten von Benachrichtigungen für Änderungen der Benutzerdaten

Die Microsoft Graph-API verwendet einen Webhook-Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der eine eigene URL zum Empfangen von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um bei Änderungen ihren Status zu aktualisieren.

Nachdem Microsoft Graph die Abonnementsanfrage akzeptiert hat, werden Pushbenachrichtigungen an die im Abonnement angegebene URL gesendet. Die App führt dann Aktionen gemäß der Geschäftslogik aus. Sie ruft z. B. weitere Daten ab, aktualisiert Zwischenspeicher für Dokumente und Ansichten usw.

## <a name="supported-resources"></a>Unterstützte Ressourcen

Mit der Microsoft Graph-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:

- Nachrichten
- Ereignisse
- Kontakte
- Benutzer
- Gruppen
- Gruppenunterhaltungen
- Inhalten, die in OneDrive freigegeben werden, einschließlich der diesen SharePoint-Websites zugeordneten Laufwerke
- Persönlichen OneDrive-Ordnern des Benutzers
- Sicherheitswarnungen

Sie können zum Beispiel ein Abonnement für einen bestimmten Mailordner erstellen: `me/mailFolders('inbox')/messages`

Oder für eine Ressource der obersten Ebene: `me/messages`, `me/contacts`, `me/events`, `users`, oder `groups`

Oder für eine bestimmte Ressourceninstanz: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`

Oder für ein Sharepoint Online/OneDrive for Business-Laufwerk: `/drive/root`

Oder für die persönliche OneDrive-Umgebung eines Benutzers: `/drives/{id}/root`
`/drives/{id}/root/subfolder`

Oder für eine neue [Sicherheits-API-Benachrichtigung](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`

### <a name="azure-ad-resource-limitations"></a>Azure AD-Ressourceneinschränkungen

Bestimmte Einschränkungen gelten für Azure AD-basierte Ressourcen (Benutzer, Gruppen) und können bei Überschreitung Fehler hervorrufen:

- Maximale Abonnementkontingente:

  - Pro App: 50 000 Abonnements insgesamt
  - Pro Mandant: 35 Abonnements insgesamt in allen Apps
  - Pro App und Mandanten kombiniert: 7 Abonnements insgesamt

- Azure AD B2C-Mandanten werden nicht unterstützt.

- Benachrichtigungen für Benutzerentitäten werden für persönliche Microsoft-Konten nicht unterstützt.

## <a name="subscription-lifetime"></a>Gültigkeitsdauer von Abonnements

Abonnements haben eine eingeschränkte Gültigkeit. Apps müssen ihre Abonnements vor dem Ablaufzeitpunkt verlängern. Andernfalls müssen sie ein neues Abonnement erstellen. Eine Liste maximaler Ablaufzeiten finden Sie unter [Maximale Abonnementdauer pro Ressourcentyp](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).

Apps können auch jederzeit gekündigt werden, um keine weiteren Benachrichtigungen zu erhalten.

## <a name="managing-subscriptions"></a>Verwalten von Abonnements

Clients können Abonnements erstellen, verlängern und löschen.

### <a name="creating-a-subscription"></a>Erstellen eines Abonnements

Um Benachrichtigungen für eine Ressource zu erhalten, muss in einem ersten Schritt ein Abonnement erstellt werden. Der Abonnementprozess läuft wie folgt ab:

1. Der Client sendet eine Abonnementanforderung (POST) für eine bestimmte Ressource.

1. Microsoft Graph überprüft die Anforderung.

    - Wenn die Anforderung gültig ist, sendet Microsoft Graph ein Überprüfungsstoken an die Benachrichtigungs-URL.
    - Wenn die Anfrage ungültig ist, sendet Microsoft Graph eine Fehlermeldung mit Code und Details.

1. Der Client sendet das Überprüfungstoken zurück an Microsoft Graph.

1. Microsoft Graph sendet eine Antwort an den Client zurück.

Der Client muss die Abonnement-ID speichern, um Benachrichtigungen mit dem Abonnement korrelieren zu können.

#### <a name="subscription-request-example"></a>Beispiel für eine Abonnementanfrage

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

Die Eigenschaften `changeType`, `notificationUrl`, `resource` und `expirationDateTime` sind erforderlich. Unter [subscription-Ressourcentyp](/graph/api/resources/subscription?view=graph-rest-1.0) finden Sie die Eigenschaftsdefinitionen und Werte.

Die Eigenschaft `resource` gibt die Ressource an, deren Änderungen überwacht werden. Sie können z. B. ein Abonnement für einen bestimmten E-Mail-Ordner erstellen: `me/mailFolders('inbox')/messages` oder im Auftrag eines Benutzers mit der Zustimmung eines Administrators: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.

`clientState` ist zwar nicht erforderlich, muss aber eingeschlossen werden, um unserem empfohlenen Prozess zum Umgang mit Benachrichtigungen zu entsprechen. Durch das Festlegen dieser Eigenschaft können Sie bestätigen, dass die empfangenen Benachrichtigungen vom Microsoft Graph-Dienst stammen. Aus diesem Grund muss der Wert der Eigenschaft geheim bleiben und darf nur der Anwendung und dem Microsoft Graph-Dienst bekannt sein.

Wenn der Vorgang erfolgreich war, gibt Microsoft Graph einen `201 Created`-Code und ein [subscription](/graph/api/resources/subscription?view=graph-rest-1.0)-Objekt im Textkörper zurück.

#### <a name="notification-endpoint-validation"></a>Endpunktprüfung für Benachrichtigungen

Microsoft Graph überprüft den Benachrichtigungsendpunkt, der in der Eigenschaft `notificationUrl` der Abonnementanfrage angegeben ist, bevor das Abonnement erstellt wird. Der Überprüfungsprozess läuft wie folgt ab:

1. Microsoft Graph sendet eine POST-Anforderung an die Benachrichtigungs-URL:

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > **Wichtig:** Da `validationToken` ein Abfrageparameter ist, muss er gemäß den HTTP-Codierungspraktiken ordnungsgemäß vom Client decodiert werden. Wenn der Client das Token nicht decodiert und stattdessen im nächsten Schritt (Antwort) den codierten Wert verwendet, tritt bei der Überprüfung ein Fehler auf. Der Client sollte den Tokenwert außerdem als nicht transparent behandeln, da sich das Tokenformat in der Zukunft möglicherweise ohne vorherige Ankündigung ändern kann.

1. Der Client muss innerhalb von 10 Sekunden eine Antwort mit folgenden Merkmalen bereitstellen:

    - Statuscode 200 (OK).
    - Der Inhaltstyp muss `text/plain` sein.
    - Der Textkörper muss das von Microsoft Graph bereitgestellte Überprüfungstoken enthalten.

Der Client muss den Überprüfungstoken verwerfen, nachdem er in der Antwort bereitgestellt wurde.

### <a name="renewing-a-subscription"></a>Verlängern eines Abonnements

Der Kunde kann ein Abonnement mit einem bestimmten Ablaufdatum von bis zu drei Tagen ab dem Zeitpunkt der Anforderung verlängern. Die Eigenschaft `expirationDateTime` muss angegeben werden.

#### <a name="subscription-renewal-example"></a>Beispiel für eine Abonnementverlängerung

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

Wenn der Vorgang erfolgreich war, gibt Microsoft Graph einen `200 OK`-Code und ein [subscription](/graph/api/resources/subscription?view=graph-rest-1.0)-Objekt im Textkörper zurück. Das Abonnementobjekt enthält den neuen Wert für `expirationDateTime`.

### <a name="deleting-a-subscription"></a>Löschen eines Abonnements

Der Client kann den Erhalt von Benachrichtigungen stoppen, indem er das Abonnement anhand seiner ID löscht.

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

Wenn der Vorgang erfolgreich verläuft, gibt Microsoft Graph einen `204 No Content`-Code zurück.

## <a name="notifications"></a>Benachrichtigungen

Der Client beginnt, Benachrichtigungen zu erhalten, nachdem das Abonnement erstellt wurde. Microsoft Graph sendet eine POST-Anforderung an die Benachrichtigungs-URL, wenn sich die Ressource ändert. Benachrichtigungen werden nur für die Änderungen des Typs gesendet, der im Abonnement angegeben ist, z. B. `created`.

> **Hinweis:** Wenn Sie mehrere Abonnements verwenden, die den gleichen Ressourcentyp überwachen und die gleiche Benachrichtigungs-URL verwenden, kann ein POST gesendet werden, der mehrere Benachrichtigungen mit verschiedenen Abonnement-IDs enthalten kann. Es kann nicht garantiert werden, dass alle Benachrichtigungen in einem POST zu einem einzelnen Abonnement gehören.

### <a name="notification-properties"></a>Benachrichtigungseigenschaften

Das Benachrichtigungsobjekt verfügt über die folgenden Eigenschaften:

| Eigenschaft | Typ | Beschreibung |
|:---------|:-----|:------------|
| subscriptionId | string | Die ID des Abonnements, das die Benachrichtigung generiert hat. |
| subscriptionExpirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | Die Ablaufzeit für das Abonnement. |
| clientState | string | Die `clientState`-Eigenschaft in der Abonnementanforderung (falls vorhanden). |
| changeType | string | Der Ereignistyp, der die Benachrichtigung ausgelöst hat. Beispiel: `created` bei Erhalt einer E-Mail oder `updated`, wenn eine Nachricht als gelesen markiert wird. |
| resource | string | Der URI der Ressource relativ zu `https://graph.microsoft.com`. |
| resourceData | object | Der Inhalt dieser Eigenschaft hängt vom Typ der Ressource ab, die abonniert wurde. |

Beispiel: Für Outlook-Ressourcen enthält `resourceData` die folgenden Felder:

| Eigenschaft | Typ | Beschreibung |
|:---------|:-----|:------------|
| @odata.type | string | Der OData-Entitätstyp in Microsoft Graph, der das dargestellte Objekt beschreibt. |
| @odata.id | string | Der OData-Bezeichner des Objekts. |
| @odata.etag | string | Das HTTP-Entitäts-Tag, das eine Version des Objekts darstellt. |
| id | string | Der Bezeichner des Objekts. |

> **Hinweis:** Der Wert `id`, der in `resourceData` bereitgestellt wird, ist zu dem Zeitpunkt gültig, zu dem die Benachrichtigung generiert wurde. Einige Aktionen, z. B. das Verschieben einer Nachricht in einen anderen Ordner, können dazu führen, dass die `id` nicht mehr gültig ist, wenn die Benachrichtigung verarbeitet wird.

### <a name="notification-example"></a>Benachrichtigungsbeispiel

Wenn der Benutzer eine E-Mail empfängt, sendet Microsoft Graph eine Benachrichtigung wie die folgende:

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@<tenant_guid>/messages/{long_id_string}",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"<long_id_string>"
      }
    }
  ]
}
```

Beachten Sie, dass das Feld `value` ein Array von Objekten ist. Wenn viele Benachrichtigungen in der Warteschlange stehen, sendet Microsoft Graph möglicherweise mehrere Objekte in einer einzigen Anforderung. Benachrichtigungen aus anderen Abonnements können in dieselbe Benachrichtigungsanforderung aufgenommen werden.

### <a name="processing-the-notification"></a>Verarbeiten der Benachrichtigung

Jede Benachrichtigung, die Ihre App erhält, sollte verarbeitet werden. Die folgenden Aufgaben müssen von der App mindestens durchgeführt werden, um eine Benachrichtigung zu verarbeiten:

1. Überprüfen der `clientState`-Eigenschaft. Sie muss dem Wert entsprechen, der ursprünglich mit der Anforderung zum Erstellen eines Abonnement übermittelt wurde.

    > **Hinweis:** Ist dies nicht der Fall, kann die Benachrichtigung nicht als gültig betrachtet werden. Es ist möglich, dass die Benachrichtigung nicht von Microsoft Graph stammt und möglicherweise von einem gefälschten Akteur gesendet wurde. Prüfen Sie auch, woher die Benachrichtigung stammt, und ergreifen Sie die entsprechenden Maßnahmen.

1. Aktualisieren Sie die Anwendung basierend auf Ihrer Geschäftslogik.

1. Senden Sie in Ihrer Antwort an Microsoft Graph einen `202 - Accepted` -Statuscode. Wenn Microsoft Graph keinen Code der Klasse 2xx erhält, wird versucht, die Benachrichtigung mehrmals erneut zu senden.

    > **Hinweis:** Senden Sie auch dann einen `202 - Accepted`-Statuscode, wenn die Eigenschaft `clientState` nicht mit derjenigen übereinstimmt, die in der Abonnementanfrage übermittelt wurde. Dies ist eine empfohlene Vorgehensweise, da sie verhindert, dass ein potenziell gefälschte Akteur die Tatsache erkennt, dass Sie seinen Benachrichtigungen nicht vertrauen. Anhand dieser Informationen versucht er dann möglicherweise, den Wert der `clientState`-Eigenschaft zu ermitteln.

Wiederholen Sie den Vorgang für weitere Benachrichtigungen in der Anfrage.

## <a name="code-samples"></a>Codebeispiele

Es folgen einige Codebeispiele in GitHub.

- [Microsoft Graph Webhooks-Beispiel für Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [Microsoft Graph Webhooks-Beispiel für ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [Microsoft Graph-Benutzer-Webhooks-Beispiel mit dem WebJobs-SDK](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a>Siehe auch

- [Abonnementressourcentyp](/graph/api/resources/subscription?view=graph-rest-1.0)
- [Abonnement abrufen](/graph/api/subscription-get?view=graph-rest-1.0)
- [Abonnement erstellen](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)

[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[drive]: /graph/api/resources/drive?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
