---
title: rangeformat aktualisieren
description: Dient zum Aktualisieren der Eigenschaften des rangeformat-Objekts.
author: lumine2008
ms.openlocfilehash: 0aea5712db6eb149356e1c3c9db85e5aebcebf17
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344618"
---
# <a name="update-rangeformat"></a><span data-ttu-id="f13ad-103">rangeformat aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f13ad-103">Update rangeformat</span></span>

<span data-ttu-id="f13ad-104">Dient zum Aktualisieren der Eigenschaften des rangeformat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f13ad-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f13ad-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f13ad-105">Permissions</span></span>
<span data-ttu-id="f13ad-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f13ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f13ad-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f13ad-108">Permission type</span></span>      | <span data-ttu-id="f13ad-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f13ad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f13ad-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f13ad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f13ad-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f13ad-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f13ad-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f13ad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f13ad-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f13ad-113">Not supported.</span></span>    |
|<span data-ttu-id="f13ad-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f13ad-114">Application</span></span> | <span data-ttu-id="f13ad-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f13ad-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f13ad-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f13ad-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="f13ad-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f13ad-117">Request headers</span></span>
| <span data-ttu-id="f13ad-118">Name</span><span class="sxs-lookup"><span data-stu-id="f13ad-118">Name</span></span>       | <span data-ttu-id="f13ad-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f13ad-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f13ad-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f13ad-120">Authorization</span></span>  | <span data-ttu-id="f13ad-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f13ad-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="f13ad-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f13ad-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f13ad-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f13ad-126">Request body</span></span>
<span data-ttu-id="f13ad-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f13ad-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f13ad-130">Property</span></span>     | <span data-ttu-id="f13ad-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f13ad-131">Type</span></span>   |<span data-ttu-id="f13ad-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f13ad-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f13ad-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="f13ad-133">columnWidth</span></span>|<span data-ttu-id="f13ad-134">double</span><span class="sxs-lookup"><span data-stu-id="f13ad-134">double</span></span>|<span data-ttu-id="f13ad-p105">Ruft die Breite aller Spalten innerhalb des Bereichs ab oder legt diese fest. Wenn die Breite der Spalten nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="f13ad-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="f13ad-137">horizontalAlignment</span></span>|<span data-ttu-id="f13ad-138">string</span><span class="sxs-lookup"><span data-stu-id="f13ad-138">string</span></span>|<span data-ttu-id="f13ad-139">Die horizontale Ausrichtung für das angegebene Objekt darstellt.</span><span class="sxs-lookup"><span data-stu-id="f13ad-139">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="f13ad-140">Die möglichen Werte sind: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="f13ad-140">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="f13ad-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="f13ad-141">rowHeight</span></span>|<span data-ttu-id="f13ad-142">double</span><span class="sxs-lookup"><span data-stu-id="f13ad-142">double</span></span>|<span data-ttu-id="f13ad-p107">Ruft die Höhe aller Zeilen des Bereichs ab oder legt diese fest. Wenn die Höhe der Zeilen nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="f13ad-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="f13ad-145">verticalAlignment</span></span>|<span data-ttu-id="f13ad-146">string</span><span class="sxs-lookup"><span data-stu-id="f13ad-146">string</span></span>|<span data-ttu-id="f13ad-147">Die vertikale Ausrichtung für das angegebene Objekt darstellt.</span><span class="sxs-lookup"><span data-stu-id="f13ad-147">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="f13ad-148">Die möglichen Werte sind: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="f13ad-148">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="f13ad-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="f13ad-149">wrapText</span></span>|<span data-ttu-id="f13ad-150">boolean</span><span class="sxs-lookup"><span data-stu-id="f13ad-150">boolean</span></span>|<span data-ttu-id="f13ad-p109">Gibt an, ob Excel den Text im Objekt umbricht. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Textumbruch-Einstellung hat</span><span class="sxs-lookup"><span data-stu-id="f13ad-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="f13ad-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="f13ad-153">Response</span></span>

<span data-ttu-id="f13ad-154">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [WorkbookRangeFormat](../resources/rangeformat.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f13ad-154">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f13ad-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f13ad-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="f13ad-156">Aktualisieren der Format-, Füllungs- und Schrifteigenschaften in drei Tabellenzellen</span><span class="sxs-lookup"><span data-stu-id="f13ad-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="f13ad-157">Die folgenden Beispiele veranschaulichen, wie die Eigenschaften der [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md)und [WorkbookRangeFont](../resources/rangefont.md) Eigenschaften eines bestimmten Bereichs aktualisiert wird.</span><span class="sxs-lookup"><span data-stu-id="f13ad-157">The following examples demonstrate how to update properties of the [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md), and [WorkbookRangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="f13ad-158">Das Ergebnis dieser Anforderungen ist eine Tabelle mit drei formatierten Zellen, wie in der folgenden Abbildung dargestellt.</span><span class="sxs-lookup"><span data-stu-id="f13ad-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Excel-Diagrammtabelle mit drei Zellen, deren Format-, Füllungs- und Schrifteigenschaften aktualisiert wurden.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="f13ad-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f13ad-160">Request</span></span>
<span data-ttu-id="f13ad-161">Diese Anforderung aktualisiert die vertikale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="f13ad-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="f13ad-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="f13ad-162">Response</span></span>
<span data-ttu-id="f13ad-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="f13ad-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f13ad-166">Request</span></span>
<span data-ttu-id="f13ad-167">Diese Anforderung aktualisiert die Schriftart, Größe und Farbe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="f13ad-167">This request updates the font style, size, and color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="f13ad-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="f13ad-168">Response</span></span>
<span data-ttu-id="f13ad-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="f13ad-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f13ad-172">Request</span></span>
<span data-ttu-id="f13ad-173">Diese Anforderung aktualisiert die Hintergrundfarbe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="f13ad-173">This request updates the background color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="f13ad-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="f13ad-174">Response</span></span>
<span data-ttu-id="f13ad-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="f13ad-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f13ad-178">Request</span></span>
<span data-ttu-id="f13ad-179">Diese Anforderung aktualisiert die vertikale und horizontale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="f13ad-179">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="f13ad-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="f13ad-180">Response</span></span>
<span data-ttu-id="f13ad-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="f13ad-184">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f13ad-184">Request</span></span>
<span data-ttu-id="f13ad-185">Diese Anforderung aktualisiert den Schriftschnitt und Schriftgrad der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="f13ad-185">This request updates the font style and size of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="f13ad-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="f13ad-186">Response</span></span>
<span data-ttu-id="f13ad-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="f13ad-190">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f13ad-190">Request</span></span>
<span data-ttu-id="f13ad-191">Diese Anforderung aktualisiert die Hintergrundfarbe der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="f13ad-191">This request updates the background color of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="f13ad-192">Antwort</span><span class="sxs-lookup"><span data-stu-id="f13ad-192">Response</span></span>
<span data-ttu-id="f13ad-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="f13ad-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f13ad-196">Request</span></span>
<span data-ttu-id="f13ad-197">Diese Anforderung aktualisiert die horizontale Ausrichtung, die vertikale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="f13ad-197">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="f13ad-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="f13ad-198">Response</span></span>
<span data-ttu-id="f13ad-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="f13ad-202">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f13ad-202">Request</span></span>
<span data-ttu-id="f13ad-203">Diese Anforderung aktualisiert die Schriftart, Größe und Farbe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="f13ad-203">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="f13ad-204">Beachten Sie, dass die Underline-Eigenschaft die Werte **Single** oder **Double** akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="f13ad-204">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="f13ad-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="f13ad-205">Response</span></span>
<span data-ttu-id="f13ad-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="f13ad-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f13ad-209">Request</span></span>
<span data-ttu-id="f13ad-210">Diese Anforderung aktualisiert die Hintergrundfarbe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="f13ad-210">This request updates the background color of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="f13ad-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="f13ad-211">Response</span></span>
<span data-ttu-id="f13ad-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f13ad-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: update_rangeformat_font_three/underline:
      Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ],
  "tocPath": ""
}-->