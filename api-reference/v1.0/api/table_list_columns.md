# <a name="list-columns"></a><span data-ttu-id="a6c1a-101">Spalten auflisten</span><span class="sxs-lookup"><span data-stu-id="a6c1a-101">List columns</span></span>

<span data-ttu-id="a6c1a-102">Dient zum Abrufen einer Liste von tablecolumn-Objekten.</span><span class="sxs-lookup"><span data-stu-id="a6c1a-102">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a6c1a-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a6c1a-103">Permissions</span></span>
<span data-ttu-id="a6c1a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a6c1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a6c1a-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a6c1a-106">Permission type</span></span>      | <span data-ttu-id="a6c1a-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a6c1a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6c1a-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a6c1a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a6c1a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6c1a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a6c1a-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a6c1a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6c1a-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6c1a-111">Not supported.</span></span>    |
|<span data-ttu-id="a6c1a-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a6c1a-112">Application</span></span> | <span data-ttu-id="a6c1a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6c1a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6c1a-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6c1a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a6c1a-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a6c1a-115">Optional query parameters</span></span>
<span data-ttu-id="a6c1a-116">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a6c1a-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>  <span data-ttu-id="a6c1a-117">Verwenden Sie für zuverlässige Ergebnisse die Abfrageparameter [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) und [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) zum Blättern durch die Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="a6c1a-117">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="a6c1a-118">Dies hilft, Leistungsprobleme im Zusammenhang mit großen Resultsets zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="a6c1a-118">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6c1a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a6c1a-119">Request headers</span></span>
| <span data-ttu-id="a6c1a-120">Name</span><span class="sxs-lookup"><span data-stu-id="a6c1a-120">Name</span></span>      |<span data-ttu-id="a6c1a-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6c1a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a6c1a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6c1a-122">Authorization</span></span>  | <span data-ttu-id="a6c1a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a6c1a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a6c1a-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="a6c1a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a6c1a-p104">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="a6c1a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6c1a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a6c1a-128">Request body</span></span>
<span data-ttu-id="a6c1a-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a6c1a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6c1a-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6c1a-130">Response</span></span>

<span data-ttu-id="a6c1a-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [WorkbookTableColumn](../resources/tablecolumn.md) .</span><span class="sxs-lookup"><span data-stu-id="a6c1a-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a6c1a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a6c1a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6c1a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6c1a-133">Request</span></span>
<span data-ttu-id="a6c1a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a6c1a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="a6c1a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6c1a-135">Response</span></span>
<span data-ttu-id="a6c1a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6c1a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

> <span data-ttu-id="a6c1a-139">
  \*\*Hinweis:\*\* Verwenden Sie die Abfrageparameter [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) und [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) zum Blättern durch eine große Anzahl von Spalten.</span><span class="sxs-lookup"><span data-stu-id="a6c1a-139">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="a6c1a-140">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="a6c1a-140">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->