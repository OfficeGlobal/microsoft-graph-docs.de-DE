# <a name="range-lastrow"></a><span data-ttu-id="c7881-101">Range: LastRow</span><span class="sxs-lookup"><span data-stu-id="c7881-101">Range: LastRow</span></span>

<span data-ttu-id="c7881-p101">Ruft die letzte Zeile im Bereich ab. Beispielsweise lautet die letzte Zelle des Bereichs "B2: D5" "B5:D5".</span><span class="sxs-lookup"><span data-stu-id="c7881-p101">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="c7881-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c7881-104">Permissions</span></span>
<span data-ttu-id="c7881-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7881-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c7881-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c7881-107">Permission type</span></span>      | <span data-ttu-id="c7881-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c7881-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7881-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c7881-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c7881-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7881-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c7881-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c7881-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7881-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7881-112">Not supported.</span></span>    |
|<span data-ttu-id="c7881-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c7881-113">Application</span></span> | <span data-ttu-id="c7881-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7881-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7881-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7881-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastRow

```
## <a name="request-headers"></a><span data-ttu-id="c7881-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c7881-116">Request headers</span></span>
| <span data-ttu-id="c7881-117">Name</span><span class="sxs-lookup"><span data-stu-id="c7881-117">Name</span></span>       | <span data-ttu-id="c7881-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7881-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c7881-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7881-119">Authorization</span></span>  | <span data-ttu-id="c7881-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c7881-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7881-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c7881-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c7881-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7881-123">Response</span></span>

<span data-ttu-id="c7881-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7881-124">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7881-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c7881-125">Example</span></span>
<span data-ttu-id="c7881-126">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c7881-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c7881-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7881-127">Request</span></span>
<span data-ttu-id="c7881-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c7881-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/LastRow
```

##### <a name="response"></a><span data-ttu-id="c7881-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7881-129">Response</span></span>
<span data-ttu-id="c7881-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7881-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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