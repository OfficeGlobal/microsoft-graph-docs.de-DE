# <a name="list-memberof"></a><span data-ttu-id="f275e-101">memberOf auflisten</span><span class="sxs-lookup"><span data-stu-id="f275e-101">List memberOf</span></span>
<span data-ttu-id="f275e-102">Dient zum Abrufen von Gruppen, von denen die Gruppe ein direktes Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="f275e-102">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="f275e-p101">Dieser Vorgang ist nicht transitiv. Im Gegensatz zum Abrufen der Office 365-Gruppen eines Benutzers werden hier alle Typen von Gruppen zurückgegeben, nicht nur Office 365-Gruppen.</span><span class="sxs-lookup"><span data-stu-id="f275e-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="f275e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f275e-105">Permissions</span></span>
<span data-ttu-id="f275e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f275e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f275e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f275e-108">Permission type</span></span>      | <span data-ttu-id="f275e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f275e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f275e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f275e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f275e-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f275e-111">Group.Read.All</span></span>    |
|<span data-ttu-id="f275e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f275e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f275e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f275e-113">Not supported.</span></span>    |
|<span data-ttu-id="f275e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f275e-114">Application</span></span> | <span data-ttu-id="f275e-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f275e-115">Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f275e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f275e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f275e-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f275e-117">Optional query parameters</span></span>
<span data-ttu-id="f275e-118">Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f275e-118">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f275e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f275e-119">Request headers</span></span>
| <span data-ttu-id="f275e-120">Name</span><span class="sxs-lookup"><span data-stu-id="f275e-120">Name</span></span>       | <span data-ttu-id="f275e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f275e-121">Type</span></span> | <span data-ttu-id="f275e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f275e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f275e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f275e-123">Authorization</span></span>  | <span data-ttu-id="f275e-124">string</span><span class="sxs-lookup"><span data-stu-id="f275e-124">string</span></span>  | <span data-ttu-id="f275e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f275e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f275e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f275e-127">Request body</span></span>
<span data-ttu-id="f275e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f275e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f275e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f275e-129">Response</span></span>
<span data-ttu-id="f275e-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f275e-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f275e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f275e-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f275e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f275e-132">Request</span></span>
<span data-ttu-id="f275e-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f275e-133">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```

#### <a name="response"></a><span data-ttu-id="f275e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f275e-134">Response</span></span>
<span data-ttu-id="f275e-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f275e-135">Here is an example of the response.</span></span>
><span data-ttu-id="f275e-136">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="f275e-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f275e-137">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f275e-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->