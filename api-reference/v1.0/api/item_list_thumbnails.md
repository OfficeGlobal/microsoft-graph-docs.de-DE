# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="d0991-101">Miniaturansichten für ein DriveItem auflisten</span><span class="sxs-lookup"><span data-stu-id="d0991-101">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="d0991-102">Hier erklären wir Ihnen, wie Sie eine Liste der [ThumbnailSet](../resources/thumbnailset.md)-Ressourcen einer [DriveItem](../resources/driveitem.md)-Ressource abrufen können.</span><span class="sxs-lookup"><span data-stu-id="d0991-102">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="d0991-p101">Ein DriveItem kann durch 0 oder mehr [ThumbnailSet](../resources/thumbnailset.md)-Ressourcen repräsentiert werden. Jedes **thumbnailSet** kann ein oder mehrere [**thumbnail**](../resources/thumbnail.md)-Objekte haben. Dabei handelt es sich um Bilder, die das jeweilige Element darstellen. Beispielsweise könnte ein **thumbnailSet** gängige **thumbnail**-Objekte wie `small`, `medium` oder `large` enthalten.</span><span class="sxs-lookup"><span data-stu-id="d0991-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="d0991-p102">Es gibt viele Möglichkeiten, auf OneDrive mit Miniaturansichten zu arbeiten. Die häufigsten:</span><span class="sxs-lookup"><span data-stu-id="d0991-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="d0991-108">Enumerieren der für ein Element verfügbaren Miniaturansichten</span><span class="sxs-lookup"><span data-stu-id="d0991-108">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="d0991-109">Abrufen einer einzelnen Miniaturansicht für ein Element</span><span class="sxs-lookup"><span data-stu-id="d0991-109">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="d0991-110">Abrufen von Miniaturansichtinhalten</span><span class="sxs-lookup"><span data-stu-id="d0991-110">Retrieve thumbnail content</span></span>
* <span data-ttu-id="d0991-111">Abrufen von Miniaturansichten für mehrere Elemente in einer einzigen Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0991-111">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="d0991-112">Abrufen von benutzerdefinierten Miniaturansichtgrößen</span><span class="sxs-lookup"><span data-stu-id="d0991-112">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="d0991-113">Hochladen einer benutzerdefinierten Miniaturansicht für ein Element</span><span class="sxs-lookup"><span data-stu-id="d0991-113">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="d0991-114">Ermitteln, ob eine benutzerdefinierte Miniaturansicht hochgeladen wurde</span><span class="sxs-lookup"><span data-stu-id="d0991-114">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="d0991-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d0991-115">Permissions</span></span>
<span data-ttu-id="d0991-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d0991-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d0991-118">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d0991-118">Permission type</span></span>      | <span data-ttu-id="d0991-119">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d0991-119">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="d0991-120">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d0991-120">Delegated (work or school account)</span></span> | <span data-ttu-id="d0991-121">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0991-121">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="d0991-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d0991-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0991-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0991-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="d0991-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d0991-124">Application</span></span> | <span data-ttu-id="d0991-125">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0991-125">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d0991-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0991-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0991-127">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d0991-127">Optional query parameters</span></span>
<span data-ttu-id="d0991-128">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d0991-128">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="d0991-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d0991-129">Request body</span></span>
<span data-ttu-id="d0991-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d0991-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0991-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0991-131">Response</span></span>

<span data-ttu-id="d0991-132">Bei Erfolg gibt diese Methode einen Antwortcode des Typs `200 OK` und eine Sammlung von [ThumbnailSet](../resources/thumbnailset.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d0991-132">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0991-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d0991-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d0991-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0991-134">Request</span></span>

<span data-ttu-id="d0991-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d0991-135">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_thumbnails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails
```


##### <a name="response"></a><span data-ttu-id="d0991-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0991-136">Response</span></span>
<span data-ttu-id="d0991-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d0991-137">Here is an example of the response.</span></span>

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

## <a name="retrieve-a-single-thumbnail"></a><span data-ttu-id="d0991-138">Abrufen einer einzelnen Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="d0991-138">Retrieve a single thumbnail</span></span>

<span data-ttu-id="d0991-139">Sie können die Metadaten einer einzelnen Miniaturansicht sowie ihre Größe abrufen, indem Sie sie in einer Anforderung direkt adressieren.</span><span class="sxs-lookup"><span data-stu-id="d0991-139">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

## <a name="http-request"></a><span data-ttu-id="d0991-140">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0991-140">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="d0991-141">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="d0991-141">Path parameters</span></span>

| <span data-ttu-id="d0991-142">Name</span><span class="sxs-lookup"><span data-stu-id="d0991-142">Name</span></span>         | <span data-ttu-id="d0991-143">Typ</span><span class="sxs-lookup"><span data-stu-id="d0991-143">Type</span></span>   | <span data-ttu-id="d0991-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0991-144">Description</span></span>                                                                         |
|:-------------|:-------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="d0991-145">**item-id**</span><span class="sxs-lookup"><span data-stu-id="d0991-145">**item-id**</span></span>  | <span data-ttu-id="d0991-146">string</span><span class="sxs-lookup"><span data-stu-id="d0991-146">string</span></span> | <span data-ttu-id="d0991-147">Der eindeutige Bezeichner für das referenzierte Element</span><span class="sxs-lookup"><span data-stu-id="d0991-147">The unique identifier for the item referenced.</span></span>                                      |
| <span data-ttu-id="d0991-148">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="d0991-148">**thumb-id**</span></span> | <span data-ttu-id="d0991-149">number</span><span class="sxs-lookup"><span data-stu-id="d0991-149">number</span></span> | <span data-ttu-id="d0991-150">Der Index der Miniaturansicht, in der Regel 0 bis 4</span><span class="sxs-lookup"><span data-stu-id="d0991-150">The index of the thumbnail, usually 0-4.</span></span>                                            |
| <span data-ttu-id="d0991-151">**size**</span><span class="sxs-lookup"><span data-stu-id="d0991-151">**size**</span></span>     | <span data-ttu-id="d0991-152">string</span><span class="sxs-lookup"><span data-stu-id="d0991-152">string</span></span> | <span data-ttu-id="d0991-p104">Die Größe der angeforderten Miniaturansicht. Dabei muss es sich um eine der aufgeführten Standardgrößen handeln.</span><span class="sxs-lookup"><span data-stu-id="d0991-p104">The size of the thumbnail requested. This must be one of the standard sizes listed.</span></span> |


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

## <a name="retrieve-thumbnail-content"></a><span data-ttu-id="d0991-155">Abrufen von Miniaturansichtinhalten</span><span class="sxs-lookup"><span data-stu-id="d0991-155">Retrieve thumbnail content</span></span>

<span data-ttu-id="d0991-156">Sie können den Inhalt einer Miniaturansicht direkt abrufen, indem Sie die Eigenschaft **content** der Miniaturansicht anfordern.</span><span class="sxs-lookup"><span data-stu-id="d0991-156">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

## <a name="http-request"></a><span data-ttu-id="d0991-157">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0991-157">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

## <a name="response"></a><span data-ttu-id="d0991-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0991-158">Response</span></span>

<span data-ttu-id="d0991-159">Der Dienst antwortet mit einer Umleitung auf die Miniaturansicht-URL.</span><span class="sxs-lookup"><span data-stu-id="d0991-159">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="d0991-p105">URLs zu Miniaturansichtinhalten sind vorab authentifiziert. Der Download eines Autorisierungsheaders ist nicht erforderlich. Diese URLs sind kurzlebig und nur für wenige Stunden gültig. Sie sollten nicht von Apps zwischengespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="d0991-p105">Thumbnail content URLs are pre-authenticated and do not require an authorization header to be downloaded. These URLs are short lived and only valid for a few hours and should not be cached by apps.</span></span>


## <a name="size-values"></a><span data-ttu-id="d0991-162">Größenwerte</span><span class="sxs-lookup"><span data-stu-id="d0991-162">Size values</span></span>

<span data-ttu-id="d0991-p106">In dieser Tabelle sind die möglichen Miniaturansichtgrößen definiert. Zwar können Sie jede beliebige Miniaturansichtgröße anfordern; bei den definierten Werten ist es jedoch wahrscheinlich, dass sie existieren und dass schnell ein Wert zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="d0991-p106">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="d0991-165">Name</span><span class="sxs-lookup"><span data-stu-id="d0991-165">Name</span></span>           | <span data-ttu-id="d0991-166">Auflösung</span><span class="sxs-lookup"><span data-stu-id="d0991-166">Resolution</span></span>  | <span data-ttu-id="d0991-167">Seitenverhältnis</span><span class="sxs-lookup"><span data-stu-id="d0991-167">Aspect Ratio</span></span> | <span data-ttu-id="d0991-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0991-168">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="d0991-169">96 longest
</span><span class="sxs-lookup"><span data-stu-id="d0991-169">96 longest</span></span>  | <span data-ttu-id="d0991-170">Original</span><span class="sxs-lookup"><span data-stu-id="d0991-170">Original</span></span>     | <span data-ttu-id="d0991-171">Kleine, stark komprimierte Miniaturansicht, zugeschnitten auf ein quadratisches Seitenverhältnis</span><span class="sxs-lookup"><span data-stu-id="d0991-171">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="d0991-172">176 longest</span><span class="sxs-lookup"><span data-stu-id="d0991-172">176 longest</span></span> | <span data-ttu-id="d0991-173">Original</span><span class="sxs-lookup"><span data-stu-id="d0991-173">Original</span></span>     | <span data-ttu-id="d0991-174">Zugeschnitten auf die standardmäßige Elementgröße für die OneDrive-Webansicht</span><span class="sxs-lookup"><span data-stu-id="d0991-174">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="d0991-175">800 longest
</span><span class="sxs-lookup"><span data-stu-id="d0991-175">800 longest</span></span> | <span data-ttu-id="d0991-176">Original</span><span class="sxs-lookup"><span data-stu-id="d0991-176">Original</span></span>     | <span data-ttu-id="d0991-177">Miniaturansicht, bei der die längste Kante auf 800 Pixel skaliert wurde</span><span class="sxs-lookup"><span data-stu-id="d0991-177">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |

## <a name="remarks"></a><span data-ttu-id="d0991-178">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="d0991-178">Remarks</span></span>

<span data-ttu-id="d0991-179">**Hinweis:** Für OneDrive for Business und SharePoint gilt:</span><span class="sxs-lookup"><span data-stu-id="d0991-179">**Note** In OneDrive for Business and SharePoint:</span></span>

* <span data-ttu-id="d0991-180">Die folgenden Aufrufe können nicht zur Erweiterung der Miniaturansichtsammlung verwendet werden: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span><span class="sxs-lookup"><span data-stu-id="d0991-180">Using these calls to expand the thumbnails collection will not work: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
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
