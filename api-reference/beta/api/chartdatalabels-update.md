---
title: ChartDataLabels aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des ChartDataLabels-Objekts.
ms.openlocfilehash: e98569645048aced34566c4ca077d9e0ca921118
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062804"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="5749a-103">ChartDataLabels aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5749a-103">Update chartdatalabels</span></span>

> <span data-ttu-id="5749a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5749a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5749a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5749a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5749a-106">Dient zum Aktualisieren der Eigenschaften des ChartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5749a-106">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5749a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5749a-107">Permissions</span></span>
<span data-ttu-id="5749a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5749a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5749a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5749a-110">Permission type</span></span>      | <span data-ttu-id="5749a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5749a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5749a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5749a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5749a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5749a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5749a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5749a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5749a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5749a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5749a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5749a-116">Application</span></span> | <span data-ttu-id="5749a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5749a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5749a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5749a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="5749a-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5749a-119">Optional request headers</span></span>
| <span data-ttu-id="5749a-120">Name</span><span class="sxs-lookup"><span data-stu-id="5749a-120">Name</span></span>       | <span data-ttu-id="5749a-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5749a-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5749a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5749a-122">Authorization</span></span>  | <span data-ttu-id="5749a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5749a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5749a-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="5749a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="5749a-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="5749a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5749a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5749a-128">Request body</span></span>
<span data-ttu-id="5749a-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="5749a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5749a-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5749a-132">Property</span></span>     | <span data-ttu-id="5749a-133">Typ</span><span class="sxs-lookup"><span data-stu-id="5749a-133">Type</span></span>   |<span data-ttu-id="5749a-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5749a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5749a-135">position</span><span class="sxs-lookup"><span data-stu-id="5749a-135">position</span></span>|<span data-ttu-id="5749a-136">string</span><span class="sxs-lookup"><span data-stu-id="5749a-136">string</span></span>|<span data-ttu-id="5749a-p106">DataLabelPosition-Wert, der die Position der Datenbeschriftung darstellt. Mögliche Werte: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="5749a-p106">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="5749a-139">Separator</span><span class="sxs-lookup"><span data-stu-id="5749a-139">separator</span></span>|<span data-ttu-id="5749a-140">string</span><span class="sxs-lookup"><span data-stu-id="5749a-140">string</span></span>|<span data-ttu-id="5749a-141">Zeichenfolge, die das Trennzeichen für die Datenbeschriftungen in einem Diagramm darstellt.</span><span class="sxs-lookup"><span data-stu-id="5749a-141">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="5749a-142">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="5749a-142">showBubbleSize</span></span>|<span data-ttu-id="5749a-143">boolean</span><span class="sxs-lookup"><span data-stu-id="5749a-143">boolean</span></span>|<span data-ttu-id="5749a-144">Boolescher Wert, der angibt, ob die Größe der Datenbeschriftungs-Sprechblase angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5749a-144">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="5749a-145">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="5749a-145">showCategoryName</span></span>|<span data-ttu-id="5749a-146">boolean</span><span class="sxs-lookup"><span data-stu-id="5749a-146">boolean</span></span>|<span data-ttu-id="5749a-147">Boolescher Wert, der angibt, ob der Kategoriename der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5749a-147">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="5749a-148">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="5749a-148">showLegendKey</span></span>|<span data-ttu-id="5749a-149">boolean</span><span class="sxs-lookup"><span data-stu-id="5749a-149">boolean</span></span>|<span data-ttu-id="5749a-150">Boolescher Wert, der angibt, ob das Legendensymbol der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5749a-150">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="5749a-151">showPercentage</span><span class="sxs-lookup"><span data-stu-id="5749a-151">showPercentage</span></span>|<span data-ttu-id="5749a-152">boolean</span><span class="sxs-lookup"><span data-stu-id="5749a-152">boolean</span></span>|<span data-ttu-id="5749a-153">Boolescher Wert, der angibt, ob der Prozentsatz der Datenbeschriftung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5749a-153">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="5749a-154">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="5749a-154">showSeriesName</span></span>|<span data-ttu-id="5749a-155">boolean</span><span class="sxs-lookup"><span data-stu-id="5749a-155">boolean</span></span>|<span data-ttu-id="5749a-156">Boolescher Wert, der angibt, ob der Name der Datenbeschriftungsreihe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5749a-156">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="5749a-157">showValue</span><span class="sxs-lookup"><span data-stu-id="5749a-157">showValue</span></span>|<span data-ttu-id="5749a-158">boolean</span><span class="sxs-lookup"><span data-stu-id="5749a-158">boolean</span></span>|<span data-ttu-id="5749a-159">Boolescher Wert, der angibt, ob der Datenbeschriftungswert angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="5749a-159">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="5749a-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="5749a-160">Response</span></span>

<span data-ttu-id="5749a-161">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartDataLabels](../resources/chartdatalabels.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5749a-161">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5749a-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5749a-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5749a-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5749a-163">Request</span></span>
<span data-ttu-id="5749a-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5749a-164">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="5749a-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="5749a-165">Response</span></span>
<span data-ttu-id="5749a-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5749a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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