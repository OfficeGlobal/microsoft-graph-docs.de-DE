# <a name="update-rangeformat"></a><span data-ttu-id="15d15-101">rangeformat aktualisieren</span><span class="sxs-lookup"><span data-stu-id="15d15-101">Update rangeformat</span></span>

<span data-ttu-id="15d15-102">Dient zum Aktualisieren der Eigenschaften des rangeformat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="15d15-102">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="15d15-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="15d15-103">Permissions</span></span>
<span data-ttu-id="15d15-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="15d15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="15d15-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15d15-106">Permission type</span></span>      | <span data-ttu-id="15d15-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15d15-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15d15-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15d15-108">Delegated (work or school account)</span></span> | <span data-ttu-id="15d15-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15d15-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="15d15-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15d15-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15d15-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15d15-111">Not supported.</span></span>    |
|<span data-ttu-id="15d15-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15d15-112">Application</span></span> | <span data-ttu-id="15d15-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15d15-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15d15-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15d15-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(<address>)/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="15d15-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15d15-115">Optional request headers</span></span>
| <span data-ttu-id="15d15-116">Name</span><span class="sxs-lookup"><span data-stu-id="15d15-116">Name</span></span>       | <span data-ttu-id="15d15-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15d15-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="15d15-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="15d15-118">Authorization</span></span>  | <span data-ttu-id="15d15-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15d15-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15d15-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15d15-121">Request body</span></span>
<span data-ttu-id="15d15-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="15d15-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="15d15-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15d15-125">Property</span></span>     | <span data-ttu-id="15d15-126">Typ</span><span class="sxs-lookup"><span data-stu-id="15d15-126">Type</span></span>   |<span data-ttu-id="15d15-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15d15-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15d15-128">columnWidth</span><span class="sxs-lookup"><span data-stu-id="15d15-128">columnWidth</span></span>|<span data-ttu-id="15d15-129">double</span><span class="sxs-lookup"><span data-stu-id="15d15-129">double</span></span>|<span data-ttu-id="15d15-p104">Ruft die Breite aller Spalten innerhalb des Bereichs ab oder legt diese fest. Wenn die Breite der Spalten nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15d15-p104">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="15d15-132">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="15d15-132">horizontalAlignment</span></span>|<span data-ttu-id="15d15-133">string</span><span class="sxs-lookup"><span data-stu-id="15d15-133">string</span></span>|<span data-ttu-id="15d15-p105">Stellt die horizontale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="15d15-p105">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="15d15-136">rowHeight</span><span class="sxs-lookup"><span data-stu-id="15d15-136">rowHeight</span></span>|<span data-ttu-id="15d15-137">double</span><span class="sxs-lookup"><span data-stu-id="15d15-137">double</span></span>|<span data-ttu-id="15d15-p106">Ruft die Höhe aller Zeilen des Bereichs ab oder legt diese fest. Wenn die Höhe der Zeilen nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15d15-p106">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="15d15-140">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="15d15-140">verticalAlignment</span></span>|<span data-ttu-id="15d15-141">string</span><span class="sxs-lookup"><span data-stu-id="15d15-141">string</span></span>|<span data-ttu-id="15d15-p107">Stellt die vertikale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="15d15-p107">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="15d15-144">wrapText</span><span class="sxs-lookup"><span data-stu-id="15d15-144">wrapText</span></span>|<span data-ttu-id="15d15-145">boolean</span><span class="sxs-lookup"><span data-stu-id="15d15-145">boolean</span></span>|<span data-ttu-id="15d15-p108">Gibt an, ob Excel den Text im Objekt umbricht. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Textumbruch-Einstellung hat</span><span class="sxs-lookup"><span data-stu-id="15d15-p108">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="15d15-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="15d15-148">Response</span></span>

<span data-ttu-id="15d15-149">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [RangeFormat](../resources/rangeformat.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15d15-149">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15d15-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15d15-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15d15-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15d15-151">Request</span></span>
<span data-ttu-id="15d15-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15d15-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
}
```
##### <a name="response"></a><span data-ttu-id="15d15-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="15d15-153">Response</span></span>
<span data-ttu-id="15d15-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15d15-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 96

{
  "columnWidth": 99,
  "horizontalAlignment": "horizontalAlignment-value",
  "rowHeight": 99
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