# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="bede5-101">Miniaturansichten für ein DriveItem auflisten</span><span class="sxs-lookup"><span data-stu-id="bede5-101">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="bede5-102">Hier erklären wir Ihnen, wie Sie eine Liste der [ThumbnailSet](../resources/thumbnailset.md)-Ressourcen einer [DriveItem](../resources/driveitem.md)-Ressource abrufen können.</span><span class="sxs-lookup"><span data-stu-id="bede5-102">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="bede5-p101">Ein DriveItem kann durch 0 oder mehr [ThumbnailSet](../resources/thumbnailset.md)-Ressourcen repräsentiert werden. Jedes **thumbnailSet** kann ein oder mehrere [**thumbnail**](../resources/thumbnail.md)-Objekte haben. Dabei handelt es sich um Bilder, die das jeweilige Element darstellen. Beispielsweise könnte ein **thumbnailSet** gängige **thumbnail**-Objekte wie `small`, `medium` oder `large` enthalten.</span><span class="sxs-lookup"><span data-stu-id="bede5-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="bede5-p102">Es gibt viele Möglichkeiten, auf OneDrive mit Miniaturansichten zu arbeiten. Die häufigsten:</span><span class="sxs-lookup"><span data-stu-id="bede5-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="bede5-108">Enumerieren der für ein Element verfügbaren Miniaturansichten</span><span class="sxs-lookup"><span data-stu-id="bede5-108">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="bede5-109">Abrufen einer einzelnen Miniaturansicht für ein Element</span><span class="sxs-lookup"><span data-stu-id="bede5-109">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="bede5-110">Abrufen von Miniaturansichtinhalten</span><span class="sxs-lookup"><span data-stu-id="bede5-110">Retrieve thumbnail content</span></span>
* <span data-ttu-id="bede5-111">Abrufen von Miniaturansichten für mehrere Elemente in einer einzigen Anforderung</span><span class="sxs-lookup"><span data-stu-id="bede5-111">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="bede5-112">Abrufen von benutzerdefinierten Miniaturansichtgrößen</span><span class="sxs-lookup"><span data-stu-id="bede5-112">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="bede5-113">Hochladen einer benutzerdefinierten Miniaturansicht für ein Element</span><span class="sxs-lookup"><span data-stu-id="bede5-113">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="bede5-114">Ermitteln, ob eine benutzerdefinierte Miniaturansicht hochgeladen wurde</span><span class="sxs-lookup"><span data-stu-id="bede5-114">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="prerequisites"></a><span data-ttu-id="bede5-115">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bede5-115">Prerequisites</span></span>
<span data-ttu-id="bede5-116">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="bede5-116">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="bede5-117">Files.Read</span><span class="sxs-lookup"><span data-stu-id="bede5-117">Files.Read</span></span>
* <span data-ttu-id="bede5-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bede5-118">Files.ReadWrite</span></span>
* <span data-ttu-id="bede5-119">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="bede5-119">Files.Read.All</span></span>
* <span data-ttu-id="bede5-120">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bede5-120">Files.ReadWrite.All</span></span>
* <span data-ttu-id="bede5-121">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="bede5-121">Sites.Read.All</span></span>
* <span data-ttu-id="bede5-122">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bede5-122">Sites.ReadWrite.All</span></span>


## <a name="http-request"></a><span data-ttu-id="bede5-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bede5-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bede5-124">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bede5-124">Optional query parameters</span></span>
<span data-ttu-id="bede5-125">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bede5-125">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="bede5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bede5-126">Request body</span></span>
<span data-ttu-id="bede5-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bede5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bede5-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="bede5-128">Response</span></span>

<span data-ttu-id="bede5-129">Bei Erfolg gibt diese Methode einen Antwortcode des Typs `200 OK` und eine Sammlung von [ThumbnailSet](../resources/thumbnailset.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bede5-129">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bede5-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bede5-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bede5-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bede5-131">Request</span></span>

<span data-ttu-id="bede5-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bede5-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_thumbnails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails
```


##### <a name="response"></a><span data-ttu-id="bede5-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="bede5-133">Response</span></span>
<span data-ttu-id="bede5-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bede5-134">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0",
      "small": { "height": 64, "width": 96, "url": "https://sn3302files..."},
      "medium": { "height": 117, "width": 176, "url": "https://sn3302files..."},
      "large": { "height": 533, "width": 800, "url": "https://sn3302files..."}
    }
  ]
}
```

## <a name="retrieve-a-single-thumbnail"></a><span data-ttu-id="bede5-135">Abrufen einer einzelnen Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="bede5-135">Retrieve a single thumbnail</span></span>

<span data-ttu-id="bede5-136">Sie können die Metadaten einer einzelnen Miniaturansicht sowie ihre Größe abrufen, indem Sie sie in einer Anforderung direkt adressieren.</span><span class="sxs-lookup"><span data-stu-id="bede5-136">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

## <a name="http-request"></a><span data-ttu-id="bede5-137">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bede5-137">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="bede5-138">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="bede5-138">Path parameters</span></span>

| <span data-ttu-id="bede5-139">Name</span><span class="sxs-lookup"><span data-stu-id="bede5-139">Name</span></span>         | <span data-ttu-id="bede5-140">Typ</span><span class="sxs-lookup"><span data-stu-id="bede5-140">Type</span></span>   | <span data-ttu-id="bede5-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bede5-141">Description</span></span>                                                                         |
|:-------------|:-------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="bede5-142">**item-id**</span><span class="sxs-lookup"><span data-stu-id="bede5-142">**item-id**</span></span>  | <span data-ttu-id="bede5-143">string</span><span class="sxs-lookup"><span data-stu-id="bede5-143">string</span></span> | <span data-ttu-id="bede5-144">Der eindeutige Bezeichner für das referenzierte Element</span><span class="sxs-lookup"><span data-stu-id="bede5-144">The unique identifier for the item referenced.</span></span>                                      |
| <span data-ttu-id="bede5-145">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="bede5-145">**thumb-id**</span></span> | <span data-ttu-id="bede5-146">number</span><span class="sxs-lookup"><span data-stu-id="bede5-146">number</span></span> | <span data-ttu-id="bede5-147">Der Index der Miniaturansicht, in der Regel 0 bis 4</span><span class="sxs-lookup"><span data-stu-id="bede5-147">The index of the thumbnail, usually 0-4.</span></span>                                            |
| <span data-ttu-id="bede5-148">**size**</span><span class="sxs-lookup"><span data-stu-id="bede5-148">**size**</span></span>     | <span data-ttu-id="bede5-149">string</span><span class="sxs-lookup"><span data-stu-id="bede5-149">string</span></span> | <span data-ttu-id="bede5-p103">Die Größe der angeforderten Miniaturansicht. Dabei muss es sich um eine der aufgeführten Standardgrößen handeln.</span><span class="sxs-lookup"><span data-stu-id="bede5-p103">The size of the thumbnail requested. This must be one of the standard sizes listed.</span></span> |


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "http://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-content"></a><span data-ttu-id="bede5-152">Abrufen von Miniaturansichtinhalten</span><span class="sxs-lookup"><span data-stu-id="bede5-152">Retrieve thumbnail content</span></span>

<span data-ttu-id="bede5-153">Sie können den Inhalt einer Miniaturansicht direkt abrufen, indem Sie die Eigenschaft **content** der Miniaturansicht anfordern.</span><span class="sxs-lookup"><span data-stu-id="bede5-153">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

## <a name="http-request"></a><span data-ttu-id="bede5-154">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bede5-154">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

## <a name="response"></a><span data-ttu-id="bede5-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="bede5-155">Response</span></span>

<span data-ttu-id="bede5-156">Der Dienst antwortet mit einer Umleitung auf die Miniaturansicht-URL.</span><span class="sxs-lookup"><span data-stu-id="bede5-156">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="bede5-p104">URLs zu Miniaturansichtinhalten sind vorab authentifiziert. Der Download eines Autorisierungsheaders ist nicht erforderlich. Diese URLs sind kurzlebig und nur für wenige Stunden gültig. Sie sollten nicht von Apps zwischengespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="bede5-p104">Thumbnail content URLs are pre-authenticated and do not require an authorization header to be downloaded. These URLs are short lived and only valid for a few hours and should not be cached by apps.</span></span>


## <a name="size-values"></a><span data-ttu-id="bede5-159">Größenwerte</span><span class="sxs-lookup"><span data-stu-id="bede5-159">Size values</span></span>

<span data-ttu-id="bede5-p105">In dieser Tabelle sind die möglichen Miniaturansichtgrößen definiert. Zwar können Sie jede beliebige Miniaturansichtgröße anfordern; bei den definierten Werten ist es jedoch wahrscheinlich, dass sie existieren und dass schnell ein Wert zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="bede5-p105">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="bede5-162">Name</span><span class="sxs-lookup"><span data-stu-id="bede5-162">Name</span></span>           | <span data-ttu-id="bede5-163">Auflösung</span><span class="sxs-lookup"><span data-stu-id="bede5-163">Resolution</span></span>  | <span data-ttu-id="bede5-164">Seitenverhältnis</span><span class="sxs-lookup"><span data-stu-id="bede5-164">Aspect Ratio</span></span> | <span data-ttu-id="bede5-165">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bede5-165">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="bede5-166">96 longest
</span><span class="sxs-lookup"><span data-stu-id="bede5-166">96 longest</span></span>  | <span data-ttu-id="bede5-167">Original</span><span class="sxs-lookup"><span data-stu-id="bede5-167">Original</span></span>     | <span data-ttu-id="bede5-168">Kleine, stark komprimierte Miniaturansicht, zugeschnitten auf ein quadratisches Seitenverhältnis</span><span class="sxs-lookup"><span data-stu-id="bede5-168">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="bede5-169">176 longest</span><span class="sxs-lookup"><span data-stu-id="bede5-169">176 longest</span></span> | <span data-ttu-id="bede5-170">Original</span><span class="sxs-lookup"><span data-stu-id="bede5-170">Original</span></span>     | <span data-ttu-id="bede5-171">Zugeschnitten auf die standardmäßige Elementgröße für die OneDrive-Webansicht</span><span class="sxs-lookup"><span data-stu-id="bede5-171">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="bede5-172">800 longest
</span><span class="sxs-lookup"><span data-stu-id="bede5-172">800 longest</span></span> | <span data-ttu-id="bede5-173">Original</span><span class="sxs-lookup"><span data-stu-id="bede5-173">Original</span></span>     | <span data-ttu-id="bede5-174">Miniaturansicht, bei der die längste Kante auf 800 Pixel skaliert wurde</span><span class="sxs-lookup"><span data-stu-id="bede5-174">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |

## <a name="remarks"></a><span data-ttu-id="bede5-175">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="bede5-175">Remarks</span></span>

<span data-ttu-id="bede5-176">**Hinweis:** Für OneDrive for Business und SharePoint gilt:</span><span class="sxs-lookup"><span data-stu-id="bede5-176">**Note** In OneDrive for Business and SharePoint:</span></span>

* <span data-ttu-id="bede5-177">Die folgenden Aufrufe können nicht zur Erweiterung der Miniaturansichtsammlung verwendet werden: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span><span class="sxs-lookup"><span data-stu-id="bede5-177">Using these calls to expand the thumbnails collection will not work: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
