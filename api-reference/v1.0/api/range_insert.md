# <a name="range-insert"></a><span data-ttu-id="c6219-101">Bereich: Einfügen</span><span class="sxs-lookup"><span data-stu-id="c6219-101">Range: insert</span></span>

<span data-ttu-id="c6219-p101">Fügt eine Zelle oder einen Zellbereich in das Arbeitsblatt anstelle dieses Bereichs ein, und verschiebt die anderen Zellen, um Platz zu schaffen. Gibt ein neues Bereichsobjekt in dem nun leeren Bereich zurück.</span><span class="sxs-lookup"><span data-stu-id="c6219-p101">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6219-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c6219-104">Permissions</span></span>
<span data-ttu-id="c6219-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c6219-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c6219-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c6219-107">Permission type</span></span>      | <span data-ttu-id="c6219-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c6219-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6219-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c6219-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c6219-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6219-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c6219-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c6219-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6219-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6219-112">Not supported.</span></span>    |
|<span data-ttu-id="c6219-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c6219-113">Application</span></span> | <span data-ttu-id="c6219-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6219-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6219-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6219-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="c6219-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c6219-116">Request headers</span></span>
| <span data-ttu-id="c6219-117">Name</span><span class="sxs-lookup"><span data-stu-id="c6219-117">Name</span></span>       | <span data-ttu-id="c6219-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6219-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c6219-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c6219-119">Authorization</span></span>  | <span data-ttu-id="c6219-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c6219-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c6219-122">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c6219-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="c6219-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c6219-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6219-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c6219-125">Request body</span></span>
<span data-ttu-id="c6219-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c6219-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c6219-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="c6219-127">Parameter</span></span>    | <span data-ttu-id="c6219-128">Typ</span><span class="sxs-lookup"><span data-stu-id="c6219-128">Type</span></span>   |<span data-ttu-id="c6219-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6219-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6219-130">Shift</span><span class="sxs-lookup"><span data-stu-id="c6219-130">shift</span></span>|<span data-ttu-id="c6219-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6219-131">string</span></span>|<span data-ttu-id="c6219-132">Gibt an, in welche Richtung die Zellen verschoben werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c6219-132">Specifies which way to shift the cells.  Possible values are: Down, Right</span></span>  <span data-ttu-id="c6219-133">Die möglichen Werte sind: `Down`, `Right`.</span><span class="sxs-lookup"><span data-stu-id="c6219-133">The possible values are:</span></span>|

## <a name="response"></a><span data-ttu-id="c6219-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6219-134">Response</span></span>

<span data-ttu-id="c6219-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c6219-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6219-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c6219-136">Example</span></span>
<span data-ttu-id="c6219-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c6219-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c6219-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6219-138">Request</span></span>
<span data-ttu-id="c6219-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c6219-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="c6219-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6219-140">Response</span></span>
<span data-ttu-id="c6219-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c6219-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->