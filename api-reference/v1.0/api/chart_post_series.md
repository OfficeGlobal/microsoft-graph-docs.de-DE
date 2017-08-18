# <a name="create-chartseries"></a><span data-ttu-id="39257-101">ChartSeries erstellen</span><span class="sxs-lookup"><span data-stu-id="39257-101">Create ChartSeries</span></span>

<span data-ttu-id="39257-102">Verwenden Sie diese API, um eine neue ChartSeries zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="39257-102">Use this API to create a new ChartSeries.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39257-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="39257-103">Prerequisites</span></span>
<span data-ttu-id="39257-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="39257-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="39257-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39257-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="39257-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39257-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series

```
## <a name="request-headers"></a><span data-ttu-id="39257-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39257-107">Request headers</span></span>
| <span data-ttu-id="39257-108">Name</span><span class="sxs-lookup"><span data-stu-id="39257-108">Name</span></span>       | <span data-ttu-id="39257-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39257-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="39257-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="39257-110">Authorization</span></span>  | <span data-ttu-id="39257-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="39257-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="39257-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39257-113">Request body</span></span>
<span data-ttu-id="39257-114">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartSeries](../resources/chartseries.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="39257-114">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="39257-115">Antwort</span><span class="sxs-lookup"><span data-stu-id="39257-115">Response</span></span>

<span data-ttu-id="39257-116">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [ChartSeries](../resources/chartseries.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39257-116">If successful, this method returns `201, Created` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39257-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39257-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39257-118">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39257-118">Request</span></span>
<span data-ttu-id="39257-119">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39257-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="39257-120">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartSeries](../resources/chartseries.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="39257-120">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="39257-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="39257-121">Response</span></span>
<span data-ttu-id="39257-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39257-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->