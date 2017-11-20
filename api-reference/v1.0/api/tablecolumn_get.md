# <a name="get-tablecolumn"></a><span data-ttu-id="0c745-101">TableColumn abrufen</span><span class="sxs-lookup"><span data-stu-id="0c745-101">Get TableColumn</span></span>

<span data-ttu-id="0c745-102">Dient zum Abrufen der Eigenschaften und der Beziehungen des tableColumn-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c745-102">Retrieve the properties and relationships of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c745-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0c745-103">Permissions</span></span>
<span data-ttu-id="0c745-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0c745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0c745-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0c745-106">Permission type</span></span>      | <span data-ttu-id="0c745-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0c745-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c745-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0c745-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0c745-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c745-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0c745-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0c745-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c745-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c745-111">Not supported.</span></span>    |
|<span data-ttu-id="0c745-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0c745-112">Application</span></span> | <span data-ttu-id="0c745-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c745-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c745-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c745-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns/{id|name}
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0c745-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0c745-115">Optional query parameters</span></span>
<span data-ttu-id="0c745-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0c745-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c745-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0c745-117">Request headers</span></span>
| <span data-ttu-id="0c745-118">Name</span><span class="sxs-lookup"><span data-stu-id="0c745-118">Name</span></span>      |<span data-ttu-id="0c745-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c745-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0c745-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c745-120">Authorization</span></span>  | <span data-ttu-id="0c745-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0c745-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c745-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="0c745-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0c745-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="0c745-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c745-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0c745-126">Request body</span></span>
<span data-ttu-id="0c745-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0c745-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c745-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c745-128">Response</span></span>

<span data-ttu-id="0c745-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [TableColumn](../resources/tablecolumn.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c745-129">If successful, this method returns a `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0c745-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0c745-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c745-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c745-131">Request</span></span>
<span data-ttu-id="0c745-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0c745-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecolumn"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
```
##### <a name="response"></a><span data-ttu-id="0c745-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c745-133">Response</span></span>
<span data-ttu-id="0c745-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c745-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->