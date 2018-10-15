# <a name="update-chartdatalabels"></a><span data-ttu-id="989f2-101">ChartDataLabels aktualisieren</span><span class="sxs-lookup"><span data-stu-id="989f2-101">Update chartdatalabels</span></span>

<span data-ttu-id="989f2-102">Dient zum Aktualisieren der Eigenschaften des ChartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="989f2-102">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="989f2-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="989f2-103">Permissions</span></span>
<span data-ttu-id="989f2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="989f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="989f2-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="989f2-106">Permission type</span></span>      | <span data-ttu-id="989f2-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="989f2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="989f2-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="989f2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="989f2-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="989f2-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="989f2-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="989f2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="989f2-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="989f2-111">Not supported.</span></span>    |
|<span data-ttu-id="989f2-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="989f2-112">Application</span></span> | <span data-ttu-id="989f2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="989f2-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="989f2-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="989f2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="989f2-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="989f2-115">Optional request headers</span></span>
| <span data-ttu-id="989f2-116">Name</span><span class="sxs-lookup"><span data-stu-id="989f2-116">Name</span></span>       | <span data-ttu-id="989f2-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="989f2-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="989f2-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="989f2-118">Authorization</span></span>  | <span data-ttu-id="989f2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="989f2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="989f2-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="989f2-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="989f2-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="989f2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="989f2-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="989f2-124">Request body</span></span>
<span data-ttu-id="989f2-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="989f2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="989f2-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="989f2-128">Property</span></span>     | <span data-ttu-id="989f2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="989f2-129">Type</span></span>   |<span data-ttu-id="989f2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="989f2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="989f2-131">Position</span><span class="sxs-lookup"><span data-stu-id="989f2-131">position</span></span>|<span data-ttu-id="989f2-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="989f2-132">string</span></span>|<span data-ttu-id="989f2-133">DataLabelPosition-Wert, der die Position der Datenbeschriftung darstellt.</span><span class="sxs-lookup"><span data-stu-id="989f2-133">DataLabelPosition value that represents the position of the data label. Possible values are: , , , , , , , , , , .</span></span> <span data-ttu-id="989f2-134">Die möglichen Werte sind: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="989f2-134">The possible values are `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`, or .</span></span>|
|<span data-ttu-id="989f2-135">Separator</span><span class="sxs-lookup"><span data-stu-id="989f2-135">separator</span></span>|<span data-ttu-id="989f2-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="989f2-136">string</span></span>|<span data-ttu-id="989f2-137">Zeichenfolge, die das Trennzeichen für die Datenbeschriftungen in einem Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="989f2-137">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="989f2-138">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="989f2-138">showBubbleSize</span></span>|<span data-ttu-id="989f2-139">boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="989f2-139">boolean</span></span>|<span data-ttu-id="989f2-140">Boolescher Wert, der angibt, ob die Größe der Datenbeschriftungs-Sprechblase angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="989f2-140">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="989f2-141">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="989f2-141">showCategoryName</span></span>|<span data-ttu-id="989f2-142">boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="989f2-142">boolean</span></span>|<span data-ttu-id="989f2-143">Boolescher Wert, der angibt, ob der Kategoriename der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="989f2-143">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="989f2-144">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="989f2-144">showLegendKey</span></span>|<span data-ttu-id="989f2-145">boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="989f2-145">boolean</span></span>|<span data-ttu-id="989f2-146">Boolescher Wert, der angibt, ob das Legendensymbol der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="989f2-146">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="989f2-147">showPercentage</span><span class="sxs-lookup"><span data-stu-id="989f2-147">showPercentage</span></span>|<span data-ttu-id="989f2-148">boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="989f2-148">boolean</span></span>|<span data-ttu-id="989f2-149">Boolescher Wert, der angibt, ob der Prozentsatz der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="989f2-149">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="989f2-150">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="989f2-150">showSeriesName</span></span>|<span data-ttu-id="989f2-151">boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="989f2-151">boolean</span></span>|<span data-ttu-id="989f2-152">Boolescher Wert, der angibt, ob der Name der Datenbeschriftungsreihe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="989f2-152">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="989f2-153">showValue</span><span class="sxs-lookup"><span data-stu-id="989f2-153">showValue</span></span>|<span data-ttu-id="989f2-154">boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="989f2-154">boolean</span></span>|<span data-ttu-id="989f2-155">Boolescher Wert, der angibt, ob der Datenbeschriftungswert angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="989f2-155">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="989f2-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="989f2-156">Response</span></span>

<span data-ttu-id="989f2-157">Wenn die Methode erfolgreich verläuft, werden im Antworttext der Antwortcode `200 OK` und ein [WorkbookChartDataLabels](../resources/chartdatalabels.md)-Objekt zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="989f2-157">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="989f2-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="989f2-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="989f2-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="989f2-159">Request</span></span>
<span data-ttu-id="989f2-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="989f2-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```
##### <a name="response"></a><span data-ttu-id="989f2-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="989f2-161">Response</span></span>
<span data-ttu-id="989f2-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="989f2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->