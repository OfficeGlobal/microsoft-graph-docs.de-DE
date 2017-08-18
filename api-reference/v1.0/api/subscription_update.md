# <a name="update-subscription"></a><span data-ttu-id="e0301-101">Abonnement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e0301-101">Update subscription</span></span>

<span data-ttu-id="e0301-102">Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="e0301-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="e0301-p101">Abonnements für Ressourcen laufen an Tagen ab, die von den einzelnen Ressourcentypen vorgegeben werden.  Um keine Benachrichtigungen zu verpassen, sollten Abonnements weit vor ihrem Ablaufdatum verlängert werden.  Informationen zu den einzelnen Ablaufdaten finden Sie unter [Abonnement](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="e0301-p101">Subscriptions to resources expire at dates proscribed by the individual resource types.  In order not to miss notifications, subscriptions should be renewed well in advance of their expiry date.  See [subscription](../resources/subscription.md) for individual expiry dates.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0301-106">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="e0301-106">Prerequisites</span></span>

<span data-ttu-id="e0301-107">Die folgende Tabelle listet die vorgeschlagenen Berechtigungen, die für die jeweilige Ressource erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e0301-107">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="e0301-108">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="e0301-108">Resource type / Item</span></span>        | <span data-ttu-id="e0301-109">Bereich</span><span class="sxs-lookup"><span data-stu-id="e0301-109">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="e0301-110">Kontakte</span><span class="sxs-lookup"><span data-stu-id="e0301-110">Contacts</span></span>                    | <span data-ttu-id="e0301-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e0301-111">Contacts.Read</span></span>       |
| <span data-ttu-id="e0301-112">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="e0301-112">Conversations</span></span>               | <span data-ttu-id="e0301-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0301-113">Group.Read.All</span></span>      |
| <span data-ttu-id="e0301-114">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="e0301-114">Events</span></span>                      | <span data-ttu-id="e0301-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e0301-115">Calendars.Read</span></span>      |
| <span data-ttu-id="e0301-116">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="e0301-116">Messages</span></span>                    | <span data-ttu-id="e0301-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e0301-117">Mail.Read</span></span>           |
| <span data-ttu-id="e0301-118">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="e0301-118">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="e0301-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0301-119">Files.ReadWrite</span></span>     |
| <span data-ttu-id="e0301-120">Laufwerke (freigegebene SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="e0301-120">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="e0301-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0301-121">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0301-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0301-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /subscriptions/{subscriptionId}
```

## <a name="request-headers"></a><span data-ttu-id="e0301-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0301-123">Request headers</span></span>
| <span data-ttu-id="e0301-124">Name</span><span class="sxs-lookup"><span data-stu-id="e0301-124">Name</span></span>       | <span data-ttu-id="e0301-125">Typ</span><span class="sxs-lookup"><span data-stu-id="e0301-125">Type</span></span> | <span data-ttu-id="e0301-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0301-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e0301-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0301-127">Authorization</span></span>  | <span data-ttu-id="e0301-128">string</span><span class="sxs-lookup"><span data-stu-id="e0301-128">string</span></span>  | <span data-ttu-id="e0301-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0301-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e0301-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0301-131">Response</span></span>

<span data-ttu-id="e0301-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0301-132">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0301-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0301-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0301-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0301-134">Request</span></span>
<span data-ttu-id="e0301-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0301-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="e0301-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0301-136">Response</span></span>
<span data-ttu-id="e0301-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e0301-137">Here is an example of the response.</span></span>
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
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
