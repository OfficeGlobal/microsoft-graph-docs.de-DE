# <a name="range-usedrange"></a><span data-ttu-id="2e04c-101">Spanne: UsedRange</span><span class="sxs-lookup"><span data-stu-id="2e04c-101">Range: UsedRange</span></span>

<span data-ttu-id="2e04c-102">Gibt den verwendeten Bereich des angegebenen Bereichsobjekts zurück.</span><span class="sxs-lookup"><span data-stu-id="2e04c-102">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e04c-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2e04c-103">Permissions</span></span>
<span data-ttu-id="2e04c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e04c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2e04c-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e04c-106">Permission type</span></span>      | <span data-ttu-id="2e04c-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e04c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e04c-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e04c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2e04c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e04c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2e04c-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e04c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e04c-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e04c-111">Not supported.</span></span>    |
|<span data-ttu-id="2e04c-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e04c-112">Application</span></span> | <span data-ttu-id="2e04c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e04c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e04c-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e04c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="2e04c-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e04c-115">Request headers</span></span>
| <span data-ttu-id="2e04c-116">Name</span><span class="sxs-lookup"><span data-stu-id="2e04c-116">Name</span></span>       | <span data-ttu-id="2e04c-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e04c-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2e04c-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2e04c-118">Authorization</span></span>  | <span data-ttu-id="2e04c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2e04c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2e04c-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="2e04c-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="2e04c-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="2e04c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="2e04c-124">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="2e04c-124">Path parameters</span></span>
| <span data-ttu-id="2e04c-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="2e04c-125">Parameter</span></span>    | <span data-ttu-id="2e04c-126">Typ</span><span class="sxs-lookup"><span data-stu-id="2e04c-126">Type</span></span>   |<span data-ttu-id="2e04c-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e04c-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e04c-128">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="2e04c-128">valuesOnly</span></span>|<span data-ttu-id="2e04c-129">boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2e04c-129">boolean</span></span>|<span data-ttu-id="2e04c-p104">Optional. Betrachtet nur Zellen mit Werten als verwendet.</span><span class="sxs-lookup"><span data-stu-id="2e04c-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="2e04c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e04c-132">Response</span></span>

<span data-ttu-id="2e04c-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e04c-133">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e04c-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e04c-134">Example</span></span>
<span data-ttu-id="2e04c-135">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2e04c-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2e04c-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e04c-136">Request</span></span>
<span data-ttu-id="2e04c-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e04c-137">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```

##### <a name="response"></a><span data-ttu-id="2e04c-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e04c-138">Response</span></span>
<span data-ttu-id="2e04c-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e04c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="2e04c-142">Es folgt ein Beispiel, das die optionalen `valuesOnly` Parameter angibt.</span><span class="sxs-lookup"><span data-stu-id="2e04c-142">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="2e04c-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e04c-143">Request</span></span>
<span data-ttu-id="2e04c-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e04c-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="2e04c-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e04c-145">Response</span></span>

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
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->