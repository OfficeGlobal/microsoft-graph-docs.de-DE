---
title: rangeformat aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des rangeformat-Objekts.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8d7df390628e1f8a4416042efe218e36c516a669
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873241"
---
# <a name="update-rangeformat"></a><span data-ttu-id="12fa6-103">rangeformat aktualisieren</span><span class="sxs-lookup"><span data-stu-id="12fa6-103">Update rangeformat</span></span>

> <span data-ttu-id="12fa6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="12fa6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12fa6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12fa6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12fa6-106">Dient zum Aktualisieren der Eigenschaften des rangeformat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="12fa6-106">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="12fa6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="12fa6-107">Permissions</span></span>
<span data-ttu-id="12fa6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fa6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12fa6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="12fa6-110">Permission type</span></span>      | <span data-ttu-id="12fa6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="12fa6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12fa6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="12fa6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="12fa6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12fa6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="12fa6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="12fa6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12fa6-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12fa6-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="12fa6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="12fa6-116">Application</span></span> | <span data-ttu-id="12fa6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="12fa6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12fa6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fa6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="12fa6-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="12fa6-119">Optional request headers</span></span>
| <span data-ttu-id="12fa6-120">Name</span><span class="sxs-lookup"><span data-stu-id="12fa6-120">Name</span></span>       | <span data-ttu-id="12fa6-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12fa6-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="12fa6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12fa6-122">Authorization</span></span>  | <span data-ttu-id="12fa6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12fa6-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="12fa6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="12fa6-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12fa6-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="12fa6-128">Request body</span></span>
<span data-ttu-id="12fa6-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="12fa6-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="12fa6-132">Property</span></span>     | <span data-ttu-id="12fa6-133">Typ</span><span class="sxs-lookup"><span data-stu-id="12fa6-133">Type</span></span>   |<span data-ttu-id="12fa6-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12fa6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12fa6-135">columnWidth</span><span class="sxs-lookup"><span data-stu-id="12fa6-135">columnWidth</span></span>|<span data-ttu-id="12fa6-136">double</span><span class="sxs-lookup"><span data-stu-id="12fa6-136">double</span></span>|<span data-ttu-id="12fa6-p106">Ruft die Breite aller Spalten innerhalb des Bereichs ab oder legt diese fest. Wenn die Breite der Spalten nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p106">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="12fa6-139">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="12fa6-139">horizontalAlignment</span></span>|<span data-ttu-id="12fa6-140">string</span><span class="sxs-lookup"><span data-stu-id="12fa6-140">string</span></span>|<span data-ttu-id="12fa6-p107">Stellt die horizontale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p107">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="12fa6-143">rowHeight</span><span class="sxs-lookup"><span data-stu-id="12fa6-143">rowHeight</span></span>|<span data-ttu-id="12fa6-144">double</span><span class="sxs-lookup"><span data-stu-id="12fa6-144">double</span></span>|<span data-ttu-id="12fa6-p108">Ruft die Höhe aller Zeilen des Bereichs ab oder legt diese fest. Wenn die Höhe der Zeilen nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p108">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="12fa6-147">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="12fa6-147">verticalAlignment</span></span>|<span data-ttu-id="12fa6-148">string</span><span class="sxs-lookup"><span data-stu-id="12fa6-148">string</span></span>|<span data-ttu-id="12fa6-p109">Stellt die vertikale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p109">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="12fa6-151">wrapText</span><span class="sxs-lookup"><span data-stu-id="12fa6-151">wrapText</span></span>|<span data-ttu-id="12fa6-152">boolean</span><span class="sxs-lookup"><span data-stu-id="12fa6-152">boolean</span></span>|<span data-ttu-id="12fa6-p110">Gibt an, ob Excel den Text im Objekt umbricht. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Textumbruch-Einstellung hat</span><span class="sxs-lookup"><span data-stu-id="12fa6-p110">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="12fa6-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fa6-155">Response</span></span>

<span data-ttu-id="12fa6-156">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [RangeFormat](../resources/rangeformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-156">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12fa6-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="12fa6-157">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="12fa6-158">Aktualisieren der Format-, Füllungs- und Schrifteigenschaften in drei Tabellenzellen</span><span class="sxs-lookup"><span data-stu-id="12fa6-158">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="12fa6-159">In den folgenden Beispielen wird veranschaulicht, wie die Eigenschaften der [RangeFormat](../resources/rangeformat.md)-, [RangeFill](../resources/rangefill.md)- und [RangeFont](../resources/rangefont.md)-Eigenschaften eines bestimmten Bereichs aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="12fa6-159">The following examples demonstrate how to update properties of the [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md), and [RangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="12fa6-160">Das Ergebnis dieser Anforderungen ist eine Tabelle mit drei formatierten Zellen, wie in der folgenden Abbildung dargestellt.</span><span class="sxs-lookup"><span data-stu-id="12fa6-160">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Excel-Diagrammtabelle mit drei Zellen, deren Format-, Füllungs- und Schrifteigenschaften aktualisiert wurden.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="12fa6-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fa6-162">Request</span></span>
<span data-ttu-id="12fa6-163">Diese Anforderung aktualisiert die vertikale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="12fa6-163">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="12fa6-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fa6-164">Response</span></span>
<span data-ttu-id="12fa6-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="12fa6-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fa6-168">Request</span></span>
<span data-ttu-id="12fa6-169">Diese Anforderung aktualisiert die Schriftart, Größe und Farbe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="12fa6-169">This request updates the font style, size, and color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="12fa6-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fa6-170">Response</span></span>
<span data-ttu-id="12fa6-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="12fa6-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fa6-174">Request</span></span>
<span data-ttu-id="12fa6-175">Diese Anforderung aktualisiert die Hintergrundfarbe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="12fa6-175">This request updates the background color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="12fa6-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fa6-176">Response</span></span>
<span data-ttu-id="12fa6-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="12fa6-180">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fa6-180">Request</span></span>
<span data-ttu-id="12fa6-181">Diese Anforderung aktualisiert die vertikale und horizontale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="12fa6-181">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="12fa6-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fa6-182">Response</span></span>
<span data-ttu-id="12fa6-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="12fa6-186">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fa6-186">Request</span></span>
<span data-ttu-id="12fa6-187">Diese Anforderung aktualisiert den Schriftschnitt und Schriftgrad der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="12fa6-187">This request updates the font style and size of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="12fa6-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fa6-188">Response</span></span>
<span data-ttu-id="12fa6-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="12fa6-192">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fa6-192">Request</span></span>
<span data-ttu-id="12fa6-193">Diese Anforderung aktualisiert die Hintergrundfarbe der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="12fa6-193">This request updates the background color of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="12fa6-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fa6-194">Response</span></span>
<span data-ttu-id="12fa6-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="12fa6-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fa6-198">Request</span></span>
<span data-ttu-id="12fa6-199">Diese Anforderung aktualisiert die horizontale Ausrichtung, die vertikale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="12fa6-199">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="12fa6-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fa6-200">Response</span></span>
<span data-ttu-id="12fa6-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="12fa6-204">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fa6-204">Request</span></span>
<span data-ttu-id="12fa6-205">Diese Anforderung aktualisiert die Schriftart, Größe und Farbe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="12fa6-205">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="12fa6-206">Beachten Sie, dass die Underline-Eigenschaft die Werte **Single** oder **Double** akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="12fa6-206">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="12fa6-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fa6-207">Response</span></span>
<span data-ttu-id="12fa6-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "underline": "Single"
}
```

##### <a name="request"></a><span data-ttu-id="12fa6-211">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12fa6-211">Request</span></span>
<span data-ttu-id="12fa6-212">Diese Anforderung aktualisiert die Hintergrundfarbe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="12fa6-212">This request updates the background color of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="12fa6-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="12fa6-213">Response</span></span>
<span data-ttu-id="12fa6-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12fa6-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
