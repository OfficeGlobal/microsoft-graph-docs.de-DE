# <a name="create-chartpoints"></a><span data-ttu-id="e4862-101">ChartPoints erstellen</span><span class="sxs-lookup"><span data-stu-id="e4862-101">Create ChartPoints</span></span>

<span data-ttu-id="e4862-102">Verwenden Sie diese API, um neue ChartPoints zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="e4862-102">Use this API to create a new ChartPoints.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4862-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e4862-103">Prerequisites</span></span>
<span data-ttu-id="e4862-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="e4862-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="e4862-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4862-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="e4862-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4862-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points

```
## <a name="request-headers"></a><span data-ttu-id="e4862-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4862-107">Request headers</span></span>
| <span data-ttu-id="e4862-108">Name</span><span class="sxs-lookup"><span data-stu-id="e4862-108">Name</span></span>       | <span data-ttu-id="e4862-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4862-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e4862-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4862-110">Authorization</span></span>  | <span data-ttu-id="e4862-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e4862-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e4862-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4862-113">Request body</span></span>
<span data-ttu-id="e4862-114">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartPoints](../resources/chartpoint.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e4862-114">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e4862-115">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4862-115">Response</span></span>

<span data-ttu-id="e4862-116">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [ChartPoints](../resources/chartpoint.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4862-116">If successful, this method returns `201, Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4862-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4862-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4862-118">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4862-118">Request</span></span>
<span data-ttu-id="e4862-119">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4862-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="e4862-120">Geben Sie im Anforderungstext eine JSON-Darstellung des [ChartPoints](../resources/chartpoint.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e4862-120">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e4862-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4862-121">Response</span></span>
<span data-ttu-id="e4862-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4862-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->