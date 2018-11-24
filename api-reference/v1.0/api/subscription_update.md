# <a name="update-subscription"></a><span data-ttu-id="055d2-101">Abonnement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="055d2-101">Update subscription</span></span>

<span data-ttu-id="055d2-102">Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="055d2-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="055d2-103">Abonnements laufen ab nach der Zeitspanne, die nach Ressourcentyp variiert.</span><span class="sxs-lookup"><span data-stu-id="055d2-103">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="055d2-104">Zur Vermeidung von Benachrichtigungen fehlende sollten eine app seine Abonnements im Vorfeld ihrem Ablaufdatum erneuern.</span><span class="sxs-lookup"><span data-stu-id="055d2-104">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="055d2-105">Finden Sie unter [Abonnement](../resources/subscription.md) für die maximale Länge eines Abonnements für jeden Ressourcentyp.</span><span class="sxs-lookup"><span data-stu-id="055d2-105">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="055d2-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="055d2-106">Permissions</span></span>

<span data-ttu-id="055d2-p102">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="055d2-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="055d2-109">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="055d2-109">Resource type / Item</span></span>        | <span data-ttu-id="055d2-110">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="055d2-110">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="055d2-111">Kontakte</span><span class="sxs-lookup"><span data-stu-id="055d2-111">Contacts</span></span>                    | <span data-ttu-id="055d2-112">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="055d2-112">Contacts.Read</span></span>       |
| <span data-ttu-id="055d2-113">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="055d2-113">Conversations</span></span>               | <span data-ttu-id="055d2-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="055d2-114">Group.Read.All</span></span>      |
| <span data-ttu-id="055d2-115">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="055d2-115">Events</span></span>                      | <span data-ttu-id="055d2-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="055d2-116">Calendars.Read</span></span>      |
| <span data-ttu-id="055d2-117">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="055d2-117">Messages</span></span>                    | <span data-ttu-id="055d2-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="055d2-118">Mail.Read</span></span>           |
| <span data-ttu-id="055d2-119">Gruppen</span><span class="sxs-lookup"><span data-stu-id="055d2-119">Groups</span></span>                      | <span data-ttu-id="055d2-120">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="055d2-120">Group.Read.All</span></span>      |
| <span data-ttu-id="055d2-121">Benutzer</span><span class="sxs-lookup"><span data-stu-id="055d2-121">Users</span></span>                       | <span data-ttu-id="055d2-122">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="055d2-122">User.Read.All</span></span>       |
| <span data-ttu-id="055d2-123">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="055d2-123">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="055d2-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="055d2-124">Files.ReadWrite</span></span>     |
| <span data-ttu-id="055d2-125">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="055d2-125">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="055d2-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="055d2-126">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="055d2-127">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="055d2-127">Security alert</span></span>| <span data-ttu-id="055d2-128">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="055d2-128">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="055d2-129">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="055d2-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="055d2-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="055d2-130">Request headers</span></span>

| <span data-ttu-id="055d2-131">Name</span><span class="sxs-lookup"><span data-stu-id="055d2-131">Name</span></span>       | <span data-ttu-id="055d2-132">Typ</span><span class="sxs-lookup"><span data-stu-id="055d2-132">Type</span></span> | <span data-ttu-id="055d2-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="055d2-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="055d2-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="055d2-134">Authorization</span></span>  | <span data-ttu-id="055d2-135">string</span><span class="sxs-lookup"><span data-stu-id="055d2-135">string</span></span>  | <span data-ttu-id="055d2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="055d2-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="055d2-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="055d2-138">Response</span></span>

<span data-ttu-id="055d2-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="055d2-139">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="055d2-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="055d2-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="055d2-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="055d2-141">Request</span></span>

<span data-ttu-id="055d2-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="055d2-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="055d2-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="055d2-143">Response</span></span>

<span data-ttu-id="055d2-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="055d2-144">Here is an example of the response.</span></span>
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
