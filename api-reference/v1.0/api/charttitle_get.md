# <a name="get-charttitle"></a><span data-ttu-id="aaacf-101">ChartTitle abrufen</span><span class="sxs-lookup"><span data-stu-id="aaacf-101">Get ChartTitle</span></span>

<span data-ttu-id="aaacf-102">Dient zum Abrufen der Eigenschaften und der Beziehungen des ChartTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aaacf-102">Retrieve the properties and relationships of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="aaacf-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aaacf-103">Permissions</span></span>
<span data-ttu-id="aaacf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aaacf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aaacf-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aaacf-106">Permission type</span></span>      | <span data-ttu-id="aaacf-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aaacf-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaacf-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aaacf-108">Delegated (work or school account)</span></span> | <span data-ttu-id="aaacf-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaacf-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aaacf-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aaacf-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaacf-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aaacf-111">Not supported.</span></span>    |
|<span data-ttu-id="aaacf-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aaacf-112">Application</span></span> | <span data-ttu-id="aaacf-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aaacf-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaacf-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aaacf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aaacf-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="aaacf-115">Optional query parameters</span></span>
<span data-ttu-id="aaacf-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aaacf-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aaacf-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aaacf-117">Request headers</span></span>
| <span data-ttu-id="aaacf-118">Name</span><span class="sxs-lookup"><span data-stu-id="aaacf-118">Name</span></span>      |<span data-ttu-id="aaacf-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aaacf-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aaacf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaacf-120">Authorization</span></span>  | <span data-ttu-id="aaacf-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aaacf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aaacf-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aaacf-123">Request body</span></span>
<span data-ttu-id="aaacf-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aaacf-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaacf-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="aaacf-125">Response</span></span>

<span data-ttu-id="aaacf-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [ChartTitle](../resources/charttitle.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aaacf-126">If successful, this method returns a `200 OK` response code and [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aaacf-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aaacf-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aaacf-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aaacf-128">Request</span></span>
<span data-ttu-id="aaacf-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aaacf-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_charttitle"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/title
```
##### <a name="response"></a><span data-ttu-id="aaacf-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="aaacf-130">Response</span></span>
<span data-ttu-id="aaacf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aaacf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->