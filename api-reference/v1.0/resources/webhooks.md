# <a name="working-with-webhooks-in-microsoft-graph"></a>Arbeiten mit Webhooks in Microsoft Graph

Die Microsoft Graph-REST-API verwendet einen Webhook-Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der eine eigene URL zum Empfangen von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um bei Änderungen ihren Status zu aktualisieren.

Mithilfe der Microsoft Graph-REST-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:

* Nachrichten
* Ereignisse
* Kontakte
* Gruppenunterhaltungen
* Laufwerkstammelemente

Nachdem Microsoft Graph die Abonnementsanfrage akzeptiert hat, werden Pushbenachrichtigungen an die im Abonnement angegebene URL gesendet. Die App führt dann Aktionen gemäß der Geschäftslogik aus. Sie ruft z. B. weitere Daten ab, aktualisiert Zwischenspeicher für Dokumente und Ansichten usw.

Apps sollten ihre Abonnements verlängern, bevor diese ablaufen. Abonnements können auch jederzeit gekündigt werden, um keine weiteren Benachrichtigungen zu erhalten.

Es folgen einige Codebeispiele in GitHub.

* [Microsoft Graph Webhooks-Beispiel für Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [Microsoft Graph Webhooks-Beispiel für ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

Im Folgenden wird der Abonnementprozess beschrieben.

# <a name="creating-a-subscription"></a>Erstellen eines Abonnements

Um Benachrichtigungen für eine Ressource zu erhalten, muss in einem ersten Schritt ein Abonnement erstellt werden. Der Abonnementprozess läuft wie folgt ab:

1. Der Client sendet eine Abonnementanforderung (POST) für eine bestimmte Ressource.
2. Microsoft Graph überprüft die Anforderung.
  * Wenn die Anforderung gültig ist, sendet Microsoft Graph ein Überprüfungsstoken an die Benachrichtigungs-URL.
  * Wenn die Anfrage ungültig ist, sendet Microsoft Graph eine Fehlermeldung mit Code und Details.
3. Der Client sendet das Überprüfungstoken zurück an Microsoft Graph.

Der Client muss die Abonnement-ID speichern, um eine Benachrichtigung mit dem entsprechenden Abonnement korrelieren zu können.

## <a name="characteristics-of-subscriptions"></a>Merkmale von Abonnements

Sie können Abonnements für Ressourcen wie Nachrichten, Ereignisse, Kontakte und Laufwerkstammelemente erstellen.

Sie können ein Abonnement für einen bestimmten Ordner erstellen: `https://graph.microsoft.com/v1.0/me/mailfolders('inbox')/messages`

Oder für eine Ressource der obersten Ebene: `https://graph.microsoft.com/v1.0/me/messages`

Oder ein Laufwerkstammelement: `https://graph.microsoft.com/v1.0/me/drive/root`

Für das Erstellen eines Abonnements ist in den meisten Fällen Lesezugriff auf die Ressource erforderlich. Beispiel: um Benachrichtigungsnachrichten zu erhalten, benötigt Ihre App die `mail.read`-Berechtigung. Bitte beachten Sie, das zurzeit die `Files.ReadWrite`-Berechtigung für OneDrive-Stammlaufwerkelemente erforderlich ist, während SharePoint-Websites zugeordnete Laufwerke `Files.ReadWrite.All` erfordern.

Abonnements laufen ab. Derzeit beträgt die längste Ablaufzeit drei Tage, abzüglich 90 Minuten (4230 insgesamt) ab der Erstellungszeit. Apps müssen ihre Abonnements vor dem Ablaufzeitpunkt verlängern. Andernfalls müssen sie ein neues Abonnement erstellen.

## <a name="notification-url-validation"></a>Überprüfung der Benachrichtigungs-URL

Microsoft Graph überprüft die Benachrichtigungs-URL in einer Abonnementanfrage vor dem Erstellen des Abonnements. Der Überprüfungsprozess läuft wie folgt ab:

1. Microsoft Graph sendet eine POST-Anforderung an die Benachrichtigungs-URL:

  ```
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```
 
2. Der Client muss innerhalb von 10 Sekunden eine Antwort mit folgenden Merkmalen bereitstellen:

  * Statuscode 200 (OK).
  * Der Inhaltstyp muss „text/plain“ sein. 
  * Der Textkörper muss das von Microsoft Graph bereitgestellte Überprüfungstoken enthalten.

Der Client muss den Überprüfungstoken verwerfen, nachdem er in der Antwort bereitgestellt wurde.

## <a name="subscription-request-example"></a>Beispiel für eine Abonnementanfrage

```
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

Die Eigenschaften `changeType`, `notificationUrl`, `resource` und `expirationDateTime` sind erforderlich. Unter [subscription-Ressourcentyp](subscription.md) finden Sie die Eigenschaftsdefinitionen und Werte. `clientState` ist zwar nicht erforderlich, muss aber eingeschlossen werden, um unserem empfohlenen Prozess zum Umgang mit Benachrichtigungen zu entsprechen.

Wenn der Vorgang erfolgreich war, gibt Microsoft Graph einen `201 Created`-Code und ein [subscription](subscription.md)-Objekt im Textkörper zurück.

# <a name="renewing-a-subscription"></a>Verlängern eines Abonnements

Der Kunde kann ein Abonnement mit einem bestimmten Ablaufdatum von bis zu drei Tagen ab dem Zeitpunkt der Anforderung verlängern. Die Eigenschaft „expirationDateTime“ ist erforderlich.

## <a name="subscription-renewal-example"></a>Beispiel für eine Abonnementverlängerung

```
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

Wenn der Vorgang erfolgreich war, gibt Microsoft Graph einen `200 OK`-Code und ein [subscription](subscription.md)-Objekt im Textkörper zurück. Das Abonnementobjekt enthält den neuen Wert füe „expirationDateTime“. 

# <a name="deleting-a-subscription"></a>Löschen eines Abonnements

Der Client kann den Erhalt von Benachrichtigungen stoppen, indem er das Abonnement anhand seiner ID löscht.

```
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

Wenn der Vorgang erfolgreich verläuft, gibt Microsoft Graph einen `204 No Content`-Code zurück.

# <a name="notifications"></a>Benachrichtigungen

Der Client beginnt, Benachrichtigungen zu erhalten, nachdem das Abonnement erstellt wurde. Microsoft Graph sendet eine POST-Anforderung an die Benachrichtigungs-URL, wenn Änderungen an der Ressource eintreten. Der Kunde erhält nur Benachrichtigungen gemäß dem angegebenen Änderungstyp, z. B. *created*.

## <a name="notification-properties"></a>Benachrichtigungseigenschaften

Das Benachrichtigungsobjekt verfügt über die folgenden Eigenschaften.

* subscriptionId: Die ID für das Abonnement, zu dem diese Benachrichtigung gehört.
* subscriptionExpirationDateTime: Die Ablaufzeit für das Abonnement.
* clientState: Die clientState-Eigenschaft, die in der Abonnementanfrage angegeben wurde.
* changeType: Der Ereignistyp, der die Benachrichtigung ausgelöst hat. Z. B. *created* bei Erhalt einer E-Mail oder *updated*, wenn eine Nachricht als gelesen markiert wird.
* resource: Der URI der Ressource relativ zu `https://graph.microsoft.com`. 
* resourceData: Das Objekt das von der abonnierten Ressource abhängt.  Z. B. für Outlook-Ressourcen:
  * @odata.type: Der OData-Entitätstyp in Microsoft Graph, der das dargestellte Objekt beschreibt.
  * @odata.id: Der OData-Bezeichner des Objekts.
  * @odata.etag: Das HTTP-Entitäts-Tag, das eine Version des Objekts darstellt.
  * Id: Der Bezeichner des Objekts.


> Hinweis: Der in „resourceData“ bereitgestellte Id-Wert ist zu dem Zeitpunkt gültig, zu dem die Benachrichtigung in die Warteschlange gestellt wurde. Bei einigen Aktionen, wie z. B. de Verschieben einer Nachricht in einen anderen Ordner, kann es zu einer Änderung der Ressourcen-ID kommen. 

## <a name="notification-example"></a>Benachrichtigungsbeispiel

Wenn der Benutzer eine E-Mail empfängt, sendet Microsoft Graph eine Benachrichtigung wie die folgende:

```
{
  "value":[
  {
    "subscriptionId":"<subscription_guid>",
    "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
    "clientState":"SecretClientState",
    "changeType":"Created",
    "resource":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
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

Beachten Sie, dass das Wertobjekt eine Liste enthält. Wenn viele Benachrichtigungen in der Warteschlange stehen, sendet Microsoft Graph diese in einer einzigen Anforderung.

## <a name="processing-the-notification"></a>Verarbeiten der Benachrichtigung

Sobald Ihre Anwendung Benachrichtigungen erhält, muss sie diese verarbeiten. Die folgenden Aufgaben müssen von der App mindestens durchgeführt werden, um eine Benachrichtigung zu verarbeiten:

1. Überprüfen der `clientState`-Eigenschaft. Die Eigenschaft „clientState“ in der Benachrichtigung muss derjenigen übereinstimmen, die in der Abonnementanfrage übermittelt wurde.
  > Hinweis: Ist dies nicht der Fall, kann die Benachrichtigung nicht als gültig betrachtet werden. Prüfen Sie auch, woher die Benachrichtigung stammt, und ergreifen Sie die entsprechenden Maßnahmen.

2. Aktualisieren Sie die Anwendung basierend auf Ihrer Geschäftslogik.
3. Senden Sie in Ihrer Antwort an Microsoft Graph einen `202 - Accepted` -Statuscode. Wenn Microsoft Graph keinen Code der Klasse 2xx erhält, wird versucht, die Benachrichtigung mehrmals erneut zu senden.
  > Senden Sie auch dann einen `202 - Accepted`-Statuscode, wenn die Eigenschaft „clientState“ nicht mit derjenigen übereinstimmt, die in der Abonnementanfrage übermittelt wurde.

Wiederholen Sie den Vorgang für weitere Benachrichtigungen in der Anfrage.

# <a name="additional-resources"></a>Zusätzliche Ressourcen

* [Abonnementressourcentyp](subscription.md)
* [Abonnement abrufen](../api/subscription_get.md)
* [Abonnement erstellen](../api/subscription_post_subscriptions.md)
* [Microsoft Graph Webhooks-Beispiel für Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [Microsoft Graph Webhooks-Beispiel für ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
