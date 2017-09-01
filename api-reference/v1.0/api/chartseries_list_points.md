# <a name="list-points"></a><span data-ttu-id="8b065-101">Punkte auflisten</span><span class="sxs-lookup"><span data-stu-id="8b065-101">List points</span></span>

<span data-ttu-id="8b065-102">Dient zum Abrufen einer Liste von chartPoints-Objekten.</span><span class="sxs-lookup"><span data-stu-id="8b065-102">Retrieve a list of chartpoints objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b065-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8b065-103">Permissions</span></span>
<span data-ttu-id="8b065-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8b065-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8b065-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b065-106">Permission type</span></span>      | <span data-ttu-id="8b065-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b065-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b065-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b065-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8b065-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b065-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b065-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b065-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b065-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b065-111">Not supported.</span></span>    |
|<span data-ttu-id="8b065-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b065-112">Application</span></span> | <span data-ttu-id="8b065-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b065-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b065-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b065-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8b065-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8b065-115">Optional query parameters</span></span>
<span data-ttu-id="8b065-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8b065-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b065-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b065-117">Request headers</span></span>
| <span data-ttu-id="8b065-118">Name</span><span class="sxs-lookup"><span data-stu-id="8b065-118">Name</span></span>      |<span data-ttu-id="8b065-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b065-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8b065-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b065-120">Authorization</span></span>  | <span data-ttu-id="8b065-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8b065-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b065-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b065-123">Request body</span></span>
<span data-ttu-id="8b065-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8b065-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b065-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b065-125">Response</span></span>

<span data-ttu-id="8b065-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [ChartPoints](../resources/chartpoint.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b065-126">If successful, this method returns a `200 OK` response code and collection of [ChartPoints](../resources/chartpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b065-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b065-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b065-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b065-128">Request</span></span>
<span data-ttu-id="8b065-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b065-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_points"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
```
##### <a name="response"></a><span data-ttu-id="8b065-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b065-130">Response</span></span>
<span data-ttu-id="8b065-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b065-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 32

{
  "value": [
    {
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List points",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->