# <a name="working-with-webhooks-in-microsoft-graph"></a>Arbeiten mit Webhooks in Microsoft Graph

Die Microsoft Graph-REST-API verwendet einen Webhook-Mechanismus zum Übermitteln von Benachrichtigungen an Clients. Ein Client ist ein Webdienst, der eine eigene URL zum Empfangen von Benachrichtigungen konfiguriert. Client-Apps verwenden Benachrichtigungen, um bei Änderungen ihren Status zu aktualisieren.

Mithilfe der Microsoft Graph-REST-API kann eine App Änderungen an den folgenden Ressourcen abonnieren:

* Nachrichten
* Ereignisse
* Kontakte
* Benutzer
* Gruppen
* Gruppenunterhaltungen
* Inhalten, die in OneDrive freigegeben werden, einschließlich der diesen SharePoint-Websites zugeordneten Laufwerke
* Persönlichen OneDrive-Ordnern des Benutzers

Sie können zum Beispiel ein Abonnement für einen bestimmten Ordner erstellen: `me/mailFolders('inbox')/messages`

Oder eine bestimmte ID: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`

Oder für eine Ressource der obersten Ebene: `me/messages`, `me/contacts`, `me/events`, `users`, oder `groups`

Oder ein Sharepoint Online/OneDrive for Business-Laufwerk: `/drive/root`

Oder persönliche OneDrive-Umgebung eines Benutzers:`/drives/{id}/root`
`/drives/{id}/root/subfolder`

Nachdem Microsoft Graph die Abonnementsanfrage akzeptiert hat, werden Pushbenachrichtigungen an die im Abonnement angegebene URL gesendet. Die App führt dann Aktionen gemäß der Geschäftslogik aus. Sie ruft z. B. weitere Daten ab, aktualisiert Zwischenspeicher für Dokumente und Ansichten usw.

Apps müssen ihre Abonnements vor dem Ablaufzeitpunkt verlängern. Andernfalls müssen sie ein neues Abonnement erstellen. Eine Liste maximaler Ablaufzeiten finden Sie unter [Maximale Abonnementdauer pro Ressourcentyp](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type).

Apps können auch jederzeit gekündigt werden, um keine weiteren Benachrichtigungen zu erhalten.

In der Regel sind für Abonnementvorgänge Leseberechtigungen für die Ressource erforderlich. Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. Unter [Abonnement erstellen](../api-reference/v1.0/api/subscription_post_subscriptions.md) werden die Berechtigungen aufgeführt, die für den jeweiligen Ressourcentyp erforderlich sind. Die folgende Tabelle enthält die Typen von Berechtigungen, die Ihre App für die Verwendung von Webhooks für bestimmte Ressourcentypen anfordern kann. 

| Berechtigungstyp                        | Unterstützte Ressourcentypen in v1.0                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| Delegiert – Geschäfts-, Schul- oder Unikonto     | [Kontakt][], [Unterhaltung][], [Laufwerk][], [Ereignis][], [Nachricht][] |
| Delegiert – persönliches Microsoft-Konto | Keine                                                             |
| Anwendung                            | [Kontakt][], [Unterhaltung][], [Ereignis][], [Nachricht][]            |


## <a name="code-samples"></a>Codebeispiele

Es folgen einige Codebeispiele in GitHub.

* [Microsoft Graph Webhooks-Beispiel für Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [Microsoft Graph Webhooks-Beispiel für ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

### <a name="creating-a-subscription"></a>Erstellen eines Abonnements

Um Benachrichtigungen für eine Ressource zu erhalten, muss in einem ersten Schritt ein Abonnement erstellt werden. Der Abonnementprozess läuft wie folgt ab:

1. Der Client sendet eine Abonnementanforderung (POST) für eine bestimmte Ressource.
2. Microsoft Graph überprüft die Anforderung.
  * Wenn die Anforderung gültig ist, sendet Microsoft Graph ein Überprüfungsstoken an die Benachrichtigungs-URL.
  * Wenn die Anfrage ungültig ist, sendet Microsoft Graph eine Fehlermeldung mit Code und Details.
3. Der Client sendet das Überprüfungstoken zurück an Microsoft Graph.

Der Client muss die Abonnement-ID speichern, um eine Benachrichtigung mit dem entsprechenden Abonnement korrelieren zu können.

### <a name="notification-url-validation"></a>Überprüfung der Benachrichtigungs-URL

Microsoft Graph überprüft die Benachrichtigungs-URL in einer Abonnementanfrage vor dem Erstellen des Abonnements. Der Überprüfungsprozess läuft wie folgt ab:

1. Microsoft Graph sendet eine POST-Anforderung an die Benachrichtigungs-URL:

  ``` http
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```

2. Der Client muss innerhalb von 10 Sekunden eine Antwort mit folgenden Merkmalen bereitstellen:

  * Statuscode 200 (OK).
  * Der Inhaltstyp muss „text/plain“ sein. 
  * Der Textkörper muss das von Microsoft Graph bereitgestellte Überprüfungstoken enthalten.

Der Client muss den Überprüfungstoken verwerfen, nachdem er in der Antwort bereitgestellt wurde.

### <a name="subscription-request-example"></a>Beispiel für eine Abonnementanfrage

``` http
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

Die Eigenschaften `changeType`, `notificationUrl`, `resource` und `expirationDateTime` sind erforderlich. Unter [subscription-Ressourcentyp](../api-reference/v1.0/resources/subscription.md) finden Sie die Eigenschaftsdefinitionen und Werte. `clientState` ist zwar nicht erforderlich, muss aber eingeschlossen werden, um unserem empfohlenen Prozess zum Umgang mit Benachrichtigungen zu entsprechen.

Wenn der Vorgang erfolgreich war, gibt Microsoft Graph einen `201 Created`-Code und ein [subscription](../api-reference/v1.0/resources/subscription.md)-Objekt im Textkörper zurück.

### <a name="azure-ad-resource-limitations"></a>Azure AD-Ressourceneinschränkungen

Bestimmte Einschränkungen gelten für Azure AD-basierte Ressourcen (Benutzer, Gruppen) und können bei Überschreitung Fehler hervorrufen:

* Maximale Abonnementkontingente:

  * Pro App: 50.000 Abonnements insgesamt
  * Pro Mandant: 35 Abonnements insgesamt in allen Apps
  * Pro App und Mandanten kombiniert: 7 Abonnements insgesamt

* Azure AD B2C-Mandanten werden nicht unterstützt

* Privatanwender-Konten werden nicht unterstützt

## <a name="renewing-a-subscription"></a>Verlängern eines Abonnements

Der Kunde kann ein Abonnement mit einem bestimmten Ablaufdatum von bis zu drei Tagen ab dem Zeitpunkt der Anforderung verlängern. Die Eigenschaft „expirationDateTime“ ist erforderlich.

### <a name="subscription-renewal-example"></a>Beispiel für eine Abonnementverlängerung

``` http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

Wenn der Vorgang erfolgreich war, gibt Microsoft Graph einen `200 OK`-Code und ein [subscription](../api-reference/v1.0/resources/subscription.md)-Objekt im Textkörper zurück. Das Abonnementobjekt enthält den neuen Wert füe „expirationDateTime“. 

## <a name="deleting-a-subscription"></a>Löschen eines Abonnements

Der Client kann den Erhalt von Benachrichtigungen stoppen, indem er das Abonnement anhand seiner ID löscht.

``` http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

Wenn der Vorgang erfolgreich verläuft, gibt Microsoft Graph einen `204 No Content`-Code zurück.

## <a name="notifications"></a>Benachrichtigungen

Der Client beginnt, Benachrichtigungen zu erhalten, nachdem das Abonnement erstellt wurde. Microsoft Graph sendet eine POST-Anforderung an die Benachrichtigungs-URL, wenn Änderungen an der Ressource eintreten. Der Kunde erhält nur Benachrichtigungen gemäß dem angegebenen Änderungstyp, z. B. *created*.

### <a name="notification-properties"></a>Benachrichtigungseigenschaften

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

### <a name="notification-example"></a>Benachrichtigungsbeispiel

Wenn der Benutzer eine E-Mail empfängt, sendet Microsoft Graph eine Benachrichtigung wie die folgende:

``` json
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

### <a name="processing-the-notification"></a>Verarbeiten der Benachrichtigung

Sobald Ihre Anwendung Benachrichtigungen erhält, muss sie diese verarbeiten. Die folgenden Aufgaben müssen von der App mindestens durchgeführt werden, um eine Benachrichtigung zu verarbeiten:

1. Überprüfen der `clientState`-Eigenschaft. Die Eigenschaft „clientState“ in der Benachrichtigung muss derjenigen übereinstimmen, die in der Abonnementanfrage übermittelt wurde.
  > Hinweis: Ist dies nicht der Fall, kann die Benachrichtigung nicht als gültig betrachtet werden. Prüfen Sie auch, woher die Benachrichtigung stammt, und ergreifen Sie die entsprechenden Maßnahmen.

2. Aktualisieren Sie die Anwendung basierend auf Ihrer Geschäftslogik.

3. Senden Sie in Ihrer Antwort an Microsoft Graph einen `202 - Accepted` -Statuscode. Wenn Microsoft Graph keinen Code der Klasse 2xx erhält, wird versucht, die Benachrichtigung mehrmals erneut zu senden.
  > Senden Sie auch dann einen `202 - Accepted`-Statuscode, wenn die Eigenschaft „clientState“ nicht mit derjenigen übereinstimmt, die in der Abonnementanfrage übermittelt wurde.

Wiederholen Sie den Vorgang für weitere Benachrichtigungen in der Anfrage.

## <a name="see-also"></a>Siehe auch

* [Abonnementressourcentyp](../api-reference/v1.0/resources/subscription.md)
* [Abonnement abrufen](../api-reference/v1.0/api/subscription_get.md)
* [Abonnement erstellen](../api-reference/v1.0/api/subscription_post_subscriptions.md)
* [Microsoft Graph Webhooks-Beispiel für Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [Microsoft Graph Webhooks-Beispiel für ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

[Kontakt]: ../api-reference/v1.0/resources/contact.md
[Unterhaltung]: ../api-reference/v1.0/resources/conversation.md
[Laufwerk]: ../api-reference/v1.0/resources/drive.md
[Ereignis]: ../api-reference/v1.0/resources/event.md
[Nachricht]: ../api-reference/v1.0/resources/message.md