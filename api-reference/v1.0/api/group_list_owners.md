# <a name="list-owners"></a><span data-ttu-id="ffc87-101">Besitzer auflisten</span><span class="sxs-lookup"><span data-stu-id="ffc87-101">List owners</span></span>

<span data-ttu-id="ffc87-p101">Dient zum Abrufen einer Liste der Besitzer der Gruppe. Bei den Besitzern handelt es sich um eine Reihe von Benutzern ohne Administratorrechte, die das Gruppenobjekt ändern dürfen.</span><span class="sxs-lookup"><span data-stu-id="ffc87-p101">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ffc87-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ffc87-104">Permissions</span></span>
<span data-ttu-id="ffc87-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ffc87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ffc87-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ffc87-107">Permission type</span></span>      | <span data-ttu-id="ffc87-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ffc87-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffc87-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ffc87-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ffc87-110">Group.Read.All und User.ReadBasic.All, Group.Read.All und User.Read.All, Group.Read.All und User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffc87-110">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="ffc87-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ffc87-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffc87-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ffc87-112">Not supported.</span></span>    |
|<span data-ttu-id="ffc87-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ffc87-113">Application</span></span> | <span data-ttu-id="ffc87-114">Group.Read.All und User.Read.All, Group.Read.All und User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffc87-114">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffc87-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffc87-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ffc87-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ffc87-116">Optional query parameters</span></span>
<span data-ttu-id="ffc87-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ffc87-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ffc87-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ffc87-118">Request headers</span></span>
| <span data-ttu-id="ffc87-119">Name</span><span class="sxs-lookup"><span data-stu-id="ffc87-119">Name</span></span>       | <span data-ttu-id="ffc87-120">Typ</span><span class="sxs-lookup"><span data-stu-id="ffc87-120">Type</span></span> | <span data-ttu-id="ffc87-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ffc87-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ffc87-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffc87-122">Authorization</span></span>  | <span data-ttu-id="ffc87-123">string</span><span class="sxs-lookup"><span data-stu-id="ffc87-123">string</span></span>  | <span data-ttu-id="ffc87-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ffc87-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffc87-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ffc87-126">Request body</span></span>
<span data-ttu-id="ffc87-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ffc87-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffc87-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffc87-128">Response</span></span>

<span data-ttu-id="ffc87-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ffc87-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ffc87-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ffc87-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ffc87-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffc87-131">Request</span></span>
<span data-ttu-id="ffc87-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ffc87-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
##### <a name="response"></a><span data-ttu-id="ffc87-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffc87-133">Response</span></span>
<span data-ttu-id="ffc87-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ffc87-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
