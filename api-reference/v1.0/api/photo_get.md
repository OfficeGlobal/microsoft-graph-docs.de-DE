# <a name="get-photo"></a><span data-ttu-id="39f08-101">Foto abrufen</span><span class="sxs-lookup"><span data-stu-id="39f08-101">Get photo</span></span>

<span data-ttu-id="39f08-102">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Fotoobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="39f08-102">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="39f08-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="39f08-103">Permissions</span></span>
<span data-ttu-id="39f08-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="39f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="39f08-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39f08-106">Permission type</span></span>      | <span data-ttu-id="39f08-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39f08-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39f08-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39f08-108">Delegated (work or school account)</span></span> | <span data-ttu-id="39f08-109">Files.Read</span><span class="sxs-lookup"><span data-stu-id="39f08-109">Files.Read</span></span>    |
|<span data-ttu-id="39f08-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39f08-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39f08-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="39f08-111">Files.Read</span></span>    |
|<span data-ttu-id="39f08-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39f08-112">Application</span></span> | <span data-ttu-id="39f08-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39f08-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39f08-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39f08-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="39f08-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="39f08-115">Optional query parameters</span></span>
<span data-ttu-id="39f08-116">Diese Methode unterstützt die [OData-Abfrageparameter]((http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters)) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="39f08-116">This method supports the [OData Query Parameters]((http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters)) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39f08-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39f08-117">Request headers</span></span>
| <span data-ttu-id="39f08-118">Name</span><span class="sxs-lookup"><span data-stu-id="39f08-118">Name</span></span>       | <span data-ttu-id="39f08-119">Typ</span><span class="sxs-lookup"><span data-stu-id="39f08-119">Type</span></span> | <span data-ttu-id="39f08-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39f08-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="39f08-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="39f08-121">Authorization</span></span>  | <span data-ttu-id="39f08-122">string</span><span class="sxs-lookup"><span data-stu-id="39f08-122">string</span></span>  | <span data-ttu-id="39f08-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="39f08-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39f08-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39f08-125">Request body</span></span>
<span data-ttu-id="39f08-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="39f08-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39f08-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="39f08-127">Response</span></span>

<span data-ttu-id="39f08-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [photo](../resources/photo.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39f08-128">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="39f08-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39f08-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39f08-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39f08-130">Request</span></span>
<span data-ttu-id="39f08-131">Dies ist ein Beispiel für die Anforderung von Foto-Metadaten.</span><span class="sxs-lookup"><span data-stu-id="39f08-131">Here is an example of the request for the user's drives.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="39f08-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="39f08-132">Response</span></span>
<span data-ttu-id="39f08-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="39f08-133">Here is an example of the response.</span></span>
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
##### <a name="request"></a><span data-ttu-id="39f08-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39f08-134">Request</span></span>
<span data-ttu-id="39f08-135">Hier ist ein Beispiel für die Anforderung der Fotobytes.</span><span class="sxs-lookup"><span data-stu-id="39f08-135">Here is an example of the request for the user's drives.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="39f08-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="39f08-136">Response</span></span>
<span data-ttu-id="39f08-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="39f08-137">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: image/jpeg
ETag: "A19A6498"
request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
client-request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
x-ms-ags-diagnostic: {"ServerInfo":{"DataCenter":"West US","Slice":"SliceA","Ring":"5","ScaleUnit":"003","Host":"AGSFE_IN_14","ADSiteName":"WST"}}
Access-Control-Allow-Origin: *
Access-Control-Expose-Headers: ETag, Location, Preference-Applied, Content-Range, request-id, client-request-id
Duration: 125.9389
Date: Wed, 13 Dec 2017 22:02:17 GMT
Content-Length: 250526

<binary image data>
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
