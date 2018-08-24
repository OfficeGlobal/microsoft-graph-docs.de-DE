# <a name="create-subscription"></a><span data-ttu-id="6b627-101">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="6b627-101">Create subscription</span></span>

<span data-ttu-id="6b627-102">Diese API abonniert eine Listeneranwendung, über die sie Benachrichtigungen erhält, sobald Daten in Microsoft Graph geändert werden</span><span class="sxs-lookup"><span data-stu-id="6b627-102">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b627-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6b627-103">Permissions</span></span>

<span data-ttu-id="6b627-p101">Zur Abonnementerstellung ist Lesezugriff auf die Ressource erforderlich. Beispiel: um Benachrichtigungsnachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b627-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="6b627-108">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="6b627-108">Resource type / Item</span></span>        | <span data-ttu-id="6b627-109">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="6b627-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="6b627-110">Kontakte</span><span class="sxs-lookup"><span data-stu-id="6b627-110">Contacts</span></span>                    | <span data-ttu-id="6b627-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6b627-111">Contacts.Read</span></span>       |
| <span data-ttu-id="6b627-112">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="6b627-112">Conversations</span></span>               | <span data-ttu-id="6b627-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b627-113">Group.Read.All</span></span>      |
| <span data-ttu-id="6b627-114">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="6b627-114">Events</span></span>                      | <span data-ttu-id="6b627-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6b627-115">Calendars.Read</span></span>      |
| <span data-ttu-id="6b627-116">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="6b627-116">Messages</span></span>                    | <span data-ttu-id="6b627-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6b627-117">Mail.Read</span></span>           |
| <span data-ttu-id="6b627-118">Gruppen</span><span class="sxs-lookup"><span data-stu-id="6b627-118">Groups</span></span>                      | <span data-ttu-id="6b627-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b627-119">Group.Read.All</span></span>      |
| <span data-ttu-id="6b627-120">Benutzer</span><span class="sxs-lookup"><span data-stu-id="6b627-120">Users</span></span>                       | <span data-ttu-id="6b627-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b627-121">User.Read.All</span></span>       |
| <span data-ttu-id="6b627-122">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="6b627-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="6b627-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b627-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="6b627-124">Laufwerke (freigegebene SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="6b627-124">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="6b627-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b627-125">Files.ReadWrite.All</span></span> |

 > <span data-ttu-id="6b627-126">**Hinweis:** Der Endpunkt /v1.0 erlaubt Anwendungsberechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="6b627-126">**Note:** The /v1.0 endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="6b627-127">Unterhaltungen in einer Gruppe und OneDrive-Laufwerk-Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b627-127">Note: The /v1.0 endpoint allows Application permissions for most resources. Conversations in a Group and OneDrive drive root items are not supported with Application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="6b627-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b627-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="6b627-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6b627-129">Request headers</span></span>

| <span data-ttu-id="6b627-130">Name</span><span class="sxs-lookup"><span data-stu-id="6b627-130">Name</span></span>       | <span data-ttu-id="6b627-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6b627-131">Type</span></span> | <span data-ttu-id="6b627-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b627-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6b627-133">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6b627-133">Authorization</span></span>  | <span data-ttu-id="6b627-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6b627-134">string</span></span>  | <span data-ttu-id="6b627-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6b627-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6b627-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b627-137">Response</span></span>

<span data-ttu-id="6b627-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b627-138">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b627-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b627-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6b627-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b627-140">Request</span></span>

<span data-ttu-id="6b627-141">Hier sehen Sie ein Beispiel für die Anforderung zum Senden einer Benachrichtigung, wenn der Benutzer eine neue E-Mail empfängt.</span><span class="sxs-lookup"><span data-stu-id="6b627-141">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
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
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="6b627-142">Geben Sie im Anforderungstext eine JSON-Darstellung des [subscription](../resources/subscription.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="6b627-142">In the request body, supply a JSON representation of the [Contact](../resources/subscription.md) object.</span></span>
<span data-ttu-id="6b627-143">Das Feld `clientState` ist optional.</span><span class="sxs-lookup"><span data-stu-id="6b627-143">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="6b627-144">Beispiele für Ressourcen</span><span class="sxs-lookup"><span data-stu-id="6b627-144">Resources examples</span></span>

<span data-ttu-id="6b627-145">Im Folgenden sind gültige Werte für die Ressourceneigenschaft des Abonnements aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="6b627-145">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="6b627-146">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6b627-146">Resource type</span></span> | <span data-ttu-id="6b627-147">Beispiele</span><span class="sxs-lookup"><span data-stu-id="6b627-147">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="6b627-148">Mail</span><span class="sxs-lookup"><span data-stu-id="6b627-148">Mail</span></span>|<span data-ttu-id="6b627-149">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="6b627-149">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="6b627-150">me/messages</span><span class="sxs-lookup"><span data-stu-id="6b627-150">me/messages</span></span>|
|<span data-ttu-id="6b627-151">Kontakte</span><span class="sxs-lookup"><span data-stu-id="6b627-151">Contacts</span></span>|<span data-ttu-id="6b627-152">pan data-id="undefined" class="unusedGlossaryTerm">me/messages</span><span class="sxs-lookup"><span data-stu-id="6b627-152">me/contacts</span></span>|
|<span data-ttu-id="6b627-153">Kalender</span><span class="sxs-lookup"><span data-stu-id="6b627-153">Calendars</span></span>|<span data-ttu-id="6b627-154">me/events</span><span class="sxs-lookup"><span data-stu-id="6b627-154">me/events</span></span>|
|<span data-ttu-id="6b627-155">Benutzer</span><span class="sxs-lookup"><span data-stu-id="6b627-155">Users</span></span>|<span data-ttu-id="6b627-156">users</span><span class="sxs-lookup"><span data-stu-id="6b627-156">users</span></span>|
|<span data-ttu-id="6b627-157">Gruppen</span><span class="sxs-lookup"><span data-stu-id="6b627-157">Groups</span></span>|<span data-ttu-id="6b627-158">Gruppen</span><span class="sxs-lookup"><span data-stu-id="6b627-158">groups</span></span>|
|<span data-ttu-id="6b627-159">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="6b627-159">Conversations</span></span>|<span data-ttu-id="6b627-160">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="6b627-160">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="6b627-161">Laufwerke</span><span class="sxs-lookup"><span data-stu-id="6b627-161">Drives</span></span>|<span data-ttu-id="6b627-162">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="6b627-162">me/drive/root</span></span>|

##### <a name="response"></a><span data-ttu-id="6b627-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b627-163">Response</span></span>

<span data-ttu-id="6b627-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b627-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="6b627-167">Endpunktprüfung für Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="6b627-167">Notification endpoint validation</span></span>

<span data-ttu-id="6b627-168">Der Abonnement-Benachrichtigungs-Endpunkt (in der Eigenschaft `notificationUrl` angegeben) muss auf eine Validierungsanforderung antworten können, wie beschrieben unter [Einrichten von Benachrichtigungen für Änderungen in Benutzerdaten](../../../concepts/webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="6b627-168">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](../../../concepts/webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="6b627-169">Wenn die Validierung fehlschlägt, gibt die Anforderung zur Erstellung des Abonnements einen 400-Bad Request-Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="6b627-169">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
