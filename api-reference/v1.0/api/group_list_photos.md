# <a name="list-photos"></a><span data-ttu-id="c825f-101">Auflisten von Fotos</span><span class="sxs-lookup"><span data-stu-id="c825f-101">List photos</span></span>

<span data-ttu-id="c825f-102">Mit dieser API können Sie eine Liste von Objekten des Typs [profilePhoto](../resources/profilephoto.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="c825f-102">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c825f-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c825f-103">Permissions</span></span>
<span data-ttu-id="c825f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c825f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c825f-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c825f-106">Permission type</span></span>      | <span data-ttu-id="c825f-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c825f-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c825f-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c825f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c825f-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c825f-109">Group.Read.All, Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="c825f-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c825f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c825f-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c825f-111">Not supported.</span></span>    | 
|<span data-ttu-id="c825f-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c825f-112">Application</span></span> | <span data-ttu-id="c825f-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c825f-113">Group.Read.All, Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c825f-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c825f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c825f-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c825f-115">Optional query parameters</span></span>
<span data-ttu-id="c825f-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c825f-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c825f-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c825f-117">Request headers</span></span>
| <span data-ttu-id="c825f-118">Name</span><span class="sxs-lookup"><span data-stu-id="c825f-118">Name</span></span>       | <span data-ttu-id="c825f-119">Typ</span><span class="sxs-lookup"><span data-stu-id="c825f-119">Type</span></span> | <span data-ttu-id="c825f-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c825f-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c825f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c825f-121">Authorization</span></span>  | <span data-ttu-id="c825f-122">string</span><span class="sxs-lookup"><span data-stu-id="c825f-122">string</span></span>  | <span data-ttu-id="c825f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c825f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c825f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c825f-125">Request body</span></span>
<span data-ttu-id="c825f-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c825f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c825f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c825f-127">Response</span></span>

<span data-ttu-id="c825f-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von  [profilePhoto](../resources/profilephoto.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c825f-128">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c825f-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c825f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c825f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c825f-130">Request</span></span>
<span data-ttu-id="c825f-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c825f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```
##### <a name="response"></a><span data-ttu-id="c825f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="c825f-132">Response</span></span>
<span data-ttu-id="c825f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c825f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 94

{
  "value": [
    {
      "height": 99,
      "width": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->