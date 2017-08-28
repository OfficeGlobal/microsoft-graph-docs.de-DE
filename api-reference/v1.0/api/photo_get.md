# <a name="get-photo"></a><span data-ttu-id="34471-101">Foto abrufen</span><span class="sxs-lookup"><span data-stu-id="34471-101">Get photo</span></span>

<span data-ttu-id="34471-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Fotoobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="34471-102">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="34471-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="34471-103">Permissions</span></span>
<span data-ttu-id="34471-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="34471-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="34471-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34471-106">Permission type</span></span>      | <span data-ttu-id="34471-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34471-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34471-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34471-108">Delegated (work or school account)</span></span> | <span data-ttu-id="34471-109">Files.Read</span><span class="sxs-lookup"><span data-stu-id="34471-109">Files.Read</span></span>    |
|<span data-ttu-id="34471-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34471-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34471-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="34471-111">Files.Read</span></span>    |
|<span data-ttu-id="34471-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34471-112">Application</span></span> | <span data-ttu-id="34471-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34471-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34471-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34471-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="34471-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="34471-115">Optional query parameters</span></span>
<span data-ttu-id="34471-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="34471-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34471-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="34471-117">Request headers</span></span>
| <span data-ttu-id="34471-118">Name</span><span class="sxs-lookup"><span data-stu-id="34471-118">Name</span></span>       | <span data-ttu-id="34471-119">Typ</span><span class="sxs-lookup"><span data-stu-id="34471-119">Type</span></span> | <span data-ttu-id="34471-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34471-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="34471-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="34471-121">Authorization</span></span>  | <span data-ttu-id="34471-122">string</span><span class="sxs-lookup"><span data-stu-id="34471-122">string</span></span>  | <span data-ttu-id="34471-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="34471-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34471-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="34471-125">Request body</span></span>
<span data-ttu-id="34471-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="34471-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34471-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="34471-127">Response</span></span>

<span data-ttu-id="34471-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [photo](../resources/photo.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34471-128">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34471-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34471-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34471-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34471-130">Request</span></span>
<span data-ttu-id="34471-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="34471-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="34471-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="34471-132">Response</span></span>
<span data-ttu-id="34471-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="34471-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
