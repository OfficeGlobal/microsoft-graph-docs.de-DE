---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Abrufen von Miniaturansichten für eine Datei oder einen Ordner
localization_priority: Normal
ms.openlocfilehash: 48ea0b1f876fff28affc68895aed58a063df1513
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813713"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="9535e-102">Miniaturansichten für ein DriveItem auflisten</span><span class="sxs-lookup"><span data-stu-id="9535e-102">List thumbnails for a DriveItem</span></span>

> <span data-ttu-id="9535e-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9535e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9535e-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9535e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9535e-105">Hier erklären wir Ihnen, wie Sie eine Liste der [ThumbnailSet](../resources/thumbnailset.md)-Ressourcen einer [DriveItem](../resources/driveitem.md)-Ressource abrufen können.</span><span class="sxs-lookup"><span data-stu-id="9535e-105">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="9535e-p102">Ein DriveItem kann durch 0 oder mehr [ThumbnailSet](../resources/thumbnailset.md)-Ressourcen repräsentiert werden. Jedes **thumbnailSet** kann ein oder mehrere [**thumbnail**](../resources/thumbnail.md)-Objekte haben. Dabei handelt es sich um Bilder, die das jeweilige Element darstellen. Beispielsweise könnte ein **thumbnailSet** gängige **thumbnail**-Objekte wie `small`, `medium` oder `large` enthalten.</span><span class="sxs-lookup"><span data-stu-id="9535e-p102">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="9535e-p103">Es gibt viele Möglichkeiten, auf OneDrive mit Miniaturansichten zu arbeiten. Die häufigsten:</span><span class="sxs-lookup"><span data-stu-id="9535e-p103">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="9535e-111">Enumerieren der für ein Element verfügbaren Miniaturansichten</span><span class="sxs-lookup"><span data-stu-id="9535e-111">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="9535e-112">Abrufen einer einzelnen Miniaturansicht für ein Element</span><span class="sxs-lookup"><span data-stu-id="9535e-112">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="9535e-113">Abrufen von Miniaturansichtinhalten</span><span class="sxs-lookup"><span data-stu-id="9535e-113">Retrieve thumbnail content</span></span>
* <span data-ttu-id="9535e-114">Abrufen von Miniaturansichten für mehrere Elemente in einer einzigen Anforderung</span><span class="sxs-lookup"><span data-stu-id="9535e-114">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="9535e-115">Abrufen von benutzerdefinierten Miniaturansichtgrößen</span><span class="sxs-lookup"><span data-stu-id="9535e-115">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="9535e-116">Hochladen einer benutzerdefinierten Miniaturansicht für ein Element</span><span class="sxs-lookup"><span data-stu-id="9535e-116">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="9535e-117">Ermitteln, ob eine benutzerdefinierte Miniaturansicht hochgeladen wurde</span><span class="sxs-lookup"><span data-stu-id="9535e-117">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="9535e-118">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9535e-118">Permissions</span></span>

<span data-ttu-id="9535e-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9535e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9535e-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9535e-121">Permission type</span></span>      | <span data-ttu-id="9535e-122">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9535e-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9535e-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9535e-123">Delegated (work or school account)</span></span> | <span data-ttu-id="9535e-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9535e-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9535e-125">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9535e-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9535e-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9535e-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="9535e-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9535e-127">Application</span></span> | <span data-ttu-id="9535e-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9535e-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9535e-129">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9535e-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9535e-130">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9535e-130">Optional query parameters</span></span>

<span data-ttu-id="9535e-131">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von `$select` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9535e-131">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="9535e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9535e-132">Response</span></span>

<span data-ttu-id="9535e-133">Bei Erfolg gibt diese Methode einen Antwortcode des Typs `200 OK` und eine Sammlung von [ThumbnailSet](../resources/thumbnailset.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9535e-133">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9535e-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9535e-134">Example</span></span>

<span data-ttu-id="9535e-135">Hier ist ein Beispiel für die Anforderung, die verfügbare Miniaturansichten für ein Element im OneDrive des aktuellen Benutzers abruft.</span><span class="sxs-lookup"><span data-stu-id="9535e-135">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```

<span data-ttu-id="9535e-136">Diese gibt ein Array von verfügbaren **thumbnailSets** für das Element zurück.</span><span class="sxs-lookup"><span data-stu-id="9535e-136">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="9535e-137">Ein beliebiges Element auf einem Laufwerk kann Null oder mehr Miniaturansichten aufweisen.</span><span class="sxs-lookup"><span data-stu-id="9535e-137">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="9535e-138">**Hinweis:** Sie können den _select_-Abfragezeichenfolgenparameter verwenden, um zu steuern, welche Miniaturansichtgrößen im **ThumbnailSet** zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="9535e-138">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**.</span></span>
<span data-ttu-id="9535e-139">`/thumbnails?select=medium` ruft beispielsweise nur die mittelgroßen Miniaturansichten ab.</span><span class="sxs-lookup"><span data-stu-id="9535e-139">For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="9535e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="9535e-140">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="9535e-141">Abrufen einer einzelnen Miniaturansicht</span><span class="sxs-lookup"><span data-stu-id="9535e-141">Get a single thumbnail</span></span>

<span data-ttu-id="9535e-142">Sie können die Metadaten einer einzelnen Miniaturansicht sowie ihre Größe abrufen, indem Sie sie in einer Anforderung direkt adressieren.</span><span class="sxs-lookup"><span data-stu-id="9535e-142">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="9535e-143">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9535e-143">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

### <a name="path-parameters"></a><span data-ttu-id="9535e-144">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="9535e-144">Path parameters</span></span>

| <span data-ttu-id="9535e-145">Name</span><span class="sxs-lookup"><span data-stu-id="9535e-145">Name</span></span>         | <span data-ttu-id="9535e-146">Typ</span><span class="sxs-lookup"><span data-stu-id="9535e-146">Type</span></span>   | <span data-ttu-id="9535e-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9535e-147">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="9535e-148">**item-id**</span><span class="sxs-lookup"><span data-stu-id="9535e-148">**item-id**</span></span>  | <span data-ttu-id="9535e-149">string</span><span class="sxs-lookup"><span data-stu-id="9535e-149">string</span></span> | <span data-ttu-id="9535e-150">Der eindeutige Bezeichner für das referenzierte Element</span><span class="sxs-lookup"><span data-stu-id="9535e-150">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="9535e-151">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="9535e-151">**thumb-id**</span></span> | <span data-ttu-id="9535e-152">number</span><span class="sxs-lookup"><span data-stu-id="9535e-152">number</span></span> | <span data-ttu-id="9535e-153">Der Index der Miniaturansicht, in der Regel 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="9535e-153">The index of the thumbnail, usually 0-4.</span></span> <span data-ttu-id="9535e-154">Wenn es eine benutzerdefinierte Miniaturansicht gibt, ist ihr Index 0.</span><span class="sxs-lookup"><span data-stu-id="9535e-154">If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="9535e-155">**size**</span><span class="sxs-lookup"><span data-stu-id="9535e-155">**size**</span></span>     | <span data-ttu-id="9535e-156">string</span><span class="sxs-lookup"><span data-stu-id="9535e-156">string</span></span> | <span data-ttu-id="9535e-157">Die Größe der angeforderten Miniaturansicht.</span><span class="sxs-lookup"><span data-stu-id="9535e-157">The size of the thumbnail requested.</span></span> <span data-ttu-id="9535e-158">Dabei kann es sich um eine der nachfolgend aufgeführten Standardgrößen oder um eine benutzerdefinierte Größe handeln.</span><span class="sxs-lookup"><span data-stu-id="9535e-158">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="9535e-159">Abrufen von binären Miniaturansichtinhalten</span><span class="sxs-lookup"><span data-stu-id="9535e-159">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="9535e-160">Sie können den Inhalt einer Miniaturansicht direkt abrufen, indem Sie die Eigenschaft **content** der Miniaturansicht anfordern.</span><span class="sxs-lookup"><span data-stu-id="9535e-160">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="9535e-161">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9535e-161">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

### <a name="response"></a><span data-ttu-id="9535e-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="9535e-162">Response</span></span>

<span data-ttu-id="9535e-163">Der Dienst antwortet mit einer Umleitung auf die Miniaturansicht-URL.</span><span class="sxs-lookup"><span data-stu-id="9535e-163">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="9535e-164">Miniaturansicht-URLs sind cachesicher.</span><span class="sxs-lookup"><span data-stu-id="9535e-164">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="9535e-165">Die URL ändert sich, wenn sich das Element derart ändert, dass eine neue Miniaturansicht generiert werden muss.</span><span class="sxs-lookup"><span data-stu-id="9535e-165">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="9535e-166">Abrufen von Miniaturansichten beim Auflisten von DriveItems</span><span class="sxs-lookup"><span data-stu-id="9535e-166">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="9535e-167">Wenn Sie eine Liste der anzuzeigenden DriveItem-Ressourcen abrufen, können Sie mit dem _$expand_-Abfragezeichenfolge-Parameter außerdem die Miniaturansichten für diese Ressourcen aufnehmen.</span><span class="sxs-lookup"><span data-stu-id="9535e-167">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="9535e-168">Dadurch kann Ihre App Miniaturansichten und Elemente in einer einzelnen Anforderung abrufen, statt viele Anforderungen auszuführen.</span><span class="sxs-lookup"><span data-stu-id="9535e-168">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="9535e-169">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9535e-169">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```

### <a name="response"></a><span data-ttu-id="9535e-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="9535e-170">Response</span></span>

<span data-ttu-id="9535e-171">Die Dienstantworten mit der Liste der DriveItems und ihren Miniaturansichten.</span><span class="sxs-lookup"><span data-stu-id="9535e-171">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-values"></a><span data-ttu-id="9535e-172">Größenwerte</span><span class="sxs-lookup"><span data-stu-id="9535e-172">Size values</span></span>

<span data-ttu-id="9535e-p111">In dieser Tabelle sind die möglichen Miniaturansichtgrößen definiert. Zwar können Sie jede beliebige Miniaturansichtgröße anfordern; bei den definierten Werten ist es jedoch wahrscheinlich, dass sie existieren und dass schnell ein Wert zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="9535e-p111">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="9535e-175">Name</span><span class="sxs-lookup"><span data-stu-id="9535e-175">Name</span></span>           | <span data-ttu-id="9535e-176">Auflösung</span><span class="sxs-lookup"><span data-stu-id="9535e-176">Resolution</span></span>  | <span data-ttu-id="9535e-177">Seitenverhältnis</span><span class="sxs-lookup"><span data-stu-id="9535e-177">Aspect Ratio</span></span> | <span data-ttu-id="9535e-178">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9535e-178">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="9535e-179">96 longest
</span><span class="sxs-lookup"><span data-stu-id="9535e-179">96 longest</span></span>  | <span data-ttu-id="9535e-180">Original</span><span class="sxs-lookup"><span data-stu-id="9535e-180">Original</span></span>     | <span data-ttu-id="9535e-181">Kleine, stark komprimierte Miniaturansicht, zugeschnitten auf ein quadratisches Seitenverhältnis</span><span class="sxs-lookup"><span data-stu-id="9535e-181">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="9535e-182">176 longest</span><span class="sxs-lookup"><span data-stu-id="9535e-182">176 longest</span></span> | <span data-ttu-id="9535e-183">Original</span><span class="sxs-lookup"><span data-stu-id="9535e-183">Original</span></span>     | <span data-ttu-id="9535e-184">Zugeschnitten auf die standardmäßige Elementgröße für die OneDrive-Webansicht</span><span class="sxs-lookup"><span data-stu-id="9535e-184">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="9535e-185">800 longest
</span><span class="sxs-lookup"><span data-stu-id="9535e-185">800 longest</span></span> | <span data-ttu-id="9535e-186">Original</span><span class="sxs-lookup"><span data-stu-id="9535e-186">Original</span></span>     | <span data-ttu-id="9535e-187">Miniaturansicht, bei der die längste Kante auf 800 Pixel skaliert wurde</span><span class="sxs-lookup"><span data-stu-id="9535e-187">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="9535e-188">96x96</span><span class="sxs-lookup"><span data-stu-id="9535e-188">96x96</span></span>       | <span data-ttu-id="9535e-189">Quadratisches Zuschneiden</span><span class="sxs-lookup"><span data-stu-id="9535e-189">Square Crop</span></span>  | <span data-ttu-id="9535e-190">Kleines Quadrat (Miniaturansicht)</span><span class="sxs-lookup"><span data-stu-id="9535e-190">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="9535e-191">176x176</span><span class="sxs-lookup"><span data-stu-id="9535e-191">176x176</span></span>     | <span data-ttu-id="9535e-192">Quadratisches Zuschneiden</span><span class="sxs-lookup"><span data-stu-id="9535e-192">Square Crop</span></span>  | <span data-ttu-id="9535e-193">Kleines Quadrat (Miniaturansicht)</span><span class="sxs-lookup"><span data-stu-id="9535e-193">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="9535e-194">800x800</span><span class="sxs-lookup"><span data-stu-id="9535e-194">800x800</span></span>     | <span data-ttu-id="9535e-195">Quadratisches Zuschneiden</span><span class="sxs-lookup"><span data-stu-id="9535e-195">Square Crop</span></span>  | <span data-ttu-id="9535e-196">Großes Quadrat (Miniaturansicht)</span><span class="sxs-lookup"><span data-stu-id="9535e-196">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="9535e-197">Anfordern von benutzerdefinierten Miniaturansichtgrößen</span><span class="sxs-lookup"><span data-stu-id="9535e-197">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="9535e-198">Zusätzlich zu den definierten Größen kann Ihre App eine benutzerdefinierte Miniaturansichtsgröße anfordern, indem die Dimensionen der Miniaturansicht mit dem Präfix `c` angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="9535e-198">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="9535e-199">Wenn Ihre App zum Beispiel Miniaturansichten mit einer Größe von 300 x 400 benötigt, können Sie diese Größe wie folgt anfordern:</span><span class="sxs-lookup"><span data-stu-id="9535e-199">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>

<!-- { "name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```

<span data-ttu-id="9535e-200">Die Antwort ist die benutzerdefinierte Miniaturansichtsgröße:</span><span class="sxs-lookup"><span data-stu-id="9535e-200">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="9535e-201">Sie können die folgenden Optionen nach der Größe der angeforderten Miniaturansicht angeben:</span><span class="sxs-lookup"><span data-stu-id="9535e-201">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="9535e-202">Beispiele für benutzerdefinierte Bezeichner</span><span class="sxs-lookup"><span data-stu-id="9535e-202">Examples of custom identifiers</span></span>

| <span data-ttu-id="9535e-203">Miniaturansicht-ID</span><span class="sxs-lookup"><span data-stu-id="9535e-203">Thumbnail identifier</span></span> | <span data-ttu-id="9535e-204">Auflösung</span><span class="sxs-lookup"><span data-stu-id="9535e-204">Resolution</span></span>             | <span data-ttu-id="9535e-205">Seitenverhältnis</span><span class="sxs-lookup"><span data-stu-id="9535e-205">Aspect ratio</span></span> | <span data-ttu-id="9535e-206">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9535e-206">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9535e-207">c300x400</span><span class="sxs-lookup"><span data-stu-id="9535e-207">c300x400</span></span>             | <span data-ttu-id="9535e-208">Begrenzt durch 300 x 400-Feld</span><span class="sxs-lookup"><span data-stu-id="9535e-208">Bounded by 300x400 box</span></span> | <span data-ttu-id="9535e-209">Original</span><span class="sxs-lookup"><span data-stu-id="9535e-209">Original</span></span>     | <span data-ttu-id="9535e-210">Generiert eine Miniaturansicht, die in ein Feld von 300 x 400 Pixel passt; dabei wird das Seitenverhältnis beibehalten</span><span class="sxs-lookup"><span data-stu-id="9535e-210">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="9535e-211">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="9535e-211">c300x400_Crop</span></span>        | <span data-ttu-id="9535e-212">300x400</span><span class="sxs-lookup"><span data-stu-id="9535e-212">300x400</span></span>                | <span data-ttu-id="9535e-213">Zugeschnitten</span><span class="sxs-lookup"><span data-stu-id="9535e-213">Cropped</span></span>      | <span data-ttu-id="9535e-214">Erstellt eine Miniaturansicht mit 300 x 400 Pixel.</span><span class="sxs-lookup"><span data-stu-id="9535e-214">Generate a thumbnail that is 300x400 pixels.</span></span> <span data-ttu-id="9535e-215">Dies funktioniert, indem Sie die Größe des Bilds so ändern, dass das Feld von 300 x 400 Pixel gefüllt wird, und alles zuschneiden, was über dieses Feld hinausgeht.</span><span class="sxs-lookup"><span data-stu-id="9535e-215">This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="9535e-216">**Hinweis:** Die zurückgegebenen Miniaturansicht stimmt möglicherweise nicht exakt mit den angeforderten Pixel-Abmessungen überein, , das Seitenverhältnis stimmt jedoch.</span><span class="sxs-lookup"><span data-stu-id="9535e-216">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="9535e-217">In einigen Fällen wird möglicherweise eine größere Miniaturansicht zurückgegeben als angefordert wurde, wenn die Miniaturansicht bereits vorhanden ist und einfach skaliert werden kann, damit sie der angeforderten Auflösung entspricht.</span><span class="sxs-lookup"><span data-stu-id="9535e-217">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="9535e-218">Hinweise</span><span class="sxs-lookup"><span data-stu-id="9535e-218">Remarks</span></span>

<span data-ttu-id="9535e-219">**Hinweis:** Für OneDrive for Business und SharePoint gilt:</span><span class="sxs-lookup"><span data-stu-id="9535e-219">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="9535e-220">Die folgenden Aufrufe können nicht zur Erweiterung der Miniaturansichtsammlung verwendet werden:</span><span class="sxs-lookup"><span data-stu-id="9535e-220">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="9535e-221">Miniaturansichten werden unter SharePoint Server 2016 nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9535e-221">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="9535e-222">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="9535e-222">Error responses</span></span>

<span data-ttu-id="9535e-223">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="9535e-223">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "Items/Thumbnails"
} -->
