# <a name="worksheet-cell"></a><span data-ttu-id="8df48-101">Arbeitsblatt: Zelle</span><span class="sxs-lookup"><span data-stu-id="8df48-101">Worksheet: Cell</span></span>

<span data-ttu-id="8df48-p101">Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb ihres übergeordneten Bereichs befinden, solange sie im Arbeitsblattraster bleibt.</span><span class="sxs-lookup"><span data-stu-id="8df48-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="8df48-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8df48-104">Permissions</span></span>
<span data-ttu-id="8df48-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8df48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8df48-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8df48-107">Permission type</span></span>      | <span data-ttu-id="8df48-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8df48-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8df48-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8df48-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8df48-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8df48-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8df48-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8df48-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8df48-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8df48-112">Not supported.</span></span>    |
|<span data-ttu-id="8df48-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8df48-113">Application</span></span> | <span data-ttu-id="8df48-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8df48-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8df48-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8df48-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="8df48-116">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="8df48-116">Function parameters</span></span>
<span data-ttu-id="8df48-117">Geben Sie im Anforderungspfad die folgenden Parameter an.</span><span class="sxs-lookup"><span data-stu-id="8df48-117">In the request URL, provide the following query parameters with values.</span></span>

| <span data-ttu-id="8df48-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="8df48-118">Parameter</span></span>    | <span data-ttu-id="8df48-119">Typ</span><span class="sxs-lookup"><span data-stu-id="8df48-119">Type</span></span>   |<span data-ttu-id="8df48-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8df48-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8df48-121">Zeile</span><span class="sxs-lookup"><span data-stu-id="8df48-121">row</span></span>|<span data-ttu-id="8df48-122">Int32</span><span class="sxs-lookup"><span data-stu-id="8df48-122">Int32</span></span>|<span data-ttu-id="8df48-p103">Zeilenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="8df48-p103">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="8df48-125">Spalte</span><span class="sxs-lookup"><span data-stu-id="8df48-125">column</span></span>|<span data-ttu-id="8df48-126">Int32</span><span class="sxs-lookup"><span data-stu-id="8df48-126">Int32</span></span>|<span data-ttu-id="8df48-p104">Spaltenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="8df48-p104">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="8df48-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8df48-129">Request headers</span></span>
| <span data-ttu-id="8df48-130">Name</span><span class="sxs-lookup"><span data-stu-id="8df48-130">Name</span></span>       | <span data-ttu-id="8df48-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8df48-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8df48-132">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8df48-132">Authorization</span></span>  | <span data-ttu-id="8df48-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8df48-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8df48-135">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="8df48-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="8df48-p106">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="8df48-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8df48-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8df48-138">Request body</span></span>
<span data-ttu-id="8df48-139">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8df48-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8df48-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="8df48-140">Response</span></span>

<span data-ttu-id="8df48-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8df48-141">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8df48-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8df48-142">Example</span></span>
<span data-ttu-id="8df48-143">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8df48-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8df48-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8df48-144">Request</span></span>
<span data-ttu-id="8df48-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8df48-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="8df48-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="8df48-146">Response</span></span>
<span data-ttu-id="8df48-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8df48-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 1,
  "columnCount": 1,
  "columnIndex": 3,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
