# <a name="get-chartdatalabels"></a><span data-ttu-id="7a194-101">ChartDataLabels abrufen</span><span class="sxs-lookup"><span data-stu-id="7a194-101">Get ChartDataLabels</span></span>

<span data-ttu-id="7a194-102">Dient zum Abrufen der Eigenschaften und der Beziehungen des ChartDataLabels-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7a194-102">Retrieve the properties and relationships of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a194-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7a194-103">Permissions</span></span>
<span data-ttu-id="7a194-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7a194-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7a194-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a194-106">Permission type</span></span>      | <span data-ttu-id="7a194-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a194-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a194-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a194-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7a194-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a194-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7a194-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a194-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a194-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a194-111">Not supported.</span></span>    |
|<span data-ttu-id="7a194-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a194-112">Application</span></span> | <span data-ttu-id="7a194-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7a194-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a194-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a194-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7a194-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7a194-115">Optional query parameters</span></span>
<span data-ttu-id="7a194-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7a194-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a194-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a194-117">Request headers</span></span>
| <span data-ttu-id="7a194-118">Name</span><span class="sxs-lookup"><span data-stu-id="7a194-118">Name</span></span>      |<span data-ttu-id="7a194-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a194-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7a194-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a194-120">Authorization</span></span>  | <span data-ttu-id="7a194-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7a194-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a194-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a194-123">Request body</span></span>
<span data-ttu-id="7a194-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7a194-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a194-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a194-125">Response</span></span>

<span data-ttu-id="7a194-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [ChartDataLabels](../resources/chartdatalabels.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a194-126">If successful, this method returns a `200 OK` response code and [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7a194-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a194-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a194-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a194-128">Request</span></span>
<span data-ttu-id="7a194-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a194-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartdatalabels"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
##### <a name="response"></a><span data-ttu-id="7a194-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a194-130">Response</span></span>
<span data-ttu-id="7a194-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a194-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartDataLabels"
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