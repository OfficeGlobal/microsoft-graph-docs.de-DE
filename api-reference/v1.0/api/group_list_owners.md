# <a name="list-owners"></a><span data-ttu-id="6059e-101">Besitzer auflisten</span><span class="sxs-lookup"><span data-stu-id="6059e-101">List owners</span></span>
<span data-ttu-id="6059e-p101">Dient zum Abrufen einer Liste der Besitzer der Gruppe. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.</span><span class="sxs-lookup"><span data-stu-id="6059e-p101">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6059e-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6059e-104">Permissions</span></span>
<span data-ttu-id="6059e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6059e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6059e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6059e-107">Permission type</span></span>      | <span data-ttu-id="6059e-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6059e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6059e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6059e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6059e-110">Group.Read.All und User.ReadBasic.All, Group.Read.All und User.Read.All, Group.Read.All und User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6059e-110">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="6059e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6059e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6059e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6059e-112">Not supported.</span></span>    |
|<span data-ttu-id="6059e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6059e-113">Application</span></span> | <span data-ttu-id="6059e-114">Group.Read.All und User.Read.All, Group.Read.All und User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6059e-114">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6059e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6059e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6059e-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6059e-116">Optional query parameters</span></span>
<span data-ttu-id="6059e-117">Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6059e-117">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6059e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6059e-118">Request headers</span></span>
| <span data-ttu-id="6059e-119">Name</span><span class="sxs-lookup"><span data-stu-id="6059e-119">Name</span></span>       | <span data-ttu-id="6059e-120">Typ</span><span class="sxs-lookup"><span data-stu-id="6059e-120">Type</span></span> | <span data-ttu-id="6059e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6059e-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6059e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6059e-122">Authorization</span></span>  | <span data-ttu-id="6059e-123">string</span><span class="sxs-lookup"><span data-stu-id="6059e-123">string</span></span>  | <span data-ttu-id="6059e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6059e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6059e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6059e-126">Request body</span></span>
<span data-ttu-id="6059e-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6059e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6059e-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="6059e-128">Response</span></span>
<span data-ttu-id="6059e-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6059e-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6059e-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6059e-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6059e-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6059e-131">Request</span></span>
<span data-ttu-id="6059e-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6059e-132">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="6059e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6059e-133">Response</span></span>
<span data-ttu-id="6059e-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6059e-134">Here is an example of the response.</span></span>
><span data-ttu-id="6059e-135">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="6059e-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6059e-136">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="6059e-136">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
