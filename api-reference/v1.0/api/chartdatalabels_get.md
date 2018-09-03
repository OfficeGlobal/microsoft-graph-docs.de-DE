# <a name="get-chartdatalabels"></a><span data-ttu-id="b3f58-101">ChartDataLabels abrufen</span><span class="sxs-lookup"><span data-stu-id="b3f58-101">Get ChartDataLabels</span></span>

<span data-ttu-id="b3f58-102">Dient zum Abrufen der Eigenschaften und der Beziehungen des ChartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b3f58-102">Retrieve the properties and relationships of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3f58-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b3f58-103">Permissions</span></span>
<span data-ttu-id="b3f58-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b3f58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b3f58-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3f58-106">Permission type</span></span>      | <span data-ttu-id="b3f58-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3f58-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3f58-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3f58-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b3f58-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3f58-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b3f58-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3f58-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3f58-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3f58-111">Not supported.</span></span>    |
|<span data-ttu-id="b3f58-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b3f58-112">Application</span></span> | <span data-ttu-id="b3f58-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3f58-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3f58-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3f58-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3f58-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b3f58-115">Optional query parameters</span></span>
<span data-ttu-id="b3f58-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b3f58-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3f58-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3f58-117">Request headers</span></span>
| <span data-ttu-id="b3f58-118">Name</span><span class="sxs-lookup"><span data-stu-id="b3f58-118">Name</span></span>      |<span data-ttu-id="b3f58-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3f58-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b3f58-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b3f58-120">Authorization</span></span>  | <span data-ttu-id="b3f58-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b3f58-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3f58-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="b3f58-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b3f58-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="b3f58-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3f58-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3f58-126">Request body</span></span>
<span data-ttu-id="b3f58-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b3f58-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3f58-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3f58-128">Response</span></span>

<span data-ttu-id="b3f58-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [WorkbookChartDataLabels](../resources/chartdatalabels.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3f58-129">If successful, this method returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3f58-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3f58-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3f58-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3f58-131">Request</span></span>
<span data-ttu-id="b3f58-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b3f58-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartdatalabels"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
##### <a name="response"></a><span data-ttu-id="b3f58-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3f58-133">Response</span></span>
<span data-ttu-id="b3f58-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3f58-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartDataLabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->