# <a name="chart-image"></a><span data-ttu-id="4a94e-101">Diagramm: Bild</span><span class="sxs-lookup"><span data-stu-id="4a94e-101">Chart: Image</span></span>

<span data-ttu-id="4a94e-102">Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.</span><span class="sxs-lookup"><span data-stu-id="4a94e-102">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a94e-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4a94e-103">Permissions</span></span>
<span data-ttu-id="4a94e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a94e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4a94e-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a94e-106">Permission type</span></span>      | <span data-ttu-id="4a94e-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a94e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a94e-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a94e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4a94e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a94e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4a94e-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a94e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a94e-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a94e-111">Not supported.</span></span>    |
|<span data-ttu-id="4a94e-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a94e-112">Application</span></span> | <span data-ttu-id="4a94e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a94e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a94e-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a94e-114">HTTP request</span></span>
<!-- { "blockType": "samples" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/image
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```
## <a name="request-headers"></a><span data-ttu-id="4a94e-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a94e-115">Request headers</span></span>
| <span data-ttu-id="4a94e-116">Name</span><span class="sxs-lookup"><span data-stu-id="4a94e-116">Name</span></span>       | <span data-ttu-id="4a94e-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a94e-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4a94e-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4a94e-118">Authorization</span></span>  | <span data-ttu-id="4a94e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4a94e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a94e-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="4a94e-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="4a94e-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="4a94e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="4a94e-124">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="4a94e-124">Path parameters</span></span>
<span data-ttu-id="4a94e-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="4a94e-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4a94e-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="4a94e-126">Parameter</span></span>    | <span data-ttu-id="4a94e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4a94e-127">Type</span></span>   |<span data-ttu-id="4a94e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a94e-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a94e-129">Höhe</span><span class="sxs-lookup"><span data-stu-id="4a94e-129">height</span></span>|<span data-ttu-id="4a94e-130">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94e-130">Int32</span></span>|<span data-ttu-id="4a94e-131">Die gewünschte Höhe des resultierenden Bilds.</span><span class="sxs-lookup"><span data-stu-id="4a94e-131">Optional. The desired height of the resulting image.</span></span> <span data-ttu-id="4a94e-132">Optional.</span><span class="sxs-lookup"><span data-stu-id="4a94e-132">Optional.</span></span>|
|<span data-ttu-id="4a94e-133">Breite</span><span class="sxs-lookup"><span data-stu-id="4a94e-133">width</span></span>|<span data-ttu-id="4a94e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94e-134">Int32</span></span>|<span data-ttu-id="4a94e-135">Die gewünschte Breite des resultierenden Bilds.</span><span class="sxs-lookup"><span data-stu-id="4a94e-135">Optional. The desired width of the resulting image.</span></span> <span data-ttu-id="4a94e-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="4a94e-136">Optional.</span></span>|
|<span data-ttu-id="4a94e-137">fittingMode</span><span class="sxs-lookup"><span data-stu-id="4a94e-137">fittingMode</span></span>|<span data-ttu-id="4a94e-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a94e-138">string</span></span>|<span data-ttu-id="4a94e-139">Das angewandte Verfahren für die Skalierung des Diagramms auf die Dimensionen skalieren (wenn Höhe und Breite festgelegt werden)."</span><span class="sxs-lookup"><span data-stu-id="4a94e-139">Optional. The method used to scale the chart to the specified dimensions (if both height and width are set)."  Possible values are: , , .</span></span>  <span data-ttu-id="4a94e-140">Mögliche Werte sind: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="4a94e-140">The possible values are `Fit`, `FitAndCenter`, `Fill`, , , , , , , , , or .</span></span>|

## <a name="response"></a><span data-ttu-id="4a94e-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a94e-141">Response</span></span>

<span data-ttu-id="4a94e-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine base64-Bildzeichenfolge im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a94e-142">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a94e-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a94e-143">Example</span></span>
<span data-ttu-id="4a94e-144">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4a94e-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4a94e-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a94e-145">Request</span></span>
<span data-ttu-id="4a94e-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a94e-146">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="4a94e-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a94e-147">Response</span></span>
<span data-ttu-id="4a94e-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4a94e-148">Here is an example of the response.</span></span> <span data-ttu-id="4a94e-149">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="4a94e-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4a94e-150">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a94e-150">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "response", "@odata.type": "Edm.String" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="4a94e-151">Verwendung</span><span class="sxs-lookup"><span data-stu-id="4a94e-151">Usage</span></span>

<span data-ttu-id="4a94e-152">Sie können die Base64-Zeichenfolge innerhalb eines HTML-Bild-Tags anzeigen: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="4a94e-152">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="4a94e-153">Verwenden Sie für das Standardverhalten `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="4a94e-153">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="4a94e-154">Hier ist ein Beispiel für ein Diagrammbild, das mit den standardmäßigen Parametern zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="4a94e-154">Here is an example of a chart image returned with the default parameters.</span></span>

![Excel-Diagrammbild mit Standardhöhe und -breite.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="4a94e-156">Wenn Sie die Anzeige des Bilds anpassen möchten, geben Sie eine Höhe, Breite und einen Anpassmodus an.</span><span class="sxs-lookup"><span data-stu-id="4a94e-156">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="4a94e-157">So sieht dasselbe Diagrammbild aus, wenn Sie es mit diesen Parametern abrufen: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="4a94e-157">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

![Excel-Diagrammbild mit Standardhöhe und -breite.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
