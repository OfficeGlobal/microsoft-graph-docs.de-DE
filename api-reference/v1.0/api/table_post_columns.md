# <a name="create-tablecolumn"></a><span data-ttu-id="08687-101">TableColumn erstellen</span><span class="sxs-lookup"><span data-stu-id="08687-101">Create TableColumn</span></span>

<span data-ttu-id="08687-102">Verwenden Sie diese API zum Erstellen einer neuen TableColumn.</span><span class="sxs-lookup"><span data-stu-id="08687-102">Use this API to create a new TableColumn.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="08687-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="08687-103">Prerequisites</span></span>
<span data-ttu-id="08687-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="08687-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="08687-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08687-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="08687-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08687-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="08687-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="08687-107">Request headers</span></span>
| <span data-ttu-id="08687-108">Name</span><span class="sxs-lookup"><span data-stu-id="08687-108">Name</span></span>       | <span data-ttu-id="08687-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08687-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="08687-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="08687-110">Authorization</span></span>  | <span data-ttu-id="08687-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="08687-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="08687-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="08687-113">Request body</span></span>
<span data-ttu-id="08687-114">Geben Sie im Anforderungstext eine JSON-Darstellung des [TableColumn](../resources/tablecolumn.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="08687-114">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="08687-115">Antwort</span><span class="sxs-lookup"><span data-stu-id="08687-115">Response</span></span>

<span data-ttu-id="08687-116">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [TableColumn](../resources/tablecolumn.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08687-116">If successful, this method returns `201, Created` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08687-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="08687-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08687-118">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08687-118">Request</span></span>
<span data-ttu-id="08687-119">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="08687-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="08687-120">Geben Sie im Anforderungstext eine JSON-Darstellung des [TableColumn](../resources/tablecolumn.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="08687-120">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="08687-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="08687-121">Response</span></span>
<span data-ttu-id="08687-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08687-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->