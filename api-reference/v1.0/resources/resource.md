# <a name="resource-resource-type"></a><span data-ttu-id="be699-101">resource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="be699-101">resource resource type</span></span>

<span data-ttu-id="be699-102">Ein Bild oder eine andere Dateiressource auf einer OneNote-Seite.</span><span class="sxs-lookup"><span data-stu-id="be699-102">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="be699-103">Sie können die Binärdaten einer Ressource abrufen, der Abruf einer JSON-Darstellung eines Ressourcenobjekts oder einer Ressourcensammlung wird jedoch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="be699-103">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="be699-104">Rufen Sie die Binärdaten einer bestimmten Ressource ab, indem Sie eine GET-Anforderung an den Endpunkt `content` der Ressourcen senden:</span><span class="sxs-lookup"><span data-stu-id="be699-104">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="be699-105">Der Ressourcen-URI der Datei wird zurückgegeben, wenn Sie den HTML-Inhalt einer Seite mit der folgenden Anforderung abrufen:</span><span class="sxs-lookup"><span data-stu-id="be699-105">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="be699-106">Im HTML-Code der Seite schließt ein `img`-Tag Endpunkte für die ursprüngliche Bildressource in das Attribut `data-fullres-src` und das optimierte Bild in das Attribut `src` ein:</span><span class="sxs-lookup"><span data-stu-id="be699-106">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="be699-107">Ein `object`-Tag (das Dateien wie PDF, DOCX und PNG darstellt) schließt den Endpunkt für die Dateiressource in das Attribut `data` ein:</span><span class="sxs-lookup"><span data-stu-id="be699-107">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="be699-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="be699-108">Properties</span></span>
<span data-ttu-id="be699-109">Keine.</span><span class="sxs-lookup"><span data-stu-id="be699-109">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="be699-110">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="be699-110">Relationships</span></span>
<span data-ttu-id="be699-111">Keine.</span><span class="sxs-lookup"><span data-stu-id="be699-111">None.</span></span>


## <a name="methods"></a><span data-ttu-id="be699-112">Methoden</span><span class="sxs-lookup"><span data-stu-id="be699-112">Methods</span></span>
| <span data-ttu-id="be699-113">Methode</span><span class="sxs-lookup"><span data-stu-id="be699-113">Method</span></span>           | <span data-ttu-id="be699-114">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="be699-114">Return Type</span></span>    |<span data-ttu-id="be699-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be699-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be699-116">Binärdaten von Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="be699-116">Get resource binary data</span></span>](../api/resource_get.md) | <span data-ttu-id="be699-117">Stream</span><span class="sxs-lookup"><span data-stu-id="be699-117">Stream</span></span> |<span data-ttu-id="be699-118">Dient zum Abrufen der Binärdaten einer Datei- oder Bildressource.</span><span class="sxs-lookup"><span data-stu-id="be699-118">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->