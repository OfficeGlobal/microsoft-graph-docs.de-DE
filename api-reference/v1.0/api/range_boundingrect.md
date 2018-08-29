# <a name="range-boundingrect"></a><span data-ttu-id="1b80a-101">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="1b80a-101">Range: BoundingRect</span></span>

<span data-ttu-id="1b80a-p101">Ruft das kleinste Bereichsobjekt ab, das die angegebenen Bereiche umfasst. Beispielsweise das GetBoundingRect von "B2:C5" und "D10:E15" lautet "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="1b80a-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="1b80a-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1b80a-104">Permissions</span></span>
<span data-ttu-id="1b80a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1b80a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1b80a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1b80a-107">Permission type</span></span>      | <span data-ttu-id="1b80a-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1b80a-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b80a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1b80a-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1b80a-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b80a-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1b80a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1b80a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b80a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b80a-112">Not supported.</span></span>    |
|<span data-ttu-id="1b80a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1b80a-113">Application</span></span> | <span data-ttu-id="1b80a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b80a-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b80a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b80a-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/boundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/boundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/boundingRect

```
## <a name="request-headers"></a><span data-ttu-id="1b80a-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1b80a-116">Request headers</span></span>
| <span data-ttu-id="1b80a-117">Name</span><span class="sxs-lookup"><span data-stu-id="1b80a-117">Name</span></span>       | <span data-ttu-id="1b80a-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b80a-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1b80a-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1b80a-119">Authorization</span></span>  | <span data-ttu-id="1b80a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1b80a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1b80a-122">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="1b80a-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="1b80a-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="1b80a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b80a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1b80a-125">Request body</span></span>
<span data-ttu-id="1b80a-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="1b80a-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1b80a-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="1b80a-127">Parameter</span></span>    | <span data-ttu-id="1b80a-128">Typ</span><span class="sxs-lookup"><span data-stu-id="1b80a-128">Type</span></span>   |<span data-ttu-id="1b80a-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b80a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b80a-130">anotherRange</span><span class="sxs-lookup"><span data-stu-id="1b80a-130">anotherRange</span></span>|<span data-ttu-id="1b80a-131">string</span><span class="sxs-lookup"><span data-stu-id="1b80a-131">string</span></span>|<span data-ttu-id="1b80a-132">Das Bereichsobjekt oder die Adresse oder der Bereichsname.</span><span class="sxs-lookup"><span data-stu-id="1b80a-132">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="1b80a-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b80a-133">Response</span></span>

<span data-ttu-id="1b80a-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b80a-134">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b80a-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1b80a-135">Example</span></span>
<span data-ttu-id="1b80a-136">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="1b80a-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1b80a-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b80a-137">Request</span></span>
<span data-ttu-id="1b80a-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1b80a-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/boundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="1b80a-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b80a-139">Response</span></span>
<span data-ttu-id="1b80a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b80a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->