<span data-ttu-id="4c7a7-p101">Mit der einfachen Upload-API können Sie den Inhalt einer neuen Datei bereitstellen oder den Inhalt einer vorhandenen Datei in einem einzigen API-Aufruf aktualisieren . Diese Methode unterstützt nur Dateien, die bis zu 4MB groß sind.</span><span class="sxs-lookup"><span data-stu-id="4c7a7-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

Mit der einfachen Upload-API können Sie den Inhalt einer neuen Datei bereitstellen oder den Inhalt einer vorhandenen Datei in einem einzigen API-Aufruf aktualisieren . Diese Methode unterstützt nur Dateien, die bis zu 4MB groß sind.

<span data-ttu-id="4c7a7-104">Informationen zum Hochladen großer Dateien finden Sie unter [Hochladen großer Dateien mit einer Uploadsitzung](item_createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="4c7a7-104">To upload large files see [Upload large files with an upload session](item_createuploadsession.md).</span></span>

## <span data-ttu-id="4c7a7-105">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4c7a7-105">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="4c7a7-106">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="4c7a7-106">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="4c7a7-107">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c7a7-107">Files.ReadWrite</span></span>
* <span data-ttu-id="4c7a7-108">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c7a7-108">Files.ReadWrite.All</span></span>
* <span data-ttu-id="4c7a7-109">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c7a7-109">Sites.ReadWrite.All</span></span>


## <span data-ttu-id="4c7a7-110">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c7a7-110">HTTP request</span></span>
<a id="http-request" class="xliff"></a>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/root:/{parent-path}/{filename}:/content
PUT /me/drive/items/{parent-id}/children/{filename}/content
PUT /groups/{id}/drive/items/{parent-id}/children/{filename}/content
```

## <span data-ttu-id="4c7a7-111">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4c7a7-111">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="4c7a7-112">Der Inhalt des Anforderungstexts sollte den binären Stream der hochzuladenden Datei sein.</span><span class="sxs-lookup"><span data-stu-id="4c7a7-112">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <span data-ttu-id="4c7a7-113">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c7a7-113">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="4c7a7-114">Wenn die Methode erfolgreich verläuft, wird ein [driveItem](../resources/driveitem.md)-Objekt im Antworttext der neu erstellten Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4c7a7-114">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created file.</span></span>

## <span data-ttu-id="4c7a7-115">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4c7a7-115">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="4c7a7-116">In diesem Beispiel wird eine Datei über den Pfad zu der angemeldeten Benutzer OneDrive hoch geladen.</span><span class="sxs-lookup"><span data-stu-id="4c7a7-116">This example uploads a file by path to the signed-in user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "upload_item"
}-->
```http
PUT /me/drive/root:/{item-path}:/content
Content-type: text/plain

The contents of the file goes here.
```

## <span data-ttu-id="4c7a7-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c7a7-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="4c7a7-118">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4c7a7-118">Here is an example of the response.</span></span>
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
