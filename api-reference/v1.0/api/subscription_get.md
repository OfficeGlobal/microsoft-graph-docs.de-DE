# <a name="get-subscription"></a><span data-ttu-id="28889-101">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="28889-101">Get subscription</span></span>

<span data-ttu-id="28889-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.</span><span class="sxs-lookup"><span data-stu-id="28889-102">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="28889-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="28889-103">Permissions</span></span>

<span data-ttu-id="28889-p101">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="28889-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="28889-106">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="28889-106">Resource type / Item</span></span>        | <span data-ttu-id="28889-107">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="28889-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="28889-108">Kontakte</span><span class="sxs-lookup"><span data-stu-id="28889-108">Contacts</span></span>                    | <span data-ttu-id="28889-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="28889-109">Contacts.Read</span></span>       |
| <span data-ttu-id="28889-110">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="28889-110">Conversations</span></span>               | <span data-ttu-id="28889-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="28889-111">Group.Read.All</span></span>      |
| <span data-ttu-id="28889-112">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="28889-112">Events</span></span>                      | <span data-ttu-id="28889-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="28889-113">Calendars.Read</span></span>      |
| <span data-ttu-id="28889-114">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="28889-114">Messages</span></span>                    | <span data-ttu-id="28889-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="28889-115">Mail.Read</span></span>           |
| <span data-ttu-id="28889-116">Gruppen</span><span class="sxs-lookup"><span data-stu-id="28889-116">Groups</span></span>                      | <span data-ttu-id="28889-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="28889-117">Group.Read.All</span></span>      |
| <span data-ttu-id="28889-118">Benutzer</span><span class="sxs-lookup"><span data-stu-id="28889-118">Users</span></span>                       | <span data-ttu-id="28889-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="28889-119">User.Read.All</span></span>       |
| <span data-ttu-id="28889-120">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="28889-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="28889-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28889-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="28889-122">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="28889-122">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="28889-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28889-123">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="28889-124">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="28889-124">Security alert</span></span>| <span data-ttu-id="28889-125">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28889-125">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28889-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28889-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28889-127">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="28889-127">Optional query parameters</span></span>

<span data-ttu-id="28889-128">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="28889-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28889-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28889-129">Request headers</span></span>

| <span data-ttu-id="28889-130">Name</span><span class="sxs-lookup"><span data-stu-id="28889-130">Name</span></span>       | <span data-ttu-id="28889-131">Typ</span><span class="sxs-lookup"><span data-stu-id="28889-131">Type</span></span> | <span data-ttu-id="28889-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28889-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="28889-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="28889-133">Authorization</span></span>  | <span data-ttu-id="28889-134">string</span><span class="sxs-lookup"><span data-stu-id="28889-134">string</span></span>  | <span data-ttu-id="28889-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="28889-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28889-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28889-137">Request body</span></span>

<span data-ttu-id="28889-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="28889-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28889-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="28889-139">Response</span></span>

<span data-ttu-id="28889-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28889-140">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28889-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28889-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="28889-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28889-142">Request</span></span>

<span data-ttu-id="28889-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28889-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="28889-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="28889-144">Response</span></span>

<span data-ttu-id="28889-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="28889-145">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
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
