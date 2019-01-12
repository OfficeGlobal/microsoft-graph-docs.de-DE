---
title: ChartDataLabels aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartDataLabels-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 44eb2888a878d71b04017198f3eae7bc8a637097
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932238"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="0e25b-103">ChartDataLabels aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0e25b-103">Update chartdatalabels</span></span>

<span data-ttu-id="0e25b-104">Dient zum Aktualisieren der Eigenschaften des ChartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e25b-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e25b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0e25b-105">Permissions</span></span>
<span data-ttu-id="0e25b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e25b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e25b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e25b-108">Permission type</span></span>      | <span data-ttu-id="0e25b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e25b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e25b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e25b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e25b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e25b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e25b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e25b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e25b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e25b-113">Not supported.</span></span>    |
|<span data-ttu-id="0e25b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e25b-114">Application</span></span> | <span data-ttu-id="0e25b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e25b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e25b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e25b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="0e25b-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e25b-117">Optional request headers</span></span>
| <span data-ttu-id="0e25b-118">Name</span><span class="sxs-lookup"><span data-stu-id="0e25b-118">Name</span></span>       | <span data-ttu-id="0e25b-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e25b-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0e25b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e25b-120">Authorization</span></span>  | <span data-ttu-id="0e25b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0e25b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e25b-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="0e25b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0e25b-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="0e25b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e25b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e25b-126">Request body</span></span>
<span data-ttu-id="0e25b-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="0e25b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0e25b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e25b-130">Property</span></span>     | <span data-ttu-id="0e25b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0e25b-131">Type</span></span>   |<span data-ttu-id="0e25b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e25b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e25b-133">position</span><span class="sxs-lookup"><span data-stu-id="0e25b-133">position</span></span>|<span data-ttu-id="0e25b-134">string</span><span class="sxs-lookup"><span data-stu-id="0e25b-134">string</span></span>|<span data-ttu-id="0e25b-135">DataLabelPosition-Wert, der die Position der Datenbeschriftung darstellt.</span><span class="sxs-lookup"><span data-stu-id="0e25b-135">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="0e25b-136">Die möglichen Werte sind: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="0e25b-136">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="0e25b-137">Separator</span><span class="sxs-lookup"><span data-stu-id="0e25b-137">separator</span></span>|<span data-ttu-id="0e25b-138">string</span><span class="sxs-lookup"><span data-stu-id="0e25b-138">string</span></span>|<span data-ttu-id="0e25b-139">Zeichenfolge, die das Trennzeichen für die Datenbeschriftungen in einem Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="0e25b-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="0e25b-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="0e25b-140">showBubbleSize</span></span>|<span data-ttu-id="0e25b-141">boolean</span><span class="sxs-lookup"><span data-stu-id="0e25b-141">boolean</span></span>|<span data-ttu-id="0e25b-142">Boolescher Wert, der angibt, ob die Größe der Datenbeschriftungs-Sprechblase angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0e25b-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="0e25b-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="0e25b-143">showCategoryName</span></span>|<span data-ttu-id="0e25b-144">boolean</span><span class="sxs-lookup"><span data-stu-id="0e25b-144">boolean</span></span>|<span data-ttu-id="0e25b-145">Boolescher Wert, der angibt, ob der Kategoriename der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0e25b-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="0e25b-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="0e25b-146">showLegendKey</span></span>|<span data-ttu-id="0e25b-147">boolean</span><span class="sxs-lookup"><span data-stu-id="0e25b-147">boolean</span></span>|<span data-ttu-id="0e25b-148">Boolescher Wert, der angibt, ob das Legendensymbol der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0e25b-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="0e25b-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="0e25b-149">showPercentage</span></span>|<span data-ttu-id="0e25b-150">boolean</span><span class="sxs-lookup"><span data-stu-id="0e25b-150">boolean</span></span>|<span data-ttu-id="0e25b-151">Boolescher Wert, der angibt, ob der Prozentsatz der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0e25b-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="0e25b-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="0e25b-152">showSeriesName</span></span>|<span data-ttu-id="0e25b-153">boolean</span><span class="sxs-lookup"><span data-stu-id="0e25b-153">boolean</span></span>|<span data-ttu-id="0e25b-154">Boolescher Wert, der angibt, ob der Name der Datenbeschriftungsreihe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0e25b-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="0e25b-155">showValue</span><span class="sxs-lookup"><span data-stu-id="0e25b-155">showValue</span></span>|<span data-ttu-id="0e25b-156">boolean</span><span class="sxs-lookup"><span data-stu-id="0e25b-156">boolean</span></span>|<span data-ttu-id="0e25b-157">Boolescher Wert, der angibt, ob der Datenbeschriftungswert angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0e25b-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="0e25b-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e25b-158">Response</span></span>

<span data-ttu-id="0e25b-159">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookChartDataLabels](../resources/chartdatalabels.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0e25b-159">If successful, this method returns a `200 OK` response code and updated [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e25b-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e25b-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e25b-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e25b-161">Request</span></span>
<span data-ttu-id="0e25b-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e25b-162">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0e25b-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e25b-163">Response</span></span>
<span data-ttu-id="0e25b-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e25b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
