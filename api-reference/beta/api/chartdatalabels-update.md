---
title: ChartDataLabels aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartDataLabels-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 194d48075f143670488c6ae1ab0ff7a92934e4c4
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573242"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="b5d08-103">ChartDataLabels aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b5d08-103">Update chartdatalabels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5d08-104">Dient zum Aktualisieren der Eigenschaften des ChartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b5d08-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5d08-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b5d08-105">Permissions</span></span>
<span data-ttu-id="b5d08-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5d08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5d08-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5d08-108">Permission type</span></span>      | <span data-ttu-id="b5d08-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5d08-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5d08-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5d08-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5d08-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5d08-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b5d08-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5d08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5d08-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5d08-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b5d08-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5d08-114">Application</span></span> | <span data-ttu-id="b5d08-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5d08-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5d08-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5d08-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="b5d08-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b5d08-117">Optional request headers</span></span>
| <span data-ttu-id="b5d08-118">Name</span><span class="sxs-lookup"><span data-stu-id="b5d08-118">Name</span></span>       | <span data-ttu-id="b5d08-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5d08-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b5d08-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5d08-120">Authorization</span></span>  | <span data-ttu-id="b5d08-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b5d08-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b5d08-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b5d08-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b5d08-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b5d08-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5d08-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b5d08-126">Request body</span></span>
<span data-ttu-id="b5d08-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="b5d08-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b5d08-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5d08-130">Property</span></span>     | <span data-ttu-id="b5d08-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b5d08-131">Type</span></span>   |<span data-ttu-id="b5d08-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5d08-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5d08-133">position</span><span class="sxs-lookup"><span data-stu-id="b5d08-133">position</span></span>|<span data-ttu-id="b5d08-134">string</span><span class="sxs-lookup"><span data-stu-id="b5d08-134">string</span></span>|<span data-ttu-id="b5d08-135">DataLabelPosition-Wert, der die Position der Datenbeschriftung darstellt.</span><span class="sxs-lookup"><span data-stu-id="b5d08-135">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="b5d08-136">Die möglichen Werte sind: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="b5d08-136">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="b5d08-137">Separator</span><span class="sxs-lookup"><span data-stu-id="b5d08-137">separator</span></span>|<span data-ttu-id="b5d08-138">string</span><span class="sxs-lookup"><span data-stu-id="b5d08-138">string</span></span>|<span data-ttu-id="b5d08-139">Zeichenfolge, die das Trennzeichen für die Datenbeschriftungen in einem Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="b5d08-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="b5d08-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="b5d08-140">showBubbleSize</span></span>|<span data-ttu-id="b5d08-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b5d08-141">boolean</span></span>|<span data-ttu-id="b5d08-142">Boolescher Wert, der angibt, ob die Größe der Datenbeschriftungs-Sprechblase angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b5d08-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="b5d08-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="b5d08-143">showCategoryName</span></span>|<span data-ttu-id="b5d08-144">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b5d08-144">boolean</span></span>|<span data-ttu-id="b5d08-145">Boolescher Wert, der angibt, ob der Kategoriename der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b5d08-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="b5d08-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="b5d08-146">showLegendKey</span></span>|<span data-ttu-id="b5d08-147">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b5d08-147">boolean</span></span>|<span data-ttu-id="b5d08-148">Boolescher Wert, der angibt, ob das Legendensymbol der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b5d08-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="b5d08-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="b5d08-149">showPercentage</span></span>|<span data-ttu-id="b5d08-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b5d08-150">boolean</span></span>|<span data-ttu-id="b5d08-151">Boolescher Wert, der angibt, ob der Prozentsatz der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b5d08-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="b5d08-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="b5d08-152">showSeriesName</span></span>|<span data-ttu-id="b5d08-153">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b5d08-153">boolean</span></span>|<span data-ttu-id="b5d08-154">Boolescher Wert, der angibt, ob der Name der Datenbeschriftungsreihe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b5d08-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="b5d08-155">showValue</span><span class="sxs-lookup"><span data-stu-id="b5d08-155">showValue</span></span>|<span data-ttu-id="b5d08-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b5d08-156">boolean</span></span>|<span data-ttu-id="b5d08-157">Boolescher Wert, der angibt, ob der Datenbeschriftungswert angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b5d08-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="b5d08-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5d08-158">Response</span></span>

<span data-ttu-id="b5d08-159">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookChartDataLabels](../resources/chartdatalabels.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b5d08-159">If successful, this method returns a `200 OK` response code and updated [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5d08-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b5d08-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5d08-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5d08-161">Request</span></span>
<span data-ttu-id="b5d08-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b5d08-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/datalabels
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
##### <a name="response"></a><span data-ttu-id="b5d08-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5d08-163">Response</span></span>
<span data-ttu-id="b5d08-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5d08-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartdatalabels-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
