# <a name="range-column"></a><span data-ttu-id="6e230-101">Bereich: Spalte</span><span class="sxs-lookup"><span data-stu-id="6e230-101">Range: Column</span></span>

<span data-ttu-id="6e230-102">Ruft eine Spalte ab, die im Bereich enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="6e230-102">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="6e230-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6e230-103">Permissions</span></span>
<span data-ttu-id="6e230-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6e230-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6e230-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6e230-106">Permission type</span></span>      | <span data-ttu-id="6e230-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6e230-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e230-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6e230-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6e230-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e230-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6e230-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6e230-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e230-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e230-111">Not supported.</span></span>    |
|<span data-ttu-id="6e230-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6e230-112">Application</span></span> | <span data-ttu-id="6e230-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e230-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e230-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e230-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="6e230-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6e230-115">Request headers</span></span>
| <span data-ttu-id="6e230-116">Name</span><span class="sxs-lookup"><span data-stu-id="6e230-116">Name</span></span>       | <span data-ttu-id="6e230-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e230-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6e230-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6e230-118">Authorization</span></span>  | <span data-ttu-id="6e230-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e230-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6e230-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="6e230-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="6e230-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="6e230-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="6e230-124">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="6e230-124">Path parameters</span></span>
<span data-ttu-id="6e230-125">Geben Sie im Anforderungspfad die folgenden Parameter an.</span><span class="sxs-lookup"><span data-stu-id="6e230-125">In the request URL, provide the following query parameters with values.</span></span>

| <span data-ttu-id="6e230-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="6e230-126">Parameter</span></span>    | <span data-ttu-id="6e230-127">Typ</span><span class="sxs-lookup"><span data-stu-id="6e230-127">Type</span></span>   |<span data-ttu-id="6e230-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e230-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e230-129">Spalte</span><span class="sxs-lookup"><span data-stu-id="6e230-129">column</span></span>|<span data-ttu-id="6e230-130">Int32</span><span class="sxs-lookup"><span data-stu-id="6e230-130">Int32</span></span>|<span data-ttu-id="6e230-p104">Spaltenanzahl des abzurufenden Bereichs. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="6e230-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="6e230-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e230-133">Response</span></span>

<span data-ttu-id="6e230-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6e230-134">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e230-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6e230-135">Example</span></span>
<span data-ttu-id="6e230-136">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="6e230-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6e230-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e230-137">Request</span></span>
<span data-ttu-id="6e230-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6e230-138">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```

##### <a name="response"></a><span data-ttu-id="6e230-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e230-139">Response</span></span>
<span data-ttu-id="6e230-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6e230-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->