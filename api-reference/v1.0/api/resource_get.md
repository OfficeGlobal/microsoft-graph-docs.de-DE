# <a name="get-resource"></a><span data-ttu-id="9dc2b-101">Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="9dc2b-101">Get resource</span></span>

<span data-ttu-id="9dc2b-102">Mit dieser API können Sie die Binärdateien eines Objekts des Typs [resource](../resources/resource.md) mit der Eigenschaft „file“ oder der Eigenschaft „image“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="9dc2b-102">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9dc2b-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9dc2b-103">Permissions</span></span>
<span data-ttu-id="9dc2b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9dc2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9dc2b-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9dc2b-106">Permission type</span></span>      | <span data-ttu-id="9dc2b-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9dc2b-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="9dc2b-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9dc2b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9dc2b-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dc2b-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="9dc2b-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9dc2b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dc2b-111">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9dc2b-111">Notes.Read, Notes.ReadWrite</span></span>    | 
|<span data-ttu-id="9dc2b-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9dc2b-112">Application</span></span> | <span data-ttu-id="9dc2b-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dc2b-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9dc2b-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9dc2b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="9dc2b-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9dc2b-115">Request headers</span></span>
| <span data-ttu-id="9dc2b-116">Name</span><span class="sxs-lookup"><span data-stu-id="9dc2b-116">Name</span></span>       | <span data-ttu-id="9dc2b-117">Typ</span><span class="sxs-lookup"><span data-stu-id="9dc2b-117">Type</span></span> | <span data-ttu-id="9dc2b-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9dc2b-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9dc2b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dc2b-119">Authorization</span></span>  | <span data-ttu-id="9dc2b-120">string</span><span class="sxs-lookup"><span data-stu-id="9dc2b-120">string</span></span>  | <span data-ttu-id="9dc2b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9dc2b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9dc2b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9dc2b-123">Request body</span></span>
<span data-ttu-id="9dc2b-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9dc2b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dc2b-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="9dc2b-125">Response</span></span>

<span data-ttu-id="9dc2b-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die Binärdaten des Bilds oder der Datei im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9dc2b-126">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="9dc2b-127">Hinweis: Bilder werden nicht direkt in einem Browser gerendert, da zum Abrufen eine Autorisierung erforderlich ist, ebenso wie für den Rest des Seiteninhalts.</span><span class="sxs-lookup"><span data-stu-id="9dc2b-127">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="9dc2b-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9dc2b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9dc2b-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9dc2b-129">Request</span></span>
<span data-ttu-id="9dc2b-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9dc2b-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="9dc2b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9dc2b-131">Response</span></span>
<span data-ttu-id="9dc2b-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9dc2b-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
