# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="866ef-101">Inhalte von DriveItem hochladen oder ersetzen</span><span class="sxs-lookup"><span data-stu-id="866ef-101">Upload or replace the contents of a driveItem</span></span>

<span data-ttu-id="866ef-p101">Mit der einfachen Upload-API können Sie den Inhalt einer neuen Datei bereitstellen oder den Inhalt einer vorhandenen Datei in einem einzigen API-Aufruf aktualisieren . Diese Methode unterstützt nur Dateien, die bis zu 4MB groß sind.</span><span class="sxs-lookup"><span data-stu-id="866ef-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="866ef-104">Informationen zum Hochladen großer Dateien finden Sie unter [Große Dateien mit einer Uploadsitzung hochladen](item_createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="866ef-104">To upload large files see [Upload large files with an upload session](item_createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="866ef-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="866ef-105">Permissions</span></span>
<span data-ttu-id="866ef-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="866ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="866ef-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="866ef-108">Permission type</span></span>      | <span data-ttu-id="866ef-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="866ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="866ef-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="866ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="866ef-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="866ef-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="866ef-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="866ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="866ef-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="866ef-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="866ef-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="866ef-114">Application</span></span> | <span data-ttu-id="866ef-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="866ef-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="866ef-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="866ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/root:/{parent-path}/{filename}:/content
PUT /me/drive/items/{parent-id}/children/{filename}/content
PUT /groups/{id}/drive/items/{parent-id}/children/{filename}/content
```

## <a name="request-body"></a><span data-ttu-id="866ef-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="866ef-117">Request body</span></span>
<span data-ttu-id="866ef-118">Der Inhalt des Anforderungstexts sollte den binären Stream der hochzuladenden Datei sein.</span><span class="sxs-lookup"><span data-stu-id="866ef-118">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="866ef-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="866ef-119">Response</span></span>

<span data-ttu-id="866ef-120">Wenn die Methode erfolgreich verläuft, wird ein [driveItem](../resources/driveitem.md)-Objekt im Antworttext der neu erstellten Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="866ef-120">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created file.</span></span>

## <a name="example"></a><span data-ttu-id="866ef-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="866ef-121">Example</span></span>
<span data-ttu-id="866ef-122">In diesem Beispiel wird eine Datei über den Pfad zu der angemeldeten Benutzer OneDrive hoch geladen.</span><span class="sxs-lookup"><span data-stu-id="866ef-122">This example uploads a file by path to the signed-in user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "upload_item"
}-->
```http
PUT /me/drive/root:/{item-path}:/content
Content-type: text/plain

The contents of the file goes here.
```

##### <a name="response"></a><span data-ttu-id="866ef-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="866ef-123">Response</span></span>

<span data-ttu-id="866ef-124">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="866ef-124">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "myfile.jpg",
  "size": 10191,
  "file": { }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
