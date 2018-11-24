# <a name="create-subscription"></a><span data-ttu-id="afff7-101">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="afff7-101">Create subscription</span></span>

<span data-ttu-id="afff7-102">Diese API abonniert eine Listeneranwendung, über die sie Benachrichtigungen erhält, sobald Daten in Microsoft Graph geändert werden</span><span class="sxs-lookup"><span data-stu-id="afff7-102">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="afff7-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="afff7-103">Permissions</span></span>

<span data-ttu-id="afff7-p101">Zur Abonnementerstellung ist Lesezugriff auf die Ressource erforderlich. Beispiel: um Benachrichtigungsnachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="afff7-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="afff7-108">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="afff7-108">Resource type / Item</span></span>        | <span data-ttu-id="afff7-109">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="afff7-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="afff7-110">Kontakte</span><span class="sxs-lookup"><span data-stu-id="afff7-110">Contacts</span></span>                    | <span data-ttu-id="afff7-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="afff7-111">Contacts.Read</span></span>       |
| <span data-ttu-id="afff7-112">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="afff7-112">Conversations</span></span>               | <span data-ttu-id="afff7-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="afff7-113">Group.Read.All</span></span>      |
| <span data-ttu-id="afff7-114">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="afff7-114">Events</span></span>                      | <span data-ttu-id="afff7-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="afff7-115">Calendars.Read</span></span>      |
| <span data-ttu-id="afff7-116">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="afff7-116">Messages</span></span>                    | <span data-ttu-id="afff7-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="afff7-117">Mail.Read</span></span>           |
| <span data-ttu-id="afff7-118">Gruppen</span><span class="sxs-lookup"><span data-stu-id="afff7-118">Groups</span></span>                      | <span data-ttu-id="afff7-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="afff7-119">Group.Read.All</span></span>      |
| <span data-ttu-id="afff7-120">Benutzer</span><span class="sxs-lookup"><span data-stu-id="afff7-120">Users</span></span>                       | <span data-ttu-id="afff7-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="afff7-121">User.Read.All</span></span>       |
| <span data-ttu-id="afff7-122">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="afff7-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="afff7-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="afff7-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="afff7-124">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="afff7-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="afff7-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afff7-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="afff7-126">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="afff7-126">Security alert</span></span>| <span data-ttu-id="afff7-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afff7-127">SecurityEvents.ReadWrite.All</span></span> |

 > <span data-ttu-id="afff7-128">**Hinweis:** Der Endpunkt /v1.0 kann Berechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="afff7-128">**Note:** The /v1.0 endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="afff7-129">Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="afff7-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="afff7-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="afff7-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="afff7-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="afff7-131">Request headers</span></span>

| <span data-ttu-id="afff7-132">Name</span><span class="sxs-lookup"><span data-stu-id="afff7-132">Name</span></span>       | <span data-ttu-id="afff7-133">Typ</span><span class="sxs-lookup"><span data-stu-id="afff7-133">Type</span></span> | <span data-ttu-id="afff7-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="afff7-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="afff7-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="afff7-135">Authorization</span></span>  | <span data-ttu-id="afff7-136">string</span><span class="sxs-lookup"><span data-stu-id="afff7-136">string</span></span>  | <span data-ttu-id="afff7-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="afff7-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="afff7-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="afff7-139">Response</span></span>

<span data-ttu-id="afff7-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="afff7-140">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afff7-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="afff7-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="afff7-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="afff7-142">Request</span></span>

<span data-ttu-id="afff7-143">Hier sehen Sie ein Beispiel für die Anforderung zum Senden einer Benachrichtigung, wenn der Benutzer eine neue E-Mail empfängt.</span><span class="sxs-lookup"><span data-stu-id="afff7-143">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
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

<span data-ttu-id="afff7-144">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Abonnement](../resources/subscription.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="afff7-144">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="afff7-145">Die `clientState` Feld ist optional.</span><span class="sxs-lookup"><span data-stu-id="afff7-145">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="afff7-146">Beispiele für Ressourcen</span><span class="sxs-lookup"><span data-stu-id="afff7-146">Resources examples</span></span>

<span data-ttu-id="afff7-147">Im Folgenden sind gültige Werte für die Ressourceneigenschaft des Abonnements aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="afff7-147">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="afff7-148">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="afff7-148">Resource type</span></span> | <span data-ttu-id="afff7-149">Beispiele</span><span class="sxs-lookup"><span data-stu-id="afff7-149">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="afff7-150">Mail</span><span class="sxs-lookup"><span data-stu-id="afff7-150">Mail</span></span>|<span data-ttu-id="afff7-151">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="afff7-151">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="afff7-152">me/messages</span><span class="sxs-lookup"><span data-stu-id="afff7-152">me/messages</span></span>|
|<span data-ttu-id="afff7-153">Kontakte</span><span class="sxs-lookup"><span data-stu-id="afff7-153">Contacts</span></span>|<span data-ttu-id="afff7-154">me/contacts</span><span class="sxs-lookup"><span data-stu-id="afff7-154">me/contacts</span></span>|
|<span data-ttu-id="afff7-155">Kalender</span><span class="sxs-lookup"><span data-stu-id="afff7-155">Calendars</span></span>|<span data-ttu-id="afff7-156">me/events</span><span class="sxs-lookup"><span data-stu-id="afff7-156">me/events</span></span>|
|<span data-ttu-id="afff7-157">Benutzer</span><span class="sxs-lookup"><span data-stu-id="afff7-157">Users</span></span>|<span data-ttu-id="afff7-158">users</span><span class="sxs-lookup"><span data-stu-id="afff7-158">users</span></span>|
|<span data-ttu-id="afff7-159">Gruppen</span><span class="sxs-lookup"><span data-stu-id="afff7-159">Groups</span></span>|<span data-ttu-id="afff7-160">Gruppen</span><span class="sxs-lookup"><span data-stu-id="afff7-160">groups</span></span>|
|<span data-ttu-id="afff7-161">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="afff7-161">Conversations</span></span>|<span data-ttu-id="afff7-162">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="afff7-162">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="afff7-163">Laufwerke</span><span class="sxs-lookup"><span data-stu-id="afff7-163">Drives</span></span>|<span data-ttu-id="afff7-164">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="afff7-164">me/drive/root</span></span>|
|<span data-ttu-id="afff7-165">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="afff7-165">Security alert</span></span>|<span data-ttu-id="afff7-166">Sicherheitshinweise /? $filter = Status Eq 'Neu'</span><span class="sxs-lookup"><span data-stu-id="afff7-166">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="afff7-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="afff7-167">Response</span></span>

<span data-ttu-id="afff7-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="afff7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="afff7-171">Endpunktprüfung für Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="afff7-171">Notification endpoint validation</span></span>

<span data-ttu-id="afff7-172">Das Abonnement Benachrichtigung Endpunkt (im angegebenen der `notificationUrl` -Eigenschaft) müssen Daten aneinander zur Reaktion auf eine Anforderung zur Überprüfung, wie unter [Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten](../../../concepts/webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="afff7-172">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](../../../concepts/webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="afff7-173">Wenn die Überprüfung fehlschlägt, gibt die Anforderung an das Abonnement zu erstellen einer 400-Bad Request-Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="afff7-173">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
