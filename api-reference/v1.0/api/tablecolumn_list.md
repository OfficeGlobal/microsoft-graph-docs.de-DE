# <a name="list-tablecolumncollection"></a><span data-ttu-id="9227d-101">TableColumnCollection auflisten</span><span class="sxs-lookup"><span data-stu-id="9227d-101">List TableColumnCollection</span></span>

<span data-ttu-id="9227d-102">Dient zum Abrufen einer Liste von tablecolumn-Objekten.</span><span class="sxs-lookup"><span data-stu-id="9227d-102">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="9227d-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9227d-103">Permissions</span></span>
<span data-ttu-id="9227d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9227d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9227d-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9227d-106">Permission type</span></span>      | <span data-ttu-id="9227d-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9227d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9227d-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9227d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9227d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9227d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9227d-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9227d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9227d-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9227d-111">Not supported.</span></span>    |
|<span data-ttu-id="9227d-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9227d-112">Application</span></span> | <span data-ttu-id="9227d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9227d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9227d-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9227d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9227d-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9227d-115">Optional query parameters</span></span>
<span data-ttu-id="9227d-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9227d-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9227d-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9227d-117">Request headers</span></span>
| <span data-ttu-id="9227d-118">Name</span><span class="sxs-lookup"><span data-stu-id="9227d-118">Name</span></span>      |<span data-ttu-id="9227d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9227d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9227d-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9227d-120">Authorization</span></span>  | <span data-ttu-id="9227d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9227d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9227d-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="9227d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9227d-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="9227d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9227d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9227d-126">Request body</span></span>
<span data-ttu-id="9227d-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9227d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9227d-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9227d-128">Response</span></span>

<span data-ttu-id="9227d-129">Wenn erfolgreich, gibt diese Methode einen `200 OK` Antwortcode und eine Sammlung von [WorkbookTableColumn](../resources/tablecolumn.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9227d-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9227d-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9227d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9227d-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9227d-131">Request</span></span>
<span data-ttu-id="9227d-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9227d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecolumncollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
```
##### <a name="response"></a><span data-ttu-id="9227d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9227d-133">Response</span></span>
<span data-ttu-id="9227d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9227d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableColumnCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->