# <a name="onenoteresource-resource-type"></a><span data-ttu-id="0d65e-101">Ressourcentyp OneNoteResource</span><span class="sxs-lookup"><span data-stu-id="0d65e-101">OneNoteResource resource type</span></span>

<span data-ttu-id="0d65e-102">Ein Bild oder eine andere Dateiressource auf einer OneNote-Seite.</span><span class="sxs-lookup"><span data-stu-id="0d65e-102">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="0d65e-103">Sie können die Binärdaten einer Ressource abrufen, der Abruf einer JSON-Darstellung eines Ressourcenobjekts oder einer Ressourcensammlung wird jedoch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d65e-103">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

<span data-ttu-id="0d65e-104">Rufen Sie die Binärdaten einer bestimmten Ressource ab, indem Sie eine GET-Anforderung an den Endpunkt `content` der Ressourcen senden:</span><span class="sxs-lookup"><span data-stu-id="0d65e-104">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="0d65e-105">Der Ressourcen-URI der Datei wird zurückgegeben, wenn Sie den HTML-Inhalt einer Seite mit der folgenden Anforderung abrufen:</span><span class="sxs-lookup"><span data-stu-id="0d65e-105">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="0d65e-106">Im HTML-Code der Seite schließt ein `img`-Tag Endpunkte für die ursprüngliche Bildressource in das Attribut `data-fullres-src` und das optimierte Bild in das Attribut `src` ein:</span><span class="sxs-lookup"><span data-stu-id="0d65e-106">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="0d65e-107">Ein `object`-Tag (das Dateien wie PDF, DOCX und PNG darstellt) schließt den Endpunkt für die Dateiressource in das Attribut `data` ein:</span><span class="sxs-lookup"><span data-stu-id="0d65e-107">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="0d65e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0d65e-108">Properties</span></span>

| <span data-ttu-id="0d65e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d65e-109">Property</span></span>             | <span data-ttu-id="0d65e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="0d65e-110">Type</span></span>            | <span data-ttu-id="0d65e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d65e-111">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="0d65e-112">Inhalt</span><span class="sxs-lookup"><span data-stu-id="0d65e-112">content</span></span>              | <span data-ttu-id="0d65e-113">Stream</span><span class="sxs-lookup"><span data-stu-id="0d65e-113">Stream</span></span>          | <span data-ttu-id="0d65e-114">Der Inhaltsstream</span><span class="sxs-lookup"><span data-stu-id="0d65e-114">The content stream.</span></span>
| <span data-ttu-id="0d65e-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="0d65e-115">contentUrl</span></span>           | <span data-ttu-id="0d65e-116">Zeichenfolge (URL)</span><span class="sxs-lookup"><span data-stu-id="0d65e-116">string (url)</span></span>    | <span data-ttu-id="0d65e-117">Die URL für das Herunterladen von Inhalten</span><span class="sxs-lookup"><span data-stu-id="0d65e-117">The URL for the page's HTML content.  Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="0d65e-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0d65e-118">Relationships</span></span>
<span data-ttu-id="0d65e-119">Keine.</span><span class="sxs-lookup"><span data-stu-id="0d65e-119">None.</span></span>


## <a name="methods"></a><span data-ttu-id="0d65e-120">Methoden</span><span class="sxs-lookup"><span data-stu-id="0d65e-120">Methods</span></span>
| <span data-ttu-id="0d65e-121">Methode</span><span class="sxs-lookup"><span data-stu-id="0d65e-121">Method</span></span>           | <span data-ttu-id="0d65e-122">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0d65e-122">Return Type</span></span>    |<span data-ttu-id="0d65e-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d65e-123">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d65e-124">Binärdaten von Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="0d65e-124">Get resource binary data</span></span>](../api/resource_get.md) | <span data-ttu-id="0d65e-125">Stream</span><span class="sxs-lookup"><span data-stu-id="0d65e-125">Stream</span></span> |<span data-ttu-id="0d65e-126">Dient zum Abrufen der Binärdaten einer Datei- oder Bildressource.</span><span class="sxs-lookup"><span data-stu-id="0d65e-126">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->