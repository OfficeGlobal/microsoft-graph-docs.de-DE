# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="6983f-101">Inhalte von DriveItem hochladen oder ersetzen</span><span class="sxs-lookup"><span data-stu-id="6983f-101">Upload or replace the contents of a driveItem</span></span>

<span data-ttu-id="6983f-p101">Mit der einfachen Upload-API können Sie den Inhalt einer neuen Datei bereitstellen oder den Inhalt einer vorhandenen Datei in einem einzigen API-Aufruf aktualisieren . Diese Methode unterstützt nur Dateien, die bis zu 4MB groß sind.</span><span class="sxs-lookup"><span data-stu-id="6983f-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="6983f-104">Informationen zum Hochladen großer Dateien finden Sie unter [Hochladen großer Dateien mit einer Uploadsitzung](item_createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="6983f-104">To upload large files see [Upload large files with an upload session](item_createuploadsession.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6983f-105">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6983f-105">Prerequisites</span></span>
<span data-ttu-id="6983f-106">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="6983f-106">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="6983f-107">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6983f-107">Files.ReadWrite</span></span>
* <span data-ttu-id="6983f-108">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6983f-108">Files.ReadWrite.All</span></span>
* <span data-ttu-id="6983f-109">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6983f-109">Sites.ReadWrite.All</span></span>


## <a name="http-request"></a><span data-ttu-id="6983f-110">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6983f-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/root:/{parent-path}/{filename}:/content
PUT /me/drive/items/{parent-id}/children/{filename}/content
PUT /groups/{id}/drive/items/{parent-id}/children/{filename}/content
```

## <a name="request-body"></a><span data-ttu-id="6983f-111">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6983f-111">Request body</span></span>
<span data-ttu-id="6983f-112">Der Inhalt des Anforderungstexts sollte den binären Stream der hochzuladenden Datei sein.</span><span class="sxs-lookup"><span data-stu-id="6983f-112">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="6983f-113">Antwort</span><span class="sxs-lookup"><span data-stu-id="6983f-113">Response</span></span>

<span data-ttu-id="6983f-114">Wenn die Methode erfolgreich verläuft, wird ein [driveItem](../resources/driveitem.md)-Objekt im Antworttext der neu erstellten Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6983f-114">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created file.</span></span>

## <a name="example"></a><span data-ttu-id="6983f-115">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6983f-115">Example</span></span>
<span data-ttu-id="6983f-116">In diesem Beispiel wird eine Datei über den Pfad zu der angemeldeten Benutzer OneDrive hoch geladen.</span><span class="sxs-lookup"><span data-stu-id="6983f-116">This example uploads a file by path to the signed-in user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "upload_item"
}-->
```http
PUT /me/drive/root:/{item-path}:/content
Content-type: text/plain

The contents of the file goes here.
```

##### <a name="response"></a><span data-ttu-id="6983f-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="6983f-117">Response</span></span>

<span data-ttu-id="6983f-118">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="6983f-118">The following example shows an Autodiscover error response.</span></span>

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
