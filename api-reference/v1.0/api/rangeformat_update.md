# <a name="update-rangeformat"></a><span data-ttu-id="04d2a-101">rangeformat aktualisieren</span><span class="sxs-lookup"><span data-stu-id="04d2a-101">Update rangeformat</span></span>

<span data-ttu-id="04d2a-102">Dient zum Aktualisieren der Eigenschaften des rangeformat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="04d2a-102">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="04d2a-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="04d2a-103">Permissions</span></span>
<span data-ttu-id="04d2a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="04d2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04d2a-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04d2a-106">Permission type</span></span>      | <span data-ttu-id="04d2a-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04d2a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04d2a-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04d2a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="04d2a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04d2a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="04d2a-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04d2a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04d2a-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04d2a-111">Not supported.</span></span>    |
|<span data-ttu-id="04d2a-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04d2a-112">Application</span></span> | <span data-ttu-id="04d2a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04d2a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04d2a-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04d2a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="04d2a-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04d2a-115">Request headers</span></span>
| <span data-ttu-id="04d2a-116">Name</span><span class="sxs-lookup"><span data-stu-id="04d2a-116">Name</span></span>       | <span data-ttu-id="04d2a-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04d2a-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="04d2a-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="04d2a-118">Authorization</span></span>  | <span data-ttu-id="04d2a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04d2a-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="04d2a-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="04d2a-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04d2a-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04d2a-124">Request body</span></span>
<span data-ttu-id="04d2a-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="04d2a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="04d2a-128">Property</span></span>     | <span data-ttu-id="04d2a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="04d2a-129">Type</span></span>   |<span data-ttu-id="04d2a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04d2a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04d2a-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="04d2a-131">columnWidth</span></span>|<span data-ttu-id="04d2a-132">double</span><span class="sxs-lookup"><span data-stu-id="04d2a-132">double</span></span>|<span data-ttu-id="04d2a-p105">Ruft die Breite aller Spalten innerhalb des Bereichs ab oder legt diese fest. Wenn die Breite der Spalten nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="04d2a-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="04d2a-135">horizontalAlignment</span></span>|<span data-ttu-id="04d2a-136">string</span><span class="sxs-lookup"><span data-stu-id="04d2a-136">string</span></span>|<span data-ttu-id="04d2a-137">Stellt die horizontale Ausrichtung für das angegebene Objekt dar.</span><span class="sxs-lookup"><span data-stu-id="04d2a-137">Returns or sets the horizontal alignment for the specified object.</span></span> <span data-ttu-id="04d2a-138">Mögliche Werte: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="04d2a-138">The possible values are `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`, , , , or .</span></span>|
|<span data-ttu-id="04d2a-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="04d2a-139">rowHeight</span></span>|<span data-ttu-id="04d2a-140">double</span><span class="sxs-lookup"><span data-stu-id="04d2a-140">double</span></span>|<span data-ttu-id="04d2a-p107">Ruft die Höhe aller Zeilen des Bereichs ab oder legt diese fest. Wenn die Höhe der Zeilen nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="04d2a-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="04d2a-143">verticalAlignment</span></span>|<span data-ttu-id="04d2a-144">string</span><span class="sxs-lookup"><span data-stu-id="04d2a-144">string</span></span>|<span data-ttu-id="04d2a-145">Stellt die vertikale Ausrichtung für das angegebene Objekt dar.</span><span class="sxs-lookup"><span data-stu-id="04d2a-145">Represents the vertical alignment for the specified object. Possible values are: , , , , .</span></span> <span data-ttu-id="04d2a-146">Mögliche Werte sind: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="04d2a-146">The possible values are `Top`, `Center`, `Bottom`, `Justify`, `Distributed`, , , , , , , or .</span></span>|
|<span data-ttu-id="04d2a-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="04d2a-147">wrapText</span></span>|<span data-ttu-id="04d2a-148">boolean</span><span class="sxs-lookup"><span data-stu-id="04d2a-148">boolean</span></span>|<span data-ttu-id="04d2a-p109">Gibt an, ob Excel den Text im Objekt umbricht. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Textumbruch-Einstellung hat</span><span class="sxs-lookup"><span data-stu-id="04d2a-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="04d2a-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="04d2a-151">Response</span></span>

<span data-ttu-id="04d2a-152">Wenn die Methode erfolgreich verläuft, werden der `200 OK` Antwortcode und ein aktualisiertes [WorkbookRangeFormat](../resources/rangeformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04d2a-152">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="04d2a-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04d2a-153">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="04d2a-154">Aktualisieren der Format-, Füllungs- und Schrifteigenschaften in drei Tabellenzellen</span><span class="sxs-lookup"><span data-stu-id="04d2a-154">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="04d2a-155">Die folgenden Beispiele veranschaulichen, wie die Eigenschaften [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md)und [WorkbookRangeFont](../resources/rangefont.md) eines bestimmten Bereichs aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="04d2a-155">The following examples demonstrate how to update properties of the [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md), and [RangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="04d2a-156">Das Ergebnis dieser Anforderungen ist eine Tabelle mit drei formatierten Zellen, wie in der folgenden Abbildung dargestellt.</span><span class="sxs-lookup"><span data-stu-id="04d2a-156">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![Excel-Diagrammtabelle mit drei Zellen, deren Format-, Füllungs- und Schrifteigenschaften aktualisiert wurden.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="04d2a-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04d2a-158">Request</span></span>
<span data-ttu-id="04d2a-159">Diese Anforderung aktualisiert die vertikale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="04d2a-159">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="04d2a-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="04d2a-160">Response</span></span>
<span data-ttu-id="04d2a-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="04d2a-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04d2a-164">Request</span></span>
<span data-ttu-id="04d2a-165">Diese Anforderung aktualisiert die Schriftart, Größe und Farbe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="04d2a-165">This request updates the font style, size, and color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="04d2a-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="04d2a-166">Response</span></span>
<span data-ttu-id="04d2a-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="04d2a-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04d2a-170">Request</span></span>
<span data-ttu-id="04d2a-171">Diese Anforderung aktualisiert die Hintergrundfarbe der ersten Zelle.</span><span class="sxs-lookup"><span data-stu-id="04d2a-171">This request updates the background color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="04d2a-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="04d2a-172">Response</span></span>
<span data-ttu-id="04d2a-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="04d2a-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04d2a-176">Request</span></span>
<span data-ttu-id="04d2a-177">Diese Anforderung aktualisiert die vertikale und horizontale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="04d2a-177">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="04d2a-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="04d2a-178">Response</span></span>
<span data-ttu-id="04d2a-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="04d2a-182">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04d2a-182">Request</span></span>
<span data-ttu-id="04d2a-183">Diese Anforderung aktualisiert den Schriftschnitt und Schriftgrad der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="04d2a-183">This request updates the font style and size of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="04d2a-184">Antwort</span><span class="sxs-lookup"><span data-stu-id="04d2a-184">Response</span></span>
<span data-ttu-id="04d2a-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="04d2a-188">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04d2a-188">Request</span></span>
<span data-ttu-id="04d2a-189">Diese Anforderung aktualisiert die Hintergrundfarbe der zweiten Zelle.</span><span class="sxs-lookup"><span data-stu-id="04d2a-189">This request updates the background color of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="04d2a-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="04d2a-190">Response</span></span>
<span data-ttu-id="04d2a-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="04d2a-194">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04d2a-194">Request</span></span>
<span data-ttu-id="04d2a-195">Diese Anforderung aktualisiert die horizontale Ausrichtung, die vertikale Ausrichtung, die Zeilenhöhe und Spaltenhöhe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="04d2a-195">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="04d2a-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="04d2a-196">Response</span></span>
<span data-ttu-id="04d2a-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="04d2a-200">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04d2a-200">Request</span></span>
<span data-ttu-id="04d2a-201">Diese Anforderung aktualisiert die Schriftart, Größe und Farbe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="04d2a-201">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="04d2a-202">Beachten Sie, dass die Underline-Eigenschaft die Werte **Single** oder **Double** akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="04d2a-202">Note that the underline property takes **Single** or **Double** as values.</span></span>

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
##### <a name="response"></a><span data-ttu-id="04d2a-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="04d2a-203">Response</span></span>
<span data-ttu-id="04d2a-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="04d2a-207">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04d2a-207">Request</span></span>
<span data-ttu-id="04d2a-208">Diese Anforderung aktualisiert die Hintergrundfarbe der dritten Zelle.</span><span class="sxs-lookup"><span data-stu-id="04d2a-208">This request updates the background color of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="04d2a-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="04d2a-209">Response</span></span>
<span data-ttu-id="04d2a-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04d2a-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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