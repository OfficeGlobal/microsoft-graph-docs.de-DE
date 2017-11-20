# <a name="range-lastrow"></a><span data-ttu-id="fe315-101">Range: LastRow</span><span class="sxs-lookup"><span data-stu-id="fe315-101">Range: LastRow</span></span>

<span data-ttu-id="fe315-p101">Ruft die letzte Zeile im Bereich ab. Beispielsweise lautet die letzte Zelle des Bereichs "B2: D5" "B5:D5".</span><span class="sxs-lookup"><span data-stu-id="fe315-p101">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="fe315-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fe315-104">Permissions</span></span>
<span data-ttu-id="fe315-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe315-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fe315-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fe315-107">Permission type</span></span>      | <span data-ttu-id="fe315-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fe315-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe315-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fe315-109">Delegated (work or school account)</span></span> | <span data-ttu-id="fe315-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe315-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fe315-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fe315-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe315-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe315-112">Not supported.</span></span>    |
|<span data-ttu-id="fe315-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fe315-113">Application</span></span> | <span data-ttu-id="fe315-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe315-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe315-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe315-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastRow

```
## <a name="request-headers"></a><span data-ttu-id="fe315-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fe315-116">Request headers</span></span>
| <span data-ttu-id="fe315-117">Name</span><span class="sxs-lookup"><span data-stu-id="fe315-117">Name</span></span>       | <span data-ttu-id="fe315-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe315-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fe315-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe315-119">Authorization</span></span>  | <span data-ttu-id="fe315-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fe315-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe315-122">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="fe315-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="fe315-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="fe315-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe315-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fe315-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="fe315-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe315-126">Response</span></span>

<span data-ttu-id="fe315-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe315-127">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe315-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fe315-128">Example</span></span>
<span data-ttu-id="fe315-129">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="fe315-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fe315-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe315-130">Request</span></span>
<span data-ttu-id="fe315-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fe315-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/LastRow
```

##### <a name="response"></a><span data-ttu-id="fe315-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe315-132">Response</span></span>
<span data-ttu-id="fe315-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe315-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->