# <a name="list-borders"></a><span data-ttu-id="45d8a-101">Rahmen auflisten</span><span class="sxs-lookup"><span data-stu-id="45d8a-101">List borders</span></span>

<span data-ttu-id="45d8a-102">Dient zum Abrufen einer Liste von rangeborder-Objekten.</span><span class="sxs-lookup"><span data-stu-id="45d8a-102">Retrieve a list of rangeborder objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="45d8a-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="45d8a-103">Permissions</span></span>
<span data-ttu-id="45d8a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="45d8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="45d8a-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="45d8a-106">Permission type</span></span>      | <span data-ttu-id="45d8a-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="45d8a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45d8a-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="45d8a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="45d8a-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45d8a-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="45d8a-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="45d8a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45d8a-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45d8a-111">Not supported.</span></span>    |
|<span data-ttu-id="45d8a-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="45d8a-112">Application</span></span> | <span data-ttu-id="45d8a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45d8a-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45d8a-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="45d8a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/borders
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="45d8a-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="45d8a-115">Optional query parameters</span></span>
<span data-ttu-id="45d8a-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="45d8a-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45d8a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="45d8a-117">Request headers</span></span>
| <span data-ttu-id="45d8a-118">Name</span><span class="sxs-lookup"><span data-stu-id="45d8a-118">Name</span></span>      |<span data-ttu-id="45d8a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45d8a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="45d8a-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="45d8a-120">Authorization</span></span>  | <span data-ttu-id="45d8a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="45d8a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45d8a-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="45d8a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="45d8a-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="45d8a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45d8a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="45d8a-126">Request body</span></span>
<span data-ttu-id="45d8a-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="45d8a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45d8a-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="45d8a-128">Response</span></span>

<span data-ttu-id="45d8a-129">Wenn erfolgreich, gibt diese Methode einen `200 OK` Antwortcode und eine Sammlung von [WorkbookRangeBorder](../resources/rangeborder.md)-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="45d8a-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/rangeborder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45d8a-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="45d8a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45d8a-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="45d8a-131">Request</span></span>
<span data-ttu-id="45d8a-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="45d8a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_borders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
```
##### <a name="response"></a><span data-ttu-id="45d8a-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="45d8a-133">Response</span></span>
<span data-ttu-id="45d8a-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45d8a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 185

{
  "value": [
    {
      "id": "id-value",
      "color": "color-value",
      "style": "style-value",
      "sideIndex": "sideIndex-value",
      "weight": "weight-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List borders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->