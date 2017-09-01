# <a name="update-chartdatalabels"></a><span data-ttu-id="e3239-101">ChartDataLabels aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e3239-101">Update chartdatalabels</span></span>

<span data-ttu-id="e3239-102">Dient zum Aktualisieren der Eigenschaften des ChartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e3239-102">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e3239-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e3239-103">Permissions</span></span>
<span data-ttu-id="e3239-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3239-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e3239-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3239-106">Permission type</span></span>      | <span data-ttu-id="e3239-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3239-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3239-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3239-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e3239-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3239-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e3239-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3239-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3239-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3239-111">Not supported.</span></span>    |
|<span data-ttu-id="e3239-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3239-112">Application</span></span> | <span data-ttu-id="e3239-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3239-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3239-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3239-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="e3239-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3239-115">Optional request headers</span></span>
| <span data-ttu-id="e3239-116">Name</span><span class="sxs-lookup"><span data-stu-id="e3239-116">Name</span></span>       | <span data-ttu-id="e3239-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3239-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e3239-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3239-118">Authorization</span></span>  | <span data-ttu-id="e3239-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e3239-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3239-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3239-121">Request body</span></span>
<span data-ttu-id="e3239-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="e3239-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e3239-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3239-125">Property</span></span>     | <span data-ttu-id="e3239-126">Typ</span><span class="sxs-lookup"><span data-stu-id="e3239-126">Type</span></span>   |<span data-ttu-id="e3239-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3239-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3239-128">Position</span><span class="sxs-lookup"><span data-stu-id="e3239-128">position</span></span>|<span data-ttu-id="e3239-129">string</span><span class="sxs-lookup"><span data-stu-id="e3239-129">string</span></span>|<span data-ttu-id="e3239-p104">DataLabelPosition-Wert, der die Position der Datenbeschriftung darstellt. Mögliche Werte: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="e3239-p104">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="e3239-132">Separator</span><span class="sxs-lookup"><span data-stu-id="e3239-132">separator</span></span>|<span data-ttu-id="e3239-133">string</span><span class="sxs-lookup"><span data-stu-id="e3239-133">string</span></span>|<span data-ttu-id="e3239-134">Zeichenfolge, die das Trennzeichen für die Datenbeschriftungen in einem Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="e3239-134">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="e3239-135">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="e3239-135">showBubbleSize</span></span>|<span data-ttu-id="e3239-136">boolean</span><span class="sxs-lookup"><span data-stu-id="e3239-136">boolean</span></span>|<span data-ttu-id="e3239-137">Boolescher Wert, der angibt, ob die Größe der Datenbeschriftungs-Sprechblase angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e3239-137">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="e3239-138">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="e3239-138">showCategoryName</span></span>|<span data-ttu-id="e3239-139">boolean</span><span class="sxs-lookup"><span data-stu-id="e3239-139">boolean</span></span>|<span data-ttu-id="e3239-140">Boolescher Wert, der angibt, ob der Kategoriename der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e3239-140">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="e3239-141">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="e3239-141">showLegendKey</span></span>|<span data-ttu-id="e3239-142">boolean</span><span class="sxs-lookup"><span data-stu-id="e3239-142">boolean</span></span>|<span data-ttu-id="e3239-143">Boolescher Wert, der angibt, ob das Legendensymbol der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e3239-143">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="e3239-144">showPercentage</span><span class="sxs-lookup"><span data-stu-id="e3239-144">showPercentage</span></span>|<span data-ttu-id="e3239-145">boolean</span><span class="sxs-lookup"><span data-stu-id="e3239-145">boolean</span></span>|<span data-ttu-id="e3239-146">Boolescher Wert, der angibt, ob der Prozentsatz der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e3239-146">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="e3239-147">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="e3239-147">showSeriesName</span></span>|<span data-ttu-id="e3239-148">boolean</span><span class="sxs-lookup"><span data-stu-id="e3239-148">boolean</span></span>|<span data-ttu-id="e3239-149">Boolescher Wert, der angibt, ob der Name der Datenbeschriftungsreihe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e3239-149">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="e3239-150">showValue</span><span class="sxs-lookup"><span data-stu-id="e3239-150">showValue</span></span>|<span data-ttu-id="e3239-151">boolean</span><span class="sxs-lookup"><span data-stu-id="e3239-151">boolean</span></span>|<span data-ttu-id="e3239-152">Boolescher Wert, der angibt, ob der Datenbeschriftungswert angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e3239-152">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="e3239-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3239-153">Response</span></span>

<span data-ttu-id="e3239-154">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartDataLabels](../resources/chartdatalabels.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3239-154">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3239-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3239-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3239-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3239-156">Request</span></span>
<span data-ttu-id="e3239-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3239-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/datalabels
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
##### <a name="response"></a><span data-ttu-id="e3239-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3239-158">Response</span></span>
<span data-ttu-id="e3239-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3239-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartDataLabels"
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