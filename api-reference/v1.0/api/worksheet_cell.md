# <a name="worksheet-cell"></a><span data-ttu-id="82abf-101">Arbeitsblatt: Zelle</span><span class="sxs-lookup"><span data-stu-id="82abf-101">Worksheet: Cell</span></span>

<span data-ttu-id="82abf-p101">Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb ihres übergeordneten Bereichs befinden, solange sie im Arbeitsblattraster bleibt.</span><span class="sxs-lookup"><span data-stu-id="82abf-p101">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="82abf-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="82abf-104">Permissions</span></span>
<span data-ttu-id="82abf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="82abf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="82abf-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="82abf-107">Permission type</span></span>      | <span data-ttu-id="82abf-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="82abf-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82abf-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="82abf-109">Delegated (work or school account)</span></span> | <span data-ttu-id="82abf-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82abf-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="82abf-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="82abf-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82abf-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82abf-112">Not supported.</span></span>    |
|<span data-ttu-id="82abf-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="82abf-113">Application</span></span> | <span data-ttu-id="82abf-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82abf-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82abf-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="82abf-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/cell(row=<row>,column=<column>)

```
## <a name="request-headers"></a><span data-ttu-id="82abf-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="82abf-116">Request headers</span></span>
| <span data-ttu-id="82abf-117">Name</span><span class="sxs-lookup"><span data-stu-id="82abf-117">Name</span></span>       | <span data-ttu-id="82abf-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82abf-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="82abf-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="82abf-119">Authorization</span></span>  | <span data-ttu-id="82abf-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="82abf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="82abf-122">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="82abf-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="82abf-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="82abf-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="82abf-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="82abf-125">Parameters</span></span>
<span data-ttu-id="82abf-126">Geben Sie im Anforderungspfad die folgenden Parameter an.</span><span class="sxs-lookup"><span data-stu-id="82abf-126">In the request URL, provide the following query parameters with values.</span></span>

| <span data-ttu-id="82abf-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="82abf-127">Parameter</span></span>    | <span data-ttu-id="82abf-128">Typ</span><span class="sxs-lookup"><span data-stu-id="82abf-128">Type</span></span>   |<span data-ttu-id="82abf-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82abf-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82abf-130">Zeile</span><span class="sxs-lookup"><span data-stu-id="82abf-130">row</span></span>|<span data-ttu-id="82abf-131">Int32</span><span class="sxs-lookup"><span data-stu-id="82abf-131">Int32</span></span>|<span data-ttu-id="82abf-p105">Zeilenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="82abf-p105">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="82abf-134">Spalte</span><span class="sxs-lookup"><span data-stu-id="82abf-134">column</span></span>|<span data-ttu-id="82abf-135">Int32</span><span class="sxs-lookup"><span data-stu-id="82abf-135">Int32</span></span>|<span data-ttu-id="82abf-p106">Spaltenanzahl der abzurufenden Zelle. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="82abf-p106">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="82abf-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="82abf-138">Response</span></span>

<span data-ttu-id="82abf-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82abf-139">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82abf-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="82abf-140">Example</span></span>
<span data-ttu-id="82abf-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="82abf-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="82abf-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="82abf-142">Request</span></span>
<span data-ttu-id="82abf-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="82abf-143">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="82abf-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="82abf-144">Response</span></span>
<span data-ttu-id="82abf-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82abf-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
