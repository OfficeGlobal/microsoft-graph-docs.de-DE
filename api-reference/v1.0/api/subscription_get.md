# <a name="get-subscription"></a><span data-ttu-id="e0b84-101">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="e0b84-101">Get subscription</span></span>

<span data-ttu-id="e0b84-102">Dient zum Abrufen der Eigenschaften und der Beziehungen eines Abonnements.</span><span class="sxs-lookup"><span data-stu-id="e0b84-102">Retrieve the properties and relationships of a subscription.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0b84-103">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="e0b84-103">Prerequisites</span></span>

<span data-ttu-id="e0b84-104">Die folgende Tabelle listet die vorgeschlagenen Berechtigungen, die für die jeweilige Ressource erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e0b84-104">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="e0b84-105">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="e0b84-105">Resource type / Item</span></span>        | <span data-ttu-id="e0b84-106">Bereich</span><span class="sxs-lookup"><span data-stu-id="e0b84-106">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="e0b84-107">Kontakte</span><span class="sxs-lookup"><span data-stu-id="e0b84-107">Contacts</span></span>                    | <span data-ttu-id="e0b84-108">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e0b84-108">Contacts.Read</span></span>       |
| <span data-ttu-id="e0b84-109">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="e0b84-109">Conversations</span></span>               | <span data-ttu-id="e0b84-110">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0b84-110">Group.Read.All</span></span>      |
| <span data-ttu-id="e0b84-111">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="e0b84-111">Events</span></span>                      | <span data-ttu-id="e0b84-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e0b84-112">Calendars.Read</span></span>      |
| <span data-ttu-id="e0b84-113">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="e0b84-113">Messages</span></span>                    | <span data-ttu-id="e0b84-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e0b84-114">Mail.Read</span></span>           |
| <span data-ttu-id="e0b84-115">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="e0b84-115">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="e0b84-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0b84-116">Files.ReadWrite</span></span>     |
| <span data-ttu-id="e0b84-117">Laufwerke (freigegebene SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="e0b84-117">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="e0b84-118">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0b84-118">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0b84-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0b84-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscriptions/{subscriptionId}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e0b84-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e0b84-120">Optional query parameters</span></span>
<span data-ttu-id="e0b84-121">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e0b84-121">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0b84-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0b84-122">Request headers</span></span>
| <span data-ttu-id="e0b84-123">Name</span><span class="sxs-lookup"><span data-stu-id="e0b84-123">Name</span></span>       | <span data-ttu-id="e0b84-124">Typ</span><span class="sxs-lookup"><span data-stu-id="e0b84-124">Type</span></span> | <span data-ttu-id="e0b84-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0b84-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e0b84-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0b84-126">Authorization</span></span>  | <span data-ttu-id="e0b84-127">string</span><span class="sxs-lookup"><span data-stu-id="e0b84-127">string</span></span>  | <span data-ttu-id="e0b84-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0b84-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0b84-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e0b84-130">Request body</span></span>
<span data-ttu-id="e0b84-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e0b84-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0b84-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0b84-132">Response</span></span>

<span data-ttu-id="e0b84-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0b84-133">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0b84-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0b84-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0b84-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0b84-135">Request</span></span>
<span data-ttu-id="e0b84-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0b84-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="e0b84-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0b84-137">Response</span></span>
<span data-ttu-id="e0b84-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e0b84-138">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
