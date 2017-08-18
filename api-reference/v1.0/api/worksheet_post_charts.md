# <a name="create-chart"></a><span data-ttu-id="ad9ce-101">Diagramm erstellen</span><span class="sxs-lookup"><span data-stu-id="ad9ce-101">Create Chart</span></span>

<span data-ttu-id="ad9ce-102">Verwenden Sie diese API zum Erstellen eines neuen Diagramms.</span><span class="sxs-lookup"><span data-stu-id="ad9ce-102">Use this API to create a new Chart.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad9ce-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ad9ce-103">Prerequisites</span></span>
<span data-ttu-id="ad9ce-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="ad9ce-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="ad9ce-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad9ce-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="ad9ce-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad9ce-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="ad9ce-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ad9ce-107">Request headers</span></span>
| <span data-ttu-id="ad9ce-108">Name</span><span class="sxs-lookup"><span data-stu-id="ad9ce-108">Name</span></span>       | <span data-ttu-id="ad9ce-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad9ce-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ad9ce-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad9ce-110">Authorization</span></span>  | <span data-ttu-id="ad9ce-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ad9ce-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="ad9ce-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ad9ce-113">Request body</span></span>
<span data-ttu-id="ad9ce-114">Geben Sie im Anforderungstext eine JSON-Darstellung des [Chart](../resources/chart.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ad9ce-114">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ad9ce-115">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad9ce-115">Response</span></span>

<span data-ttu-id="ad9ce-116">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [Chart](../resources/chart.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ad9ce-116">If successful, this method returns `201, Created` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad9ce-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ad9ce-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad9ce-118">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad9ce-118">Request</span></span>
<span data-ttu-id="ad9ce-119">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ad9ce-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
<span data-ttu-id="ad9ce-120">Geben Sie im Anforderungstext eine JSON-Darstellung des [Chart](../resources/chart.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ad9ce-120">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ad9ce-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad9ce-121">Response</span></span>
<span data-ttu-id="ad9ce-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ad9ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->