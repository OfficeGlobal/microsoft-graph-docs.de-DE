# <a name="chart-image"></a><span data-ttu-id="95f40-101">Diagramm: Bild</span><span class="sxs-lookup"><span data-stu-id="95f40-101">Chart: Image</span></span>

<span data-ttu-id="95f40-102">Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.</span><span class="sxs-lookup"><span data-stu-id="95f40-102">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="95f40-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="95f40-103">Permissions</span></span>
<span data-ttu-id="95f40-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="95f40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="95f40-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="95f40-106">Permission type</span></span>      | <span data-ttu-id="95f40-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="95f40-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95f40-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="95f40-108">Delegated (work or school account)</span></span> | <span data-ttu-id="95f40-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95f40-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="95f40-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="95f40-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95f40-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="95f40-111">Not supported.</span></span>    |
|<span data-ttu-id="95f40-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="95f40-112">Application</span></span> | <span data-ttu-id="95f40-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="95f40-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="95f40-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="95f40-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="95f40-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="95f40-115">Request headers</span></span>
| <span data-ttu-id="95f40-116">Name</span><span class="sxs-lookup"><span data-stu-id="95f40-116">Name</span></span>       | <span data-ttu-id="95f40-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95f40-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="95f40-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="95f40-118">Authorization</span></span>  | <span data-ttu-id="95f40-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="95f40-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="95f40-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="95f40-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="95f40-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="95f40-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="95f40-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="95f40-124">Request body</span></span>
<span data-ttu-id="95f40-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="95f40-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="95f40-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="95f40-126">Parameter</span></span>    | <span data-ttu-id="95f40-127">Typ</span><span class="sxs-lookup"><span data-stu-id="95f40-127">Type</span></span>   |<span data-ttu-id="95f40-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95f40-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95f40-129">height</span><span class="sxs-lookup"><span data-stu-id="95f40-129">height</span></span>|<span data-ttu-id="95f40-130">number</span><span class="sxs-lookup"><span data-stu-id="95f40-130">number</span></span>|<span data-ttu-id="95f40-p104">Optional. Die gewünschte Höhe des resultierenden Bilds.</span><span class="sxs-lookup"><span data-stu-id="95f40-p104">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="95f40-133">width</span><span class="sxs-lookup"><span data-stu-id="95f40-133">width</span></span>|<span data-ttu-id="95f40-134">number</span><span class="sxs-lookup"><span data-stu-id="95f40-134">number</span></span>|<span data-ttu-id="95f40-p105">Optional. Die gewünschte Breite des resultierenden Bilds.</span><span class="sxs-lookup"><span data-stu-id="95f40-p105">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="95f40-137">fittingMode</span><span class="sxs-lookup"><span data-stu-id="95f40-137">fittingMode</span></span>|<span data-ttu-id="95f40-138">string</span><span class="sxs-lookup"><span data-stu-id="95f40-138">string</span></span>|<span data-ttu-id="95f40-p106">Optional. Die Methode, die verwendet wird, um das Diagramm auf die angegebenen Maße zu skalieren (wenn Höhe und Breite festgelegt sind).  Mögliche Werte: `Fit`, `FitAndCenter`, `Fill`.</span><span class="sxs-lookup"><span data-stu-id="95f40-p106">Optional. The method used to scale the chart to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="95f40-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="95f40-142">Response</span></span>

<span data-ttu-id="95f40-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine base64-Bildzeichenfolge im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="95f40-143">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95f40-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="95f40-144">Example</span></span>
<span data-ttu-id="95f40-145">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="95f40-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="95f40-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="95f40-146">Request</span></span>
<span data-ttu-id="95f40-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="95f40-147">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="95f40-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="95f40-148">Response</span></span>
<span data-ttu-id="95f40-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="95f40-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="95f40-152">Verwendung</span><span class="sxs-lookup"><span data-stu-id="95f40-152">Usage</span></span>

<span data-ttu-id="95f40-153">Sie können die Base64-Zeichenfolge innerhalb eines HTML-Bild-Tags anzeigen: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="95f40-153">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="95f40-154">Verwenden Sie für das Standardverhalten `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="95f40-154">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="95f40-155">Hier ist ein Beispiel für ein Diagrammbild, das mit den standardmäßigen Parametern zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="95f40-155">Here is an example of a chart image returned with the default parameters.</span></span>

![Excel-Diagrammbild mit Standardhöhe und -breite.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="95f40-157">Wenn Sie die Anzeige des Bilds anpassen möchten, geben Sie eine Höhe, Breite und einen Anpassmodus an.</span><span class="sxs-lookup"><span data-stu-id="95f40-157">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="95f40-158">So sieht dasselbe Diagrammbild aus, wenn Sie es mit diesen Parametern abrufen: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="95f40-158">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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
