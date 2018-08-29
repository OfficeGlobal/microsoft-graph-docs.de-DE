# <a name="tablerow-range"></a><span data-ttu-id="48d99-101">TableRow: Range</span><span class="sxs-lookup"><span data-stu-id="48d99-101">TableRow: Range</span></span>

<span data-ttu-id="48d99-102">Ruft das Bereichsobjekt ab, das mit der gesamten Zeile verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="48d99-102">Returns the range object associated with the entire row.</span></span>
## <a name="permissions"></a><span data-ttu-id="48d99-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="48d99-103">Permissions</span></span>
<span data-ttu-id="48d99-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="48d99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="48d99-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48d99-106">Permission type</span></span>      | <span data-ttu-id="48d99-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48d99-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48d99-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48d99-108">Delegated (work or school account)</span></span> | <span data-ttu-id="48d99-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48d99-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="48d99-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48d99-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48d99-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48d99-111">Not supported.</span></span>    |
|<span data-ttu-id="48d99-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48d99-112">Application</span></span> | <span data-ttu-id="48d99-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48d99-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48d99-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48d99-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows/{index}/range
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/range

```
## <a name="request-headers"></a><span data-ttu-id="48d99-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48d99-115">Request headers</span></span>
| <span data-ttu-id="48d99-116">Name</span><span class="sxs-lookup"><span data-stu-id="48d99-116">Name</span></span>       | <span data-ttu-id="48d99-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48d99-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="48d99-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="48d99-118">Authorization</span></span>  | <span data-ttu-id="48d99-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48d99-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="48d99-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="48d99-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="48d99-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="48d99-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48d99-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48d99-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="48d99-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="48d99-125">Response</span></span>

<span data-ttu-id="48d99-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48d99-126">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48d99-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48d99-127">Example</span></span>
<span data-ttu-id="48d99-128">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="48d99-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="48d99-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48d99-129">Request</span></span>
<span data-ttu-id="48d99-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48d99-130">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablerow_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/range
```

##### <a name="response"></a><span data-ttu-id="48d99-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="48d99-131">Response</span></span>
<span data-ttu-id="48d99-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48d99-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableRow: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->