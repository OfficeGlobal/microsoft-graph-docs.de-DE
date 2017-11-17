# <a name="get-subscription"></a><span data-ttu-id="98d42-101">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="98d42-101">Get subscription</span></span>

<span data-ttu-id="98d42-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.</span><span class="sxs-lookup"><span data-stu-id="98d42-102">Retrieve the properties and relationships of a subscription.</span></span>
## <a name="permissions"></a><span data-ttu-id="98d42-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="98d42-103">Permissions</span></span>

<span data-ttu-id="98d42-p101">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="98d42-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="98d42-106">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="98d42-106">Resource type / Item</span></span>        | <span data-ttu-id="98d42-107">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="98d42-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="98d42-108">Kontakte</span><span class="sxs-lookup"><span data-stu-id="98d42-108">Contacts</span></span>                    | <span data-ttu-id="98d42-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="98d42-109">Contacts.Read</span></span>       |
| <span data-ttu-id="98d42-110">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="98d42-110">Conversations</span></span>               | <span data-ttu-id="98d42-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="98d42-111">Group.Read.All</span></span>      |
| <span data-ttu-id="98d42-112">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="98d42-112">Events</span></span>                      | <span data-ttu-id="98d42-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="98d42-113">Calendars.Read</span></span>      |
| <span data-ttu-id="98d42-114">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="98d42-114">Messages</span></span>                    | <span data-ttu-id="98d42-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="98d42-115">Mail.Read</span></span>           |
| <span data-ttu-id="98d42-116">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="98d42-116">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="98d42-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98d42-117">Files.ReadWrite</span></span>     |
| <span data-ttu-id="98d42-118">Laufwerke (freigegebene SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="98d42-118">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="98d42-119">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98d42-119">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98d42-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="98d42-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscriptions/{subscriptionId}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="98d42-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="98d42-121">Optional query parameters</span></span>
<span data-ttu-id="98d42-122">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="98d42-122">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98d42-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="98d42-123">Request headers</span></span>
| <span data-ttu-id="98d42-124">Name</span><span class="sxs-lookup"><span data-stu-id="98d42-124">Name</span></span>       | <span data-ttu-id="98d42-125">Typ</span><span class="sxs-lookup"><span data-stu-id="98d42-125">Type</span></span> | <span data-ttu-id="98d42-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98d42-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="98d42-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="98d42-127">Authorization</span></span>  | <span data-ttu-id="98d42-128">string</span><span class="sxs-lookup"><span data-stu-id="98d42-128">string</span></span>  | <span data-ttu-id="98d42-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="98d42-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98d42-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="98d42-131">Request body</span></span>
<span data-ttu-id="98d42-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="98d42-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98d42-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="98d42-133">Response</span></span>

<span data-ttu-id="98d42-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="98d42-134">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="98d42-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="98d42-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98d42-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="98d42-136">Request</span></span>
<span data-ttu-id="98d42-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="98d42-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="98d42-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="98d42-138">Response</span></span>
<span data-ttu-id="98d42-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="98d42-139">Here is an example of the response.</span></span>
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
