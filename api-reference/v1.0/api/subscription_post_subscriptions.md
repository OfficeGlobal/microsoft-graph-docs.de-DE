# <a name="create-subscription"></a>Abonnement erstellen

Diese API abonniert eine Listeneranwendung, über die sie Benachrichtigungen erhält, sobald Daten in Microsoft Graph geändert werden
## <a name="permissions"></a>Berechtigungen
Zur Abonnementerstellung ist Lesezugriff auf die Ressource erforderlich. Beispiel: um Benachrichtigungsnachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

| Ressourcentyp/Element        | Berechtigung          |
|-----------------------------|---------------------|
| Kontakte                    | Contacts.Read       |
| Unterhaltungen               | Group.Read.All      |
| Ereignisse                      | Calendars.Read      |
| Nachrichten                    | Mail.Read           |
| Laufwerk (OneDrive eines Benutzers)    | Files.ReadWrite     |
| Laufwerke (freigegebene SharePoint-Inhalte und Laufwerke) | Files.ReadWrite.All |

 ***Hinweis:*** Der Endpunkt „/v1.0“ unterstützt Anwendungsberechtigungen für die meisten Ressourcentypen. Für Unterhaltungen in einer Gruppe und Elemente des Typs „OneDrive-Stammlaufwerk“ werden Anwendungsberechtigungen nicht unterstützt.

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions

```

## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Hier sehen Sie ein Beispiel für die Anforderung zum Senden einer Benachrichtigung, wenn der Benutzer eine neue E-Mail empfängt.
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->
```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "subscription-identifier"
}
```
Geben Sie im Anforderungstext eine JSON-Darstellung des [subscription](../resources/subscription.md)-Objekts an. Das *ClientState*-Feld ist optional.

##### <a name="resources-examples"></a>Beispiele für Ressourcen
Im Folgenden sind gültige Werte für die Ressourceneigenschaft des Abonnements aufgeführt:

| Ressourcentyp | Beispiele |
|:------ |:----- |
|Mail|me/mailfolders('inbox')/messages<br />me/messages|
|Kontakte|me/contacts|
|Kalender|me/events|
|Unterhaltungen|groups('*{id}*')/conversations|
|Laufwerke|me/drive/root|

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 201 Created

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/mailFolders('Inbox')/messages",
  "changeType":"created, updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```
## <a name="subscription-validation"></a>Überprüfung des Abonnements
Zur Vermeidung von fehlerhaften Abonnements, die Benachrichtigungen an beliebige URLs weiterleiten, muss der Endpunkt der Abonnementsbenachrichtigung in der Lage sein, auf eine Validierungsanforderung zu reagieren. Bei der Verarbeitung des `POST`-Elements zum `/subscriptions`-Endpunkt sendet Microsoft Graph eine `POST`-Anforderung an `notificationUrl` in folgender Form: 
```http
POST https://webhook.azurewebsites.net/api/send/myNotifyClient?validationToken=<token>
```
Der Benachrichtigungsendpunkt muss innerhalb von 10 Sekunden eine 200-Antwort mit dem Wert `<token>` als Text sowie dem Inhaltstyp `text/plain`, wie unten dargestellt,  senden. Anderenfalls wird die Erstellungsanforderung ignoriert.
```http
HTTP/1.1 200 OK
Content-type: text/plain
Content-length: 7
<token>
```
## <a name="notification-payload"></a>Nutzdaten der Benachrichtigung
Wenn die abonnierten Ressource sich ändert, sendet die Webhooks-Funktion eine Benachrichtigung mit den folgenden Nutzdaten an Ihre Benachrichtigungs-URL.  Der Benachrichtigungsendpunkt muss eine Antwort von 200 oder 204 ohne Antworttext innerhalb von 30 Sekunden senden. Anderenfalls wird der Benachrichtigungsversuch in immer größer werdenden Intervallen wiederholt.  Für Dienste, die immer mindestens 30 Sekunden dauern, kann eine Begrenzung oder ein längeres Benachrichtigungsintervall eingerichtet werden.

Dienste können auch eine 422-Antwort von einer Benachrichtigung zurückgeben. In diesem Fall wird das Abonnement automatisch gelöscht und die Benachrichtigungen werden eingestellt.

Abhängig von der abonnierten Ressource kann ein zusätzliches resourceData-Feld weitere Informationen bereitstellen.

```http
{
   "value":[
      {
         "subscriptionId":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
         "subscriptionExpirationDateTime":"2015-11-20T18:23:45.9356913Z",
         "clientState":"subscription-identifier",
         "changeType":"Created",
         "resource":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
         "resourceData":{
            "@odata.type":"#Microsoft.Graph.Message",
            "@odata.id":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
            "@odata.etag":"W/\"CQAAABYAAACoeN6SYXGLRrvRm+CYrrfQAACvvGdb\"",
            "Id":"AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA="
         }
      }
   ]
}
```
Wenn Benachrichtigungen von Laufwerksabonnements empfangen werden, ist das resourceData-Element null und die [delta](item_delta.md)-API muss aufgerufen werden, um festzustellen, welche Änderungen aufgetreten sind. Hier sehen Sie ein Beispiel für eine Laufwerksbenachrichtigung:
```http
{
  "subscriptionId": "aa269f87-2a92-4cff-a43e-2771878c3727",
  "clientState": "My client state",
  "changeType": "updated",
  "resource": "me/drive/root",
  "subscriptionExpirationDateTime": "2016-08-26T23:08:37.00+00:00",
  "resourceData": null
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
