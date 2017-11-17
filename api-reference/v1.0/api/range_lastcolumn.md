# <a name="range-lastcolumn"></a><span data-ttu-id="866b3-101">Range: LastColumn</span><span class="sxs-lookup"><span data-stu-id="866b3-101">Range: LastColumn</span></span>

<span data-ttu-id="866b3-p101">Ruft die letzte Spalte im Bereich ab. Beispielsweise lautet die letzte Spalte von „B2:D5“ „D2:D5“.</span><span class="sxs-lookup"><span data-stu-id="866b3-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="866b3-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="866b3-104">Permissions</span></span>
<span data-ttu-id="866b3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="866b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="866b3-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="866b3-107">Permission type</span></span>      | <span data-ttu-id="866b3-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="866b3-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="866b3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="866b3-109">Delegated (work or school account)</span></span> | <span data-ttu-id="866b3-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="866b3-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="866b3-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="866b3-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="866b3-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="866b3-112">Not supported.</span></span>    |
|<span data-ttu-id="866b3-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="866b3-113">Application</span></span> | <span data-ttu-id="866b3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="866b3-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="866b3-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="866b3-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastColumn

```
## <a name="request-headers"></a><span data-ttu-id="866b3-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="866b3-116">Request headers</span></span>
| <span data-ttu-id="866b3-117">Name</span><span class="sxs-lookup"><span data-stu-id="866b3-117">Name</span></span>       | <span data-ttu-id="866b3-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="866b3-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="866b3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="866b3-119">Authorization</span></span>  | <span data-ttu-id="866b3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="866b3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="866b3-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="866b3-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="866b3-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="866b3-123">Response</span></span>

<span data-ttu-id="866b3-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="866b3-124">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="866b3-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="866b3-125">Example</span></span>
<span data-ttu-id="866b3-126">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="866b3-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="866b3-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="866b3-127">Request</span></span>
<span data-ttu-id="866b3-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="866b3-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastcolumn"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/LastColumn
```

##### <a name="response"></a><span data-ttu-id="866b3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="866b3-129">Response</span></span>
<span data-ttu-id="866b3-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="866b3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->