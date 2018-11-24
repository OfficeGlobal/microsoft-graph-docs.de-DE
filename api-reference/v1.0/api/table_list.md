# <a name="list-tablecollection"></a><span data-ttu-id="52341-101">TableCollection auflisten</span><span class="sxs-lookup"><span data-stu-id="52341-101">List TableCollection</span></span>

<span data-ttu-id="52341-102">Dient zum Abrufen einer Liste von Tabellenobjekten.</span><span class="sxs-lookup"><span data-stu-id="52341-102">Retrieve a list of table objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="52341-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="52341-103">Permissions</span></span>
<span data-ttu-id="52341-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="52341-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="52341-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="52341-106">Permission type</span></span>      | <span data-ttu-id="52341-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="52341-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52341-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="52341-108">Delegated (work or school account)</span></span> | <span data-ttu-id="52341-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52341-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52341-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="52341-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52341-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52341-111">Not supported.</span></span>    |
|<span data-ttu-id="52341-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="52341-112">Application</span></span> | <span data-ttu-id="52341-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52341-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52341-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="52341-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables
GET /workbook/worksheets/{id|name}/tables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="52341-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="52341-115">Optional query parameters</span></span>
<span data-ttu-id="52341-116">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="52341-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52341-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="52341-117">Request headers</span></span>
| <span data-ttu-id="52341-118">Name</span><span class="sxs-lookup"><span data-stu-id="52341-118">Name</span></span>      |<span data-ttu-id="52341-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52341-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52341-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="52341-120">Authorization</span></span>  | <span data-ttu-id="52341-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="52341-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52341-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="52341-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="52341-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="52341-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52341-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="52341-126">Request body</span></span>
<span data-ttu-id="52341-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="52341-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52341-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="52341-128">Response</span></span>

<span data-ttu-id="52341-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [WorkbookTable](../resources/table.md) .</span><span class="sxs-lookup"><span data-stu-id="52341-129">If successful, this method returns a `200 OK` response code and collection of [WorkbookTable](../resources/table.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52341-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="52341-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52341-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="52341-131">Request</span></span>
<span data-ttu-id="52341-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="52341-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables
```
##### <a name="response"></a><span data-ttu-id="52341-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="52341-133">Response</span></span>
<span data-ttu-id="52341-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52341-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "id": "99",
      "name": "name-value",
      "showHeaders": true,
      "showTotals": true,
      "style": "style-value"
    }
  ]
}
```
> <span data-ttu-id="52341-137">**Hinweis:** Verwenden Sie die Abfrageparameter [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) und [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) zum Blättern durch eine große Anzahl von Tabellen.</span><span class="sxs-lookup"><span data-stu-id="52341-137">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) query parameters to page through large numbers of tables.</span></span>

<span data-ttu-id="52341-138">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="52341-138">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
