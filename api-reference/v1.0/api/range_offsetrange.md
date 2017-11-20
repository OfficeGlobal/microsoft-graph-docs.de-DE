# <a name="range-offsetrange"></a><span data-ttu-id="fa805-101">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="fa805-101">Range: OffsetRange</span></span>

<span data-ttu-id="fa805-p101">Ruft ein Objekt ab, das einen Bereich darstellt, der aus dem angegebenen Bereich versetzt ist. Die Dimension des zurückgegebenen Bereichs entspricht diesem Bereich. Wenn der resultierende Bereich außerhalb des Arbeitsblatt-Rasters erzwungen wird, wird eine Ausnahme ausgelöst.</span><span class="sxs-lookup"><span data-stu-id="fa805-p101">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa805-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fa805-105">Permissions</span></span>
<span data-ttu-id="fa805-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa805-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fa805-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa805-108">Permission type</span></span>      | <span data-ttu-id="fa805-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa805-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa805-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa805-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa805-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa805-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fa805-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa805-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa805-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa805-113">Not supported.</span></span>    |
|<span data-ttu-id="fa805-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa805-114">Application</span></span> | <span data-ttu-id="fa805-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa805-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa805-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa805-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="fa805-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa805-117">Request headers</span></span>
| <span data-ttu-id="fa805-118">Name</span><span class="sxs-lookup"><span data-stu-id="fa805-118">Name</span></span>       | <span data-ttu-id="fa805-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa805-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fa805-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa805-120">Authorization</span></span>  | <span data-ttu-id="fa805-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fa805-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa805-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="fa805-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fa805-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="fa805-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa805-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa805-126">Request body</span></span>
<span data-ttu-id="fa805-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="fa805-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fa805-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="fa805-128">Parameter</span></span>    | <span data-ttu-id="fa805-129">Typ</span><span class="sxs-lookup"><span data-stu-id="fa805-129">Type</span></span>   |<span data-ttu-id="fa805-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa805-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa805-131">rowOffset</span><span class="sxs-lookup"><span data-stu-id="fa805-131">rowOffset</span></span>|<span data-ttu-id="fa805-132">number</span><span class="sxs-lookup"><span data-stu-id="fa805-132">number</span></span>|<span data-ttu-id="fa805-p105">Die Anzahl an Zeilen (positiv, negativ oder 0), um die der Bereich versetzt werden muss. Bei positiven Werten wird der Bereich nach unten versetzt. Bei negativen Werten wird der Bereich nach oben versetzt.</span><span class="sxs-lookup"><span data-stu-id="fa805-p105">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="fa805-135">columnOffset</span><span class="sxs-lookup"><span data-stu-id="fa805-135">columnOffset</span></span>|<span data-ttu-id="fa805-136">number</span><span class="sxs-lookup"><span data-stu-id="fa805-136">number</span></span>|<span data-ttu-id="fa805-p106">Die Anzahl an Spalten (positiv, negativ oder 0), um die der Bereich versetzt werden muss. Bei positiven Werten wird der Bereich nach unten versetzt. Bei negativen Werten wird der Bereich nach oben versetzt.</span><span class="sxs-lookup"><span data-stu-id="fa805-p106">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="fa805-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa805-139">Response</span></span>

<span data-ttu-id="fa805-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa805-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa805-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa805-141">Example</span></span>
<span data-ttu-id="fa805-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="fa805-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fa805-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa805-143">Request</span></span>
<span data-ttu-id="fa805-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa805-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="fa805-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa805-145">Response</span></span>
<span data-ttu-id="fa805-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa805-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->