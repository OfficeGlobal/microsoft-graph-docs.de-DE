# <a name="update-subscription"></a><span data-ttu-id="42457-101">Abonnement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="42457-101">Update subscription</span></span>

<span data-ttu-id="42457-102">Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="42457-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="42457-103">Abonnements enden nach einer Zeitspanne, die je nach Ressourcentyp variiert.</span><span class="sxs-lookup"><span data-stu-id="42457-103">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="42457-104">Um fehlende Benachrichtigungen zu vermeiden, sollte eine App ihr Abonnement frühzeitig vor ihrem Ablaufdatum erneuern.</span><span class="sxs-lookup"><span data-stu-id="42457-104">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="42457-105">Die maximale Länge eines Abonnements für jeden Ressourcentyp finden Sie unter [Abonnement](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="42457-105">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="42457-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="42457-106">Permissions</span></span>

<span data-ttu-id="42457-p102">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="42457-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="42457-109">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="42457-109">Resource type / Item</span></span>        | <span data-ttu-id="42457-110">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="42457-110">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="42457-111">Kontakte</span><span class="sxs-lookup"><span data-stu-id="42457-111">Contacts</span></span>                    | <span data-ttu-id="42457-112">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="42457-112">Contacts.Read</span></span>       |
| <span data-ttu-id="42457-113">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="42457-113">Conversations</span></span>               | <span data-ttu-id="42457-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="42457-114">Group.Read.All</span></span>      |
| <span data-ttu-id="42457-115">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="42457-115">Events</span></span>                      | <span data-ttu-id="42457-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="42457-116">Calendars.Read</span></span>      |
| <span data-ttu-id="42457-117">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="42457-117">Messages</span></span>                    | <span data-ttu-id="42457-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="42457-118">Mail.Read</span></span>           |
| <span data-ttu-id="42457-119">Gruppen</span><span class="sxs-lookup"><span data-stu-id="42457-119">Groups</span></span>                      | <span data-ttu-id="42457-120">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="42457-120">Group.Read.All</span></span>      |
| <span data-ttu-id="42457-121">Benutzer</span><span class="sxs-lookup"><span data-stu-id="42457-121">Users</span></span>                       | <span data-ttu-id="42457-122">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="42457-122">User.Read.All</span></span>       |
| <span data-ttu-id="42457-123">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="42457-123">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="42457-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42457-124">Files.ReadWrite</span></span>     |
| <span data-ttu-id="42457-125">Laufwerke (freigegebene SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="42457-125">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="42457-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42457-126">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42457-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="42457-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="42457-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="42457-128">Request headers</span></span>

| <span data-ttu-id="42457-129">Name</span><span class="sxs-lookup"><span data-stu-id="42457-129">Name</span></span>       | <span data-ttu-id="42457-130">Typ</span><span class="sxs-lookup"><span data-stu-id="42457-130">Type</span></span> | <span data-ttu-id="42457-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42457-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="42457-132">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="42457-132">Authorization</span></span>  | <span data-ttu-id="42457-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="42457-133">string</span></span>  | <span data-ttu-id="42457-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="42457-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="42457-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="42457-136">Response</span></span>

<span data-ttu-id="42457-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42457-137">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42457-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="42457-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="42457-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="42457-139">Request</span></span>

<span data-ttu-id="42457-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="42457-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="42457-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="42457-141">Response</span></span>

<span data-ttu-id="42457-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="42457-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
