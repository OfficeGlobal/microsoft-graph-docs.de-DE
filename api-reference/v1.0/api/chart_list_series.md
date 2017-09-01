# <a name="list-series"></a><span data-ttu-id="fe9a7-101">Reihe auflisten</span><span class="sxs-lookup"><span data-stu-id="fe9a7-101">List series</span></span>

<span data-ttu-id="fe9a7-102">Dient zum Abrufen einer Liste von chartseries-Objekten.</span><span class="sxs-lookup"><span data-stu-id="fe9a7-102">Retrieve a list of chartseries objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe9a7-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fe9a7-103">Permissions</span></span>
<span data-ttu-id="fe9a7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe9a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fe9a7-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fe9a7-106">Permission type</span></span>      | <span data-ttu-id="fe9a7-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fe9a7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe9a7-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fe9a7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fe9a7-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe9a7-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fe9a7-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fe9a7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe9a7-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe9a7-111">Not supported.</span></span>    |
|<span data-ttu-id="fe9a7-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fe9a7-112">Application</span></span> | <span data-ttu-id="fe9a7-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe9a7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe9a7-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe9a7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/series
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fe9a7-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fe9a7-115">Optional query parameters</span></span>
<span data-ttu-id="fe9a7-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fe9a7-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe9a7-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fe9a7-117">Request headers</span></span>
| <span data-ttu-id="fe9a7-118">Name</span><span class="sxs-lookup"><span data-stu-id="fe9a7-118">Name</span></span>      |<span data-ttu-id="fe9a7-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe9a7-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fe9a7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe9a7-120">Authorization</span></span>  | <span data-ttu-id="fe9a7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fe9a7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe9a7-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fe9a7-123">Request body</span></span>
<span data-ttu-id="fe9a7-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fe9a7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe9a7-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe9a7-125">Response</span></span>

<span data-ttu-id="fe9a7-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [ChartSeries](../resources/chartseries.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe9a7-126">If successful, this method returns a `200 OK` response code and collection of [ChartSeries](../resources/chartseries.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe9a7-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fe9a7-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe9a7-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe9a7-128">Request</span></span>
<span data-ttu-id="fe9a7-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fe9a7-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_series"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
```
##### <a name="response"></a><span data-ttu-id="fe9a7-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe9a7-130">Response</span></span>
<span data-ttu-id="fe9a7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe9a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 59

{
  "value": [
    {
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List series",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->