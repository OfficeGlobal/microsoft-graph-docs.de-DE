# <a name="range-cell"></a><span data-ttu-id="96385-101">Range: Cell</span><span class="sxs-lookup"><span data-stu-id="96385-101">Range: Cell</span></span>

<span data-ttu-id="96385-p101">Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb seines übergeordneten Bereichs befinden, solange es im Arbeitsblatt-Raster bleibt. Die zurückgegebene Zelle befindet sich relativ zur obersten linken Zelle des Bereichs.</span><span class="sxs-lookup"><span data-stu-id="96385-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="96385-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="96385-105">Permissions</span></span>
<span data-ttu-id="96385-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="96385-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="96385-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96385-108">Permission type</span></span>      | <span data-ttu-id="96385-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96385-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96385-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96385-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96385-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96385-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96385-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96385-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96385-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96385-113">Not supported.</span></span>    |
|<span data-ttu-id="96385-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96385-114">Application</span></span> | <span data-ttu-id="96385-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96385-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96385-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96385-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="96385-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96385-117">Request headers</span></span>
| <span data-ttu-id="96385-118">Name</span><span class="sxs-lookup"><span data-stu-id="96385-118">Name</span></span>       | <span data-ttu-id="96385-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96385-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96385-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="96385-120">Authorization</span></span>  | <span data-ttu-id="96385-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="96385-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96385-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="96385-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="96385-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="96385-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96385-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96385-126">Request body</span></span>
<span data-ttu-id="96385-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="96385-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="96385-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="96385-128">Parameter</span></span>    | <span data-ttu-id="96385-129">Typ</span><span class="sxs-lookup"><span data-stu-id="96385-129">Type</span></span>   |<span data-ttu-id="96385-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96385-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96385-131">row</span><span class="sxs-lookup"><span data-stu-id="96385-131">row</span></span>|<span data-ttu-id="96385-132">number</span><span class="sxs-lookup"><span data-stu-id="96385-132">number</span></span>|<span data-ttu-id="96385-p105">Zeilenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="96385-p105">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="96385-135">Spalte</span><span class="sxs-lookup"><span data-stu-id="96385-135">column</span></span>|<span data-ttu-id="96385-136">number</span><span class="sxs-lookup"><span data-stu-id="96385-136">number</span></span>|<span data-ttu-id="96385-p106">Spaltenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="96385-p106">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="96385-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="96385-139">Response</span></span>

<span data-ttu-id="96385-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96385-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96385-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96385-141">Example</span></span>
<span data-ttu-id="96385-142">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="96385-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="96385-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96385-143">Request</span></span>
<span data-ttu-id="96385-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96385-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Cell
Content-type: application/json
Content-length: 37

{
  "row": {
  },
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="96385-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="96385-145">Response</span></span>
<span data-ttu-id="96385-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96385-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->