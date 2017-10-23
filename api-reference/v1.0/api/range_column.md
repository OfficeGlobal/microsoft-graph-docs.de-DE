# <a name="range-column"></a><span data-ttu-id="a2859-101">Range: Column</span><span class="sxs-lookup"><span data-stu-id="a2859-101">Range: Column</span></span>

<span data-ttu-id="a2859-102">Ruft eine Spalte ab, die im Bereich enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="a2859-102">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="a2859-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a2859-103">Permissions</span></span>
<span data-ttu-id="a2859-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a2859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a2859-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2859-106">Permission type</span></span>      | <span data-ttu-id="a2859-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2859-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2859-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2859-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a2859-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2859-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a2859-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2859-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2859-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2859-111">Not supported.</span></span>    |
|<span data-ttu-id="a2859-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2859-112">Application</span></span> | <span data-ttu-id="a2859-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2859-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2859-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2859-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Column
GET /workbook/worksheets/{id|name}/range(<address>)/Column
GET /workbook/tables/{id|name}/columns/{id|name}/range/Column

```
## <a name="request-headers"></a><span data-ttu-id="a2859-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2859-115">Request headers</span></span>
| <span data-ttu-id="a2859-116">Name</span><span class="sxs-lookup"><span data-stu-id="a2859-116">Name</span></span>       | <span data-ttu-id="a2859-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2859-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a2859-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2859-118">Authorization</span></span>  | <span data-ttu-id="a2859-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a2859-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2859-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a2859-121">Request body</span></span>
<span data-ttu-id="a2859-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="a2859-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a2859-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="a2859-123">Parameter</span></span>    | <span data-ttu-id="a2859-124">Typ</span><span class="sxs-lookup"><span data-stu-id="a2859-124">Type</span></span>   |<span data-ttu-id="a2859-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2859-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2859-126">column</span><span class="sxs-lookup"><span data-stu-id="a2859-126">column</span></span>|<span data-ttu-id="a2859-127">number</span><span class="sxs-lookup"><span data-stu-id="a2859-127">number</span></span>|<span data-ttu-id="a2859-p103">Spaltenanzahl des abzurufenden Bereichs. Nullindiziert.</span><span class="sxs-lookup"><span data-stu-id="a2859-p103">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="a2859-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2859-130">Response</span></span>

<span data-ttu-id="a2859-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2859-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2859-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2859-132">Example</span></span>
<span data-ttu-id="a2859-133">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="a2859-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a2859-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2859-134">Request</span></span>
<span data-ttu-id="a2859-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2859-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/Column
Content-type: application/json
Content-length: 21

{
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="a2859-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2859-136">Response</span></span>
<span data-ttu-id="a2859-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2859-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->