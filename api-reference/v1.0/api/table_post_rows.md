# <a name="create-tablerow"></a><span data-ttu-id="e0d08-101">TableRow erstellen</span><span class="sxs-lookup"><span data-stu-id="e0d08-101">Create TableRow</span></span>

<span data-ttu-id="e0d08-102">Verwenden Sie diese API zum Erstellen einer neuen TableRow.</span><span class="sxs-lookup"><span data-stu-id="e0d08-102">Use this API to create a new TableRow.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0d08-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e0d08-103">Prerequisites</span></span>
<span data-ttu-id="e0d08-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="e0d08-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="e0d08-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0d08-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="e0d08-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0d08-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows

```
## <a name="request-headers"></a><span data-ttu-id="e0d08-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0d08-107">Request headers</span></span>
| <span data-ttu-id="e0d08-108">Name</span><span class="sxs-lookup"><span data-stu-id="e0d08-108">Name</span></span>       | <span data-ttu-id="e0d08-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0d08-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e0d08-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0d08-110">Authorization</span></span>  | <span data-ttu-id="e0d08-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0d08-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e0d08-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e0d08-113">Request body</span></span>
<span data-ttu-id="e0d08-114">Geben Sie im Anforderungstext eine JSON-Darstellung des [TableRow](../resources/tablerow.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e0d08-114">In the request body, supply a JSON representation of [TableRow](../resources/tablerow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e0d08-115">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0d08-115">Response</span></span>

<span data-ttu-id="e0d08-116">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [TableRow](../resources/tablerow.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0d08-116">If successful, this method returns `201, Created` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0d08-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0d08-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0d08-118">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0d08-118">Request</span></span>
<span data-ttu-id="e0d08-119">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0d08-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablerow_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="e0d08-120">Geben Sie im Anforderungstext eine JSON-Darstellung des [TableRow](../resources/tablerow.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e0d08-120">In the request body, supply a JSON representation of [TableRow](../resources/tablerow.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e0d08-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0d08-121">Response</span></span>
<span data-ttu-id="e0d08-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0d08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->