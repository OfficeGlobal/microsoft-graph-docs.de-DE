---
title: Aktualisieren eines Bereichsformats in Excel mit Microsoft Graph
description: In den folgenden Beispielen wird veranschaulicht, wie die Eigenschaften der RangeFormat-, RangeFill- und RangeFont-Eigenschaften eines bestimmten Bereichs aktualisiert werden können.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: ad1aae186fb7803ff38c321f87bd786096d257a1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971641"
---
# <a name="update-a-range-format-in-excel-with-microsoft-graph"></a><span data-ttu-id="0d096-103">Aktualisieren eines Bereichsformats in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0d096-103">Update a range format in Excel with Microsoft Graph</span></span>

<span data-ttu-id="0d096-104">In den folgenden Beispielen wird veranschaulicht, wie die Eigenschaften der [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0)-, [RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0)- und [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0)-Eigenschaften eines bestimmten Bereichs aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="0d096-104">The following examples demonstrate how to update properties of the [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0), [RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0), and [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) properties of a specified range.</span></span>

<span data-ttu-id="0d096-105">Das Ergebnis dieser Anforderungen ist eine Tabelle mit drei formatierten Zellen, wie in der folgenden Abbildung dargestellt.</span><span class="sxs-lookup"><span data-stu-id="0d096-105">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Excel-Diagrammtabelle mit drei Zellen, deren Format-, Füllungs- und Schrifteigenschaften aktualisiert wurden.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="0d096-107">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d096-107">Request</span></span>
<span data-ttu-id="0d096-108">Diese Anforderung aktualisiert die vertikale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="0d096-108">This request updates the vertical alignment, row height, and column height of the first cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="0d096-109">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d096-109">Response</span></span>
<span data-ttu-id="0d096-p101">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d096-p101">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "General",
    "rowHeight": 49,
    "verticalAlignment": "Top",
    "wrapText": false
}
```

##### <a name="request"></a><span data-ttu-id="0d096-113">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d096-113">Request</span></span>
<span data-ttu-id="0d096-114">Diese Anforderung aktualisiert die Schriftart, Größe und Farbe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="0d096-114">This request updates the font style, size, and color of the first cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="0d096-115">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d096-115">Response</span></span>
<span data-ttu-id="0d096-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d096-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": true,
    "color": "#4B180E",
    "italic": false,
    "name": "Calibri",
    "size": 26,
    "underline": "None"
}
```

##### <a name="request"></a><span data-ttu-id="0d096-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d096-119">Request</span></span>
<span data-ttu-id="0d096-120">Diese Anforderung aktualisiert die Hintergrundfarbe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="0d096-120">This request updates the background color of the first cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="0d096-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d096-121">Response</span></span>
<span data-ttu-id="0d096-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d096-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#FF0000"
}
```
##### <a name="request"></a><span data-ttu-id="0d096-125">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d096-125">Request</span></span>
<span data-ttu-id="0d096-126">Diese Anforderung aktualisiert die vertikale und horizontale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="0d096-126">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="0d096-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d096-127">Response</span></span>
<span data-ttu-id="0d096-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d096-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "Center",
    "rowHeight": 49,
    "verticalAlignment": "Center",
    "wrapText": false
}
```

##### <a name="request"></a><span data-ttu-id="0d096-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d096-131">Request</span></span>
<span data-ttu-id="0d096-132">Diese Anforderung aktualisiert den Schriftschnitt und Schriftgrad der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="0d096-132">This request updates the font style and size of the second cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="0d096-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d096-133">Response</span></span>
<span data-ttu-id="0d096-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d096-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": false,
    "color": "#000000",
    "italic": true,
    "name": "Calibri",
    "size": 26,
    "underline": "None"
}
```

##### <a name="request"></a><span data-ttu-id="0d096-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d096-137">Request</span></span>
<span data-ttu-id="0d096-138">Diese Anforderung aktualisiert die Hintergrundfarbe der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="0d096-138">This request updates the background color of the second cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="0d096-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d096-139">Response</span></span>
<span data-ttu-id="0d096-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d096-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#00FF00"
}
```

##### <a name="request"></a><span data-ttu-id="0d096-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d096-143">Request</span></span>
<span data-ttu-id="0d096-144">Diese Anforderung aktualisiert die horizontale Ausrichtung, die vertikale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="0d096-144">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="0d096-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d096-145">Response</span></span>
<span data-ttu-id="0d096-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d096-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "Right",
    "rowHeight": 49,
    "verticalAlignment": "Top",
    "wrapText": false
}
```

##### <a name="request"></a><span data-ttu-id="0d096-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d096-149">Request</span></span>
<span data-ttu-id="0d096-150">Diese Anforderung aktualisiert die Schriftart, Größe und Farbe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="0d096-150">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="0d096-151">Beachten Sie, dass die Underline-Eigenschaft die Werte **Single** oder **Double** akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="0d096-151">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="0d096-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d096-152">Response</span></span>
<span data-ttu-id="0d096-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d096-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": false,
    "color": "#FFFFFF",
    "italic": false,
    "name": "Calibri",
    "size": 26,
    "underline": "Single"
}
```

##### <a name="request"></a><span data-ttu-id="0d096-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d096-156">Request</span></span>
<span data-ttu-id="0d096-157">Diese Anforderung aktualisiert die Hintergrundfarbe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="0d096-157">This request updates the background color of the third cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="0d096-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d096-158">Response</span></span>
<span data-ttu-id="0d096-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d096-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#0000FF"
}
```


## <a name="see-also"></a><span data-ttu-id="0d096-162">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="0d096-162">See also</span></span>
* [<span data-ttu-id="0d096-163">Verwalten von Sitzungen in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0d096-163">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="0d096-164">Schreiben in eine Excel-Arbeitsmappe mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0d096-164">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="0d096-165">Verwenden von Arbeitsmappenfunktionen in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0d096-165">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="0d096-166">Anzeigen eines Diagrammbilds in Excel mithilfe von Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0d096-166">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="0d096-167">Verwenden der Excel-REST-API</span><span class="sxs-lookup"><span data-stu-id="0d096-167">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
