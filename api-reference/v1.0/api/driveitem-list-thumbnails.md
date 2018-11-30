---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Abrufen von Miniaturansichten für eine Datei oder einen Ordner
ms.openlocfilehash: 990c8f6714c188e9468e73ffe35526d3c3825cc2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017092"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="547f1-102">Miniaturansichten für ein DriveItem auflisten</span><span class="sxs-lookup"><span data-stu-id="547f1-102">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="547f1-103">Hier erklären wir Ihnen, wie Sie eine Liste der [ThumbnailSet](../resources/thumbnailset.md)-Ressourcen einer [DriveItem](../resources/driveitem.md)-Ressource abrufen können.</span><span class="sxs-lookup"><span data-stu-id="547f1-103">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="547f1-p101">Ein DriveItem kann durch 0 oder mehr [ThumbnailSet](../resources/thumbnailset.md)-Ressourcen repräsentiert werden. Jedes **thumbnailSet** kann ein oder mehrere [**thumbnail**](../resources/thumbnail.md)-Objekte haben. Dabei handelt es sich um Bilder, die das jeweilige Element darstellen. Beispielsweise könnte ein **thumbnailSet** gängige **thumbnail**-Objekte wie `small`, `medium` oder `large` enthalten.</span><span class="sxs-lookup"><span data-stu-id="547f1-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="547f1-p102">Es gibt viele Möglichkeiten, auf OneDrive mit Miniaturansichten zu arbeiten. Die häufigsten:</span><span class="sxs-lookup"><span data-stu-id="547f1-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="547f1-109">Enumerieren der für ein Element verfügbaren Miniaturansichten</span><span class="sxs-lookup"><span data-stu-id="547f1-109">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="547f1-110">Abrufen einer einzelnen Miniaturansicht für ein Element</span><span class="sxs-lookup"><span data-stu-id="547f1-110">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="547f1-111">Abrufen von Miniaturansichtinhalten</span><span class="sxs-lookup"><span data-stu-id="547f1-111">Retrieve thumbnail content</span></span>
* <span data-ttu-id="547f1-112">Abrufen von Miniaturansichten für mehrere Elemente in einer einzigen Anforderung</span><span class="sxs-lookup"><span data-stu-id="547f1-112">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="547f1-113">Abrufen von benutzerdefinierten Miniaturansichtgrößen</span><span class="sxs-lookup"><span data-stu-id="547f1-113">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="547f1-114">Hochladen einer benutzerdefinierten Miniaturansicht für ein Element</span><span class="sxs-lookup"><span data-stu-id="547f1-114">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="547f1-115">Ermitteln, ob eine benutzerdefinierte Miniaturansicht hochgeladen wurde</span><span class="sxs-lookup"><span data-stu-id="547f1-115">Determine if a custom uploaded thumbnail exists</span></span>

## <a name="permissions"></a><span data-ttu-id="547f1-116">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="547f1-116">Permissions</span></span>

<span data-ttu-id="547f1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="547f1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="547f1-119">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="547f1-119">Permission type</span></span>      | <span data-ttu-id="547f1-120">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="547f1-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="547f1-121">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="547f1-121">Delegated (work or school account)</span></span> | <span data-ttu-id="547f1-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="547f1-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="547f1-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="547f1-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="547f1-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="547f1-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="547f1-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="547f1-125">Application</span></span> | <span data-ttu-id="547f1-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="547f1-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="547f1-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="547f1-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="547f1-128">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="547f1-128">Optional query parameters</span></span>

<span data-ttu-id="547f1-129">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von `$select` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="547f1-129">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="547f1-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="547f1-130">Response</span></span>

<span data-ttu-id="547f1-131">Bei Erfolg gibt diese Methode einen Antwortcode des Typs `200 OK` und eine Sammlung von [ThumbnailSet](../resources/thumbnailset.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="547f1-131">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="547f1-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="547f1-132">Example</span></span>

<span data-ttu-id="547f1-133">Hier ist ein Beispiel für die Anforderung, die verfügbare Miniaturansichten für ein Element im OneDrive des aktuellen Benutzers abruft.</span><span class="sxs-lookup"><span data-stu-id="547f1-133">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```

<span data-ttu-id="547f1-134">Diese gibt ein Array von verfügbaren **thumbnailSets** für das Element zurück.</span><span class="sxs-lookup"><span data-stu-id="547f1-134">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="547f1-135">Ein beliebiges Element auf einem Laufwerk kann Null oder mehr Miniaturansichten aufweisen.</span><span class="sxs-lookup"><span data-stu-id="547f1-135">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="547f1-136">**Hinweis:** Sie können den _select_-Abfragezeichenfolgenparameter verwenden, um zu steuern, welche Miniaturansichtgrößen im **ThumbnailSet** zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="547f1-136">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**.</span></span>
<span data-ttu-id="547f1-137">`/thumbnails?select=medium` ruft beispielsweise nur die mittelgroßen Miniaturansichten ab.</span><span class="sxs-lookup"><span data-stu-id="547f1-137">For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="547f1-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="547f1-138">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="547f1-139">Abrufen einer einzelnen Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="547f1-139">Get a single thumbnail</span></span>

<span data-ttu-id="547f1-140">Sie können die Metadaten einer einzelnen Miniaturansicht sowie ihre Größe abrufen, indem Sie sie in einer Anforderung direkt adressieren.</span><span class="sxs-lookup"><span data-stu-id="547f1-140">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="547f1-141">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="547f1-141">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

### <a name="path-parameters"></a><span data-ttu-id="547f1-142">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="547f1-142">Path parameters</span></span>

| <span data-ttu-id="547f1-143">Name</span><span class="sxs-lookup"><span data-stu-id="547f1-143">Name</span></span>         | <span data-ttu-id="547f1-144">Typ</span><span class="sxs-lookup"><span data-stu-id="547f1-144">Type</span></span>   | <span data-ttu-id="547f1-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="547f1-145">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="547f1-146">**item-id**</span><span class="sxs-lookup"><span data-stu-id="547f1-146">**item-id**</span></span>  | <span data-ttu-id="547f1-147">string</span><span class="sxs-lookup"><span data-stu-id="547f1-147">string</span></span> | <span data-ttu-id="547f1-148">Der eindeutige Bezeichner für das referenzierte Element</span><span class="sxs-lookup"><span data-stu-id="547f1-148">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="547f1-149">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="547f1-149">**thumb-id**</span></span> | <span data-ttu-id="547f1-150">number</span><span class="sxs-lookup"><span data-stu-id="547f1-150">number</span></span> | <span data-ttu-id="547f1-151">Der Index der Miniaturansicht, in der Regel 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="547f1-151">The index of the thumbnail, usually 0-4.</span></span> <span data-ttu-id="547f1-152">Wenn es eine benutzerdefinierte Miniaturansicht gibt, ist ihr Index 0.</span><span class="sxs-lookup"><span data-stu-id="547f1-152">If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="547f1-153">**size**</span><span class="sxs-lookup"><span data-stu-id="547f1-153">**size**</span></span>     | <span data-ttu-id="547f1-154">string</span><span class="sxs-lookup"><span data-stu-id="547f1-154">string</span></span> | <span data-ttu-id="547f1-155">Die Größe der angeforderten Miniaturansicht.</span><span class="sxs-lookup"><span data-stu-id="547f1-155">The size of the thumbnail requested.</span></span> <span data-ttu-id="547f1-156">Dabei kann es sich um eine der nachfolgend aufgeführten Standardgrößen oder um eine benutzerdefinierte Größe handeln.</span><span class="sxs-lookup"><span data-stu-id="547f1-156">This can be one of the standard sizes listed below or a custom size.</span></span> |

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "https://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="547f1-157">Abrufen von binären Miniaturansichtinhalten</span><span class="sxs-lookup"><span data-stu-id="547f1-157">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="547f1-158">Sie können den Inhalt einer Miniaturansicht direkt abrufen, indem Sie die Eigenschaft **content** der Miniaturansicht anfordern.</span><span class="sxs-lookup"><span data-stu-id="547f1-158">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="547f1-159">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="547f1-159">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

### <a name="response"></a><span data-ttu-id="547f1-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="547f1-160">Response</span></span>

<span data-ttu-id="547f1-161">Der Dienst antwortet mit einer Umleitung auf die Miniaturansicht-URL.</span><span class="sxs-lookup"><span data-stu-id="547f1-161">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="547f1-162">Miniaturansicht-URLs sind cachesicher.</span><span class="sxs-lookup"><span data-stu-id="547f1-162">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="547f1-163">Die URL ändert sich, wenn sich das Element derart ändert, dass eine neue Miniaturansicht generiert werden muss.</span><span class="sxs-lookup"><span data-stu-id="547f1-163">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="547f1-164">Abrufen von Miniaturansichten beim Auflisten von DriveItems</span><span class="sxs-lookup"><span data-stu-id="547f1-164">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="547f1-165">Wenn Sie eine Liste der anzuzeigenden DriveItem-Ressourcen abrufen, können Sie mit dem _$expand_-Abfragezeichenfolge-Parameter außerdem die Miniaturansichten für diese Ressourcen aufnehmen.</span><span class="sxs-lookup"><span data-stu-id="547f1-165">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="547f1-166">Dadurch kann Ihre App Miniaturansichten und Elemente in einer einzelnen Anforderung abrufen, statt viele Anforderungen auszuführen.</span><span class="sxs-lookup"><span data-stu-id="547f1-166">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="547f1-167">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="547f1-167">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```

### <a name="response"></a><span data-ttu-id="547f1-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="547f1-168">Response</span></span>

<span data-ttu-id="547f1-169">Die Dienstantworten mit der Liste der DriveItems und ihren Miniaturansichten.</span><span class="sxs-lookup"><span data-stu-id="547f1-169">The service responses with the list of DriveItems and their thumbnails.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "182331E8-2788-4932-B52A-A6550577043F",
      "name": "my photo.jpg",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    },
    {
      "id": "2D223953-A56B-4D9B-ADF3-13E7820673A2",
      "name": "presentation.pptx",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    }
  ]
}
```

## <a name="size-options"></a><span data-ttu-id="547f1-170">Größenoptionen</span><span class="sxs-lookup"><span data-stu-id="547f1-170">Size options</span></span>

<span data-ttu-id="547f1-p110">In dieser Tabelle sind die möglichen Miniaturansichtgrößen definiert. Zwar können Sie jede beliebige Miniaturansichtgröße anfordern; bei den definierten Werten ist es jedoch wahrscheinlich, dass sie existieren und dass schnell ein Wert zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="547f1-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="547f1-173">Name</span><span class="sxs-lookup"><span data-stu-id="547f1-173">Name</span></span>           | <span data-ttu-id="547f1-174">Auflösung</span><span class="sxs-lookup"><span data-stu-id="547f1-174">Resolution</span></span>  | <span data-ttu-id="547f1-175">Seitenverhältnis</span><span class="sxs-lookup"><span data-stu-id="547f1-175">Aspect Ratio</span></span> | <span data-ttu-id="547f1-176">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="547f1-176">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="547f1-177">96 longest
</span><span class="sxs-lookup"><span data-stu-id="547f1-177">96 longest</span></span>  | <span data-ttu-id="547f1-178">Original</span><span class="sxs-lookup"><span data-stu-id="547f1-178">Original</span></span>     | <span data-ttu-id="547f1-179">Kleine, stark komprimierte Miniaturansicht, zugeschnitten auf ein quadratisches Seitenverhältnis</span><span class="sxs-lookup"><span data-stu-id="547f1-179">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="547f1-180">176 longest</span><span class="sxs-lookup"><span data-stu-id="547f1-180">176 longest</span></span> | <span data-ttu-id="547f1-181">Original</span><span class="sxs-lookup"><span data-stu-id="547f1-181">Original</span></span>     | <span data-ttu-id="547f1-182">Zugeschnitten auf die standardmäßige Elementgröße für die OneDrive-Webansicht</span><span class="sxs-lookup"><span data-stu-id="547f1-182">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="547f1-183">800 longest
</span><span class="sxs-lookup"><span data-stu-id="547f1-183">800 longest</span></span> | <span data-ttu-id="547f1-184">Original</span><span class="sxs-lookup"><span data-stu-id="547f1-184">Original</span></span>     | <span data-ttu-id="547f1-185">Miniaturansicht, bei der die längste Kante auf 800 Pixel skaliert wurde</span><span class="sxs-lookup"><span data-stu-id="547f1-185">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="547f1-186">96x96</span><span class="sxs-lookup"><span data-stu-id="547f1-186">96x96</span></span>       | <span data-ttu-id="547f1-187">Quadratisches Zuschneiden</span><span class="sxs-lookup"><span data-stu-id="547f1-187">Square Crop</span></span>  | <span data-ttu-id="547f1-188">Kleines Quadrat (Miniaturansicht)</span><span class="sxs-lookup"><span data-stu-id="547f1-188">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="547f1-189">176x176</span><span class="sxs-lookup"><span data-stu-id="547f1-189">176x176</span></span>     | <span data-ttu-id="547f1-190">Quadratisches Zuschneiden</span><span class="sxs-lookup"><span data-stu-id="547f1-190">Square Crop</span></span>  | <span data-ttu-id="547f1-191">Kleines Quadrat (Miniaturansicht)</span><span class="sxs-lookup"><span data-stu-id="547f1-191">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="547f1-192">800x800</span><span class="sxs-lookup"><span data-stu-id="547f1-192">800x800</span></span>     | <span data-ttu-id="547f1-193">Quadratisches Zuschneiden</span><span class="sxs-lookup"><span data-stu-id="547f1-193">Square Crop</span></span>  | <span data-ttu-id="547f1-194">Großes Quadrat (Miniaturansicht)</span><span class="sxs-lookup"><span data-stu-id="547f1-194">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="547f1-195">Anfordern von benutzerdefinierten Miniaturansichtgrößen</span><span class="sxs-lookup"><span data-stu-id="547f1-195">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="547f1-196">Zusätzlich zu den definierten Größen kann Ihre App eine benutzerdefinierte Miniaturansichtsgröße anfordern, indem die Dimensionen der Miniaturansicht mit dem Präfix `c` angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="547f1-196">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="547f1-197">Wenn Ihre App zum Beispiel Miniaturansichten mit einer Größe von 300 x 400 benötigt, können Sie diese Größe wie folgt anfordern:</span><span class="sxs-lookup"><span data-stu-id="547f1-197">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>

<!-- { "blockType": "request", "name": "get-thumbnail-custom-size", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```

<span data-ttu-id="547f1-198">Die Antwort ist die benutzerdefinierte Miniaturansichtsgröße:</span><span class="sxs-lookup"><span data-stu-id="547f1-198">Which responds with just the custom thumbnail size selected:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "0",
      "c300x400_Crop": { "height": 300, "width": 400, "url": "https://sn3302files.onedrive.com/123"},
    }
  ]
}
```

<span data-ttu-id="547f1-199">Sie können die folgenden Optionen nach der Größe der angeforderten Miniaturansicht angeben:</span><span class="sxs-lookup"><span data-stu-id="547f1-199">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="547f1-200">Beispiele für benutzerdefinierte Bezeichner</span><span class="sxs-lookup"><span data-stu-id="547f1-200">Examples of custom identifiers</span></span>

| <span data-ttu-id="547f1-201">Miniaturansicht-ID</span><span class="sxs-lookup"><span data-stu-id="547f1-201">Thumbnail identifier</span></span> | <span data-ttu-id="547f1-202">Auflösung</span><span class="sxs-lookup"><span data-stu-id="547f1-202">Resolution</span></span>             | <span data-ttu-id="547f1-203">Seitenverhältnis</span><span class="sxs-lookup"><span data-stu-id="547f1-203">Aspect ratio</span></span> | <span data-ttu-id="547f1-204">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="547f1-204">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="547f1-205">c300x400</span><span class="sxs-lookup"><span data-stu-id="547f1-205">c300x400</span></span>             | <span data-ttu-id="547f1-206">Begrenzt durch 300 x 400-Feld</span><span class="sxs-lookup"><span data-stu-id="547f1-206">Bounded by 300x400 box</span></span> | <span data-ttu-id="547f1-207">Original</span><span class="sxs-lookup"><span data-stu-id="547f1-207">Original</span></span>     | <span data-ttu-id="547f1-208">Generiert eine Miniaturansicht, die in ein Feld von 300 x 400 Pixel passt; dabei wird das Seitenverhältnis beibehalten</span><span class="sxs-lookup"><span data-stu-id="547f1-208">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="547f1-209">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="547f1-209">c300x400_Crop</span></span>        | <span data-ttu-id="547f1-210">300x400</span><span class="sxs-lookup"><span data-stu-id="547f1-210">300x400</span></span>                | <span data-ttu-id="547f1-211">Zugeschnitten</span><span class="sxs-lookup"><span data-stu-id="547f1-211">Cropped</span></span>      | <span data-ttu-id="547f1-212">Erstellt eine Miniaturansicht mit 300 x 400 Pixel.</span><span class="sxs-lookup"><span data-stu-id="547f1-212">Generate a thumbnail that is 300x400 pixels.</span></span> <span data-ttu-id="547f1-213">Dies funktioniert, indem Sie die Größe des Bilds so ändern, dass das Feld von 300 x 400 Pixel gefüllt wird, und alles zuschneiden, was über dieses Feld hinausgeht.</span><span class="sxs-lookup"><span data-stu-id="547f1-213">This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="547f1-214">**Hinweis:** Die zurückgegebenen Miniaturansicht stimmt möglicherweise nicht exakt mit den angeforderten Pixel-Abmessungen überein, , das Seitenverhältnis stimmt jedoch.</span><span class="sxs-lookup"><span data-stu-id="547f1-214">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="547f1-215">In einigen Fällen wird möglicherweise eine größere Miniaturansicht zurückgegeben als angefordert wurde, wenn die Miniaturansicht bereits vorhanden ist und einfach skaliert werden kann, damit sie der angeforderten Auflösung entspricht.</span><span class="sxs-lookup"><span data-stu-id="547f1-215">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="547f1-216">Hinweise</span><span class="sxs-lookup"><span data-stu-id="547f1-216">Remarks</span></span>

<span data-ttu-id="547f1-217">**Hinweis:** Für OneDrive for Business und SharePoint gilt:</span><span class="sxs-lookup"><span data-stu-id="547f1-217">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="547f1-218">Die folgenden Aufrufe können nicht zur Erweiterung der Miniaturansichtsammlung verwendet werden:</span><span class="sxs-lookup"><span data-stu-id="547f1-218">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="547f1-219">Miniaturansichten werden unter SharePoint Server 2016 nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="547f1-219">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="547f1-220">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="547f1-220">Error responses</span></span>

<span data-ttu-id="547f1-221">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="547f1-221">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/driveitem-list-thumbnails.md:
      Unable to map some markdown elements into schema.
         Unmapped methods:
      enum-item-thumbnails, get-one-thumbnail, get-thumbnail-content, get-thumbnail-while-listing, get-thumbnail-custom-size
         Unmapped tables:
      Permissions - AuthScopes, Path parameters - PathParameters, Size options - Unknown, Examples of custom identifiers - Unknown",
    "Warning: Couldn't serialize request for path /me/drive/items/{var}/thumbnails/{var}/{var}/content into EDMX: System.InvalidOperationException: Uri path requires navigating into unknown object hierarchy: missing property '{var}' on 'thumbnailSet'. Possible issues:
         1) Doc bug where '{var}' isn't defined on the resource.         2) Doc bug where '{var}' is an example key and should instead be replaced with a placeholder like {item-id} or declared in the sampleKeys annotation.       3) Doc bug where 'thumbnailSet' is supposed to be an entity type, but is being treated as a complex because it (and its ancestors) are missing the keyProperty annotation
     at ApiDocs.Publishing.CSDL.CsdlWriter.ParseRequestTargetType(String requestPath, MethodCollection requestMethodCollection, EntityFramework edmx, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 1145
     at ApiDocs.Publishing.CSDL.CsdlWriter.ProcessRestRequestPaths(EntityFramework edmx, String[] baseUrlsToRemove, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 821"
  ],
  "tocPath": "Items/Thumbnails"
} -->