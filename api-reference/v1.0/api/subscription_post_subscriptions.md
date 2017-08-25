# <a name="create-subscription"></a><span data-ttu-id="490c8-101">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="490c8-101">Create subscription</span></span>

<span data-ttu-id="490c8-102">Diese API abonniert eine Listeneranwendung, über die sie Benachrichtigungen erhält, sobald Daten in Microsoft Graph geändert werden</span><span class="sxs-lookup"><span data-stu-id="490c8-102">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>
## <a name="permissions"></a><span data-ttu-id="490c8-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="490c8-103">Permissions</span></span>
<span data-ttu-id="490c8-p101">Zur Abonnementerstellung ist Lesezugriff auf die Ressource erforderlich. Beispiel: um Benachrichtigungsnachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="490c8-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="490c8-108">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="490c8-108">Resource type / Item</span></span>        | <span data-ttu-id="490c8-109">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="490c8-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="490c8-110">Kontakte</span><span class="sxs-lookup"><span data-stu-id="490c8-110">Contacts</span></span>                    | <span data-ttu-id="490c8-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="490c8-111">Contacts.Read</span></span>       |
| <span data-ttu-id="490c8-112">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="490c8-112">Conversations</span></span>               | <span data-ttu-id="490c8-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="490c8-113">Group.Read.All</span></span>      |
| <span data-ttu-id="490c8-114">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="490c8-114">Events</span></span>                      | <span data-ttu-id="490c8-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="490c8-115">Calendars.Read</span></span>      |
| <span data-ttu-id="490c8-116">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="490c8-116">Messages</span></span>                    | <span data-ttu-id="490c8-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="490c8-117">Mail.Read</span></span>           |
| <span data-ttu-id="490c8-118">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="490c8-118">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="490c8-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="490c8-119">Files.ReadWrite</span></span>     |
| <span data-ttu-id="490c8-120">Laufwerke (freigegebene SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="490c8-120">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="490c8-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="490c8-121">Files.ReadWrite.All</span></span> |

 <span data-ttu-id="490c8-p102">***Hinweis:*** Der Endpunkt „/v1.0“ unterstützt Anwendungsberechtigungen für die meisten Ressourcentypen. Für Unterhaltungen in einer Gruppe und Elemente des Typs „OneDrive-Stammlaufwerk“ werden Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="490c8-p102">***Note:*** The /v1.0 endpoint allows Application permissions for most resources. Conversations in a Group and OneDrive drive root items are not supported with Application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="490c8-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="490c8-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions

```

## <a name="request-headers"></a><span data-ttu-id="490c8-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="490c8-125">Request headers</span></span>
| <span data-ttu-id="490c8-126">Name</span><span class="sxs-lookup"><span data-stu-id="490c8-126">Name</span></span>       | <span data-ttu-id="490c8-127">Typ</span><span class="sxs-lookup"><span data-stu-id="490c8-127">Type</span></span> | <span data-ttu-id="490c8-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="490c8-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="490c8-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="490c8-129">Authorization</span></span>  | <span data-ttu-id="490c8-130">string</span><span class="sxs-lookup"><span data-stu-id="490c8-130">string</span></span>  | <span data-ttu-id="490c8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="490c8-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="490c8-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="490c8-133">Response</span></span>

<span data-ttu-id="490c8-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="490c8-134">If successful, this method returns `201, Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="490c8-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="490c8-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="490c8-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="490c8-136">Request</span></span>
<span data-ttu-id="490c8-137">Hier sehen Sie ein Beispiel für die Anforderung zum Senden einer Benachrichtigung, wenn der Benutzer eine neue E-Mail empfängt.</span><span class="sxs-lookup"><span data-stu-id="490c8-137">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
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
<span data-ttu-id="490c8-p104">Geben Sie im Anforderungstext eine JSON-Darstellung des [subscription](../resources/subscription.md)-Objekts an. Das *ClientState*-Feld ist optional.</span><span class="sxs-lookup"><span data-stu-id="490c8-p104">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object. The *clientState* field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="490c8-140">Beispiele für Ressourcen</span><span class="sxs-lookup"><span data-stu-id="490c8-140">Resources examples</span></span>
<span data-ttu-id="490c8-141">Im Folgenden sind gültige Werte für die Ressourceneigenschaft des Abonnements aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="490c8-141">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="490c8-142">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="490c8-142">Resource type</span></span> | <span data-ttu-id="490c8-143">Beispiele</span><span class="sxs-lookup"><span data-stu-id="490c8-143">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="490c8-144">Mail</span><span class="sxs-lookup"><span data-stu-id="490c8-144">Mail</span></span>|<span data-ttu-id="490c8-145">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="490c8-145">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="490c8-146">me/messages</span><span class="sxs-lookup"><span data-stu-id="490c8-146">me/messages</span></span>|
|<span data-ttu-id="490c8-147">Kontakte</span><span class="sxs-lookup"><span data-stu-id="490c8-147">Contacts</span></span>|<span data-ttu-id="490c8-148">me/contacts</span><span class="sxs-lookup"><span data-stu-id="490c8-148">me/contacts</span></span>|
|<span data-ttu-id="490c8-149">Kalender</span><span class="sxs-lookup"><span data-stu-id="490c8-149">Calendars</span></span>|<span data-ttu-id="490c8-150">me/events</span><span class="sxs-lookup"><span data-stu-id="490c8-150">me/events</span></span>|
|<span data-ttu-id="490c8-151">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="490c8-151">Conversations</span></span>|<span data-ttu-id="490c8-152">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="490c8-152">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="490c8-153">Laufwerke</span><span class="sxs-lookup"><span data-stu-id="490c8-153">Drives</span></span>|<span data-ttu-id="490c8-154">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="490c8-154">me/drive/root</span></span>|

##### <a name="response"></a><span data-ttu-id="490c8-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="490c8-155">Response</span></span>
<span data-ttu-id="490c8-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="490c8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
## <a name="subscription-validation"></a><span data-ttu-id="490c8-159">Überprüfung des Abonnements</span><span class="sxs-lookup"><span data-stu-id="490c8-159">Subscription validation</span></span>
<span data-ttu-id="490c8-p106">Zur Vermeidung von fehlerhaften Abonnements, die Benachrichtigungen an beliebige URLs weiterleiten, muss der Endpunkt der Abonnementsbenachrichtigung in der Lage sein, auf eine Validierungsanforderung zu reagieren. Bei der Verarbeitung des `POST`-Elements zum `/subscriptions`-Endpunkt sendet Microsoft Graph eine `POST`-Anforderung an `notificationUrl` in folgender Form:</span><span class="sxs-lookup"><span data-stu-id="490c8-p106">In order to to avoid mistaken subscriptions directing notifications to arbitrary URLs, the subscription notification endpoint must be capable of responding to a validation request. During processing of the `POST` to the `/subscriptions` endpoint, the Microsoft Graph will send a `POST` request back to your `notificationUrl` in the following form:</span></span> 
```http
POST https://webhook.azurewebsites.net/api/send/myNotifyClient?validationToken=<token>
```
<span data-ttu-id="490c8-162">Der Benachrichtigungsendpunkt muss innerhalb von 10 Sekunden eine 200-Antwort mit dem Wert `<token>` als Text sowie dem Inhaltstyp `text/plain`, wie unten dargestellt,  senden. Anderenfalls wird die Erstellungsanforderung ignoriert.</span><span class="sxs-lookup"><span data-stu-id="490c8-162">The notification endpoint must send a 200 response with the value of `<token>` as its body and a content type of `text/plain`, as shown below, within 10 seconds otherwise the creation request will be discarded.</span></span>
```http
HTTP/1.1 200 OK
Content-type: text/plain
Content-length: 7
<token>
```
## <a name="notification-payload"></a><span data-ttu-id="490c8-163">Nutzdaten der Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="490c8-163">Notification payload</span></span>
<span data-ttu-id="490c8-p107">Wenn die abonnierten Ressource sich ändert, sendet die Webhooks-Funktion eine Benachrichtigung mit den folgenden Nutzdaten an Ihre Benachrichtigungs-URL.  Der Benachrichtigungsendpunkt muss eine Antwort von 200 oder 204 ohne Antworttext innerhalb von 30 Sekunden senden. Anderenfalls wird der Benachrichtigungsversuch in immer größer werdenden Intervallen wiederholt.  Für Dienste, die immer mindestens 30 Sekunden dauern, kann eine Begrenzung oder ein längeres Benachrichtigungsintervall eingerichtet werden.</span><span class="sxs-lookup"><span data-stu-id="490c8-p107">When the subscribed resource changes, the webhooks facility sends a notification to your notification URL with the following payload.  The notification endpoint must send a response of 200 or 204 with no response body within 30 seconds otherwise the notification attempt will be retried at exponentially increasing intervals.  Services that consistently take 30 seconds or more may be throttled and receive a sparser notification set.</span></span>

<span data-ttu-id="490c8-167">Dienste können auch eine 422-Antwort von einer Benachrichtigung zurückgeben. In diesem Fall wird das Abonnement automatisch gelöscht und die Benachrichtigungen werden eingestellt.</span><span class="sxs-lookup"><span data-stu-id="490c8-167">Services may also return a 422 response from a notification, in which case the subscription will be automatically deleted and the stream of notifications will come to a halt.</span></span>

<span data-ttu-id="490c8-168">Abhängig von der abonnierten Ressource kann ein zusätzliches resourceData-Feld weitere Informationen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="490c8-168">Depending on the subscribed resource, an additional resourceData field may provide additional information.</span></span>

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
<span data-ttu-id="490c8-p108">Wenn Benachrichtigungen von Laufwerksabonnements empfangen werden, ist das resourceData-Element null und die [delta](item_delta.md)-API muss aufgerufen werden, um festzustellen, welche Änderungen aufgetreten sind. Hier sehen Sie ein Beispiel für eine Laufwerksbenachrichtigung:</span><span class="sxs-lookup"><span data-stu-id="490c8-p108">When receiving notifications from Drive subscriptions the resourceData will be null and the [delta](item_delta.md) API should be called to determine the changes that have occured. Here is an example of a Drive notification:</span></span>
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
