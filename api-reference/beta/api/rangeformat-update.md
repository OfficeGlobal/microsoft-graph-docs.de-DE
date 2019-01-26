---
title: rangeformat aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des rangeformat-Objekts.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b1b3f768af0efe94c5b14177c5e70bbe9a642174
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574425"
---
# <a name="update-rangeformat"></a><span data-ttu-id="5a66b-103">rangeformat aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5a66b-103">Update rangeformat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a66b-104">Dient zum Aktualisieren der Eigenschaften des rangeformat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5a66b-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5a66b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5a66b-105">Permissions</span></span>
<span data-ttu-id="5a66b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a66b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a66b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a66b-108">Permission type</span></span>      | <span data-ttu-id="5a66b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a66b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a66b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a66b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5a66b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a66b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5a66b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a66b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a66b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a66b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5a66b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a66b-114">Application</span></span> | <span data-ttu-id="5a66b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a66b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a66b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a66b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="5a66b-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a66b-117">Optional request headers</span></span>
| <span data-ttu-id="5a66b-118">Name</span><span class="sxs-lookup"><span data-stu-id="5a66b-118">Name</span></span>       | <span data-ttu-id="5a66b-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a66b-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5a66b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a66b-120">Authorization</span></span>  | <span data-ttu-id="5a66b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a66b-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="5a66b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5a66b-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a66b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a66b-126">Request body</span></span>
<span data-ttu-id="5a66b-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5a66b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5a66b-130">Property</span></span>     | <span data-ttu-id="5a66b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5a66b-131">Type</span></span>   |<span data-ttu-id="5a66b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a66b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a66b-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="5a66b-133">columnWidth</span></span>|<span data-ttu-id="5a66b-134">double</span><span class="sxs-lookup"><span data-stu-id="5a66b-134">double</span></span>|<span data-ttu-id="5a66b-p105">Ruft die Breite aller Spalten innerhalb des Bereichs ab oder legt diese fest. Wenn die Breite der Spalten nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="5a66b-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="5a66b-137">horizontalAlignment</span></span>|<span data-ttu-id="5a66b-138">string</span><span class="sxs-lookup"><span data-stu-id="5a66b-138">string</span></span>|<span data-ttu-id="5a66b-p106">Stellt die horizontale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p106">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="5a66b-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="5a66b-141">rowHeight</span></span>|<span data-ttu-id="5a66b-142">double</span><span class="sxs-lookup"><span data-stu-id="5a66b-142">double</span></span>|<span data-ttu-id="5a66b-p107">Ruft die Höhe aller Zeilen des Bereichs ab oder legt diese fest. Wenn die Höhe der Zeilen nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="5a66b-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="5a66b-145">verticalAlignment</span></span>|<span data-ttu-id="5a66b-146">string</span><span class="sxs-lookup"><span data-stu-id="5a66b-146">string</span></span>|<span data-ttu-id="5a66b-p108">Stellt die vertikale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p108">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="5a66b-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="5a66b-149">wrapText</span></span>|<span data-ttu-id="5a66b-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5a66b-150">boolean</span></span>|<span data-ttu-id="5a66b-p109">Gibt an, ob Excel den Text im Objekt umbricht. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Textumbruch-Einstellung hat</span><span class="sxs-lookup"><span data-stu-id="5a66b-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="5a66b-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a66b-153">Response</span></span>

<span data-ttu-id="5a66b-154">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [RangeFormat](../resources/rangeformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a66b-154">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5a66b-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5a66b-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="5a66b-156">Aktualisieren der Format-, Füllungs- und Schrifteigenschaften in drei Tabellenzellen</span><span class="sxs-lookup"><span data-stu-id="5a66b-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="5a66b-157">In den folgenden Beispielen wird veranschaulicht, wie die Eigenschaften der [RangeFormat](../resources/rangeformat.md)-, [RangeFill](../resources/rangefill.md)- und [RangeFont](../resources/rangefont.md)-Eigenschaften eines bestimmten Bereichs aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="5a66b-157">The following examples demonstrate how to update properties of the [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md), and [RangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="5a66b-158">Das Ergebnis dieser Anforderungen ist eine Tabelle mit drei formatierten Zellen, wie in der folgenden Abbildung dargestellt.</span><span class="sxs-lookup"><span data-stu-id="5a66b-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Excel-Diagrammtabelle mit drei Zellen, deren Format-, Füllungs- und Schrifteigenschaften aktualisiert wurden.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="5a66b-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a66b-160">Request</span></span>
<span data-ttu-id="5a66b-161">Diese Anforderung aktualisiert die vertikale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="5a66b-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="5a66b-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a66b-162">Response</span></span>
<span data-ttu-id="5a66b-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="5a66b-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a66b-166">Request</span></span>
<span data-ttu-id="5a66b-167">Diese Anforderung aktualisiert die Schriftart, Größe und Farbe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="5a66b-167">This request updates the font style, size, and color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="5a66b-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a66b-168">Response</span></span>
<span data-ttu-id="5a66b-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="5a66b-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a66b-172">Request</span></span>
<span data-ttu-id="5a66b-173">Diese Anforderung aktualisiert die Hintergrundfarbe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="5a66b-173">This request updates the background color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="5a66b-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a66b-174">Response</span></span>
<span data-ttu-id="5a66b-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#FF0000"
}
```
##### <a name="request"></a><span data-ttu-id="5a66b-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a66b-178">Request</span></span>
<span data-ttu-id="5a66b-179">Diese Anforderung aktualisiert die vertikale und horizontale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="5a66b-179">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="5a66b-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a66b-180">Response</span></span>
<span data-ttu-id="5a66b-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="5a66b-184">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a66b-184">Request</span></span>
<span data-ttu-id="5a66b-185">Diese Anforderung aktualisiert den Schriftschnitt und Schriftgrad der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="5a66b-185">This request updates the font style and size of the second cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="5a66b-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a66b-186">Response</span></span>
<span data-ttu-id="5a66b-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="5a66b-190">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a66b-190">Request</span></span>
<span data-ttu-id="5a66b-191">Diese Anforderung aktualisiert die Hintergrundfarbe der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="5a66b-191">This request updates the background color of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="5a66b-192">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a66b-192">Response</span></span>
<span data-ttu-id="5a66b-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#00FF00"
}
```

##### <a name="request"></a><span data-ttu-id="5a66b-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a66b-196">Request</span></span>
<span data-ttu-id="5a66b-197">Diese Anforderung aktualisiert die horizontale Ausrichtung, die vertikale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="5a66b-197">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="5a66b-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a66b-198">Response</span></span>
<span data-ttu-id="5a66b-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="5a66b-202">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a66b-202">Request</span></span>
<span data-ttu-id="5a66b-203">Diese Anforderung aktualisiert die Schriftart, Größe und Farbe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="5a66b-203">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="5a66b-204">Beachten Sie, dass die Underline-Eigenschaft die Werte **Single** oder **Double** akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="5a66b-204">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "None",
  "color": "#FFFFFF",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="5a66b-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a66b-205">Response</span></span>
<span data-ttu-id="5a66b-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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
    "underline": "None"
}
```

##### <a name="request"></a><span data-ttu-id="5a66b-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a66b-209">Request</span></span>
<span data-ttu-id="5a66b-210">Diese Anforderung aktualisiert die Hintergrundfarbe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="5a66b-210">This request updates the background color of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="5a66b-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a66b-211">Response</span></span>
<span data-ttu-id="5a66b-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a66b-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#0000FF"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
