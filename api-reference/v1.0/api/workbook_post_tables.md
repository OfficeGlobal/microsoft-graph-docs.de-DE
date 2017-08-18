# <a name="create-table"></a><span data-ttu-id="48006-101">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="48006-101">Create Table</span></span>

<span data-ttu-id="48006-102">Verwenden Sie diese API zum Erstellen einer neuen Tabelle.</span><span class="sxs-lookup"><span data-stu-id="48006-102">Use this API to create a new Table.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48006-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="48006-103">Prerequisites</span></span>
<span data-ttu-id="48006-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="48006-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="48006-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48006-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="48006-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48006-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="48006-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48006-107">Request headers</span></span>
| <span data-ttu-id="48006-108">Name</span><span class="sxs-lookup"><span data-stu-id="48006-108">Name</span></span>       | <span data-ttu-id="48006-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48006-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="48006-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="48006-110">Authorization</span></span>  | <span data-ttu-id="48006-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48006-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="48006-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48006-113">Request body</span></span>
<span data-ttu-id="48006-114">Geben Sie im Anforderungstext eine JSON-Darstellung des [Table](../resources/table.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="48006-114">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="48006-115">Antwort</span><span class="sxs-lookup"><span data-stu-id="48006-115">Response</span></span>

<span data-ttu-id="48006-116">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [Table](../resources/table.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48006-116">If successful, this method returns `201, Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48006-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48006-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48006-118">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48006-118">Request</span></span>
<span data-ttu-id="48006-119">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48006-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/$/add
Content-type: application/json
Content-length: 109

{
  "id": 99,
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
<span data-ttu-id="48006-120">Geben Sie im Anforderungstext eine JSON-Darstellung des [Table](../resources/table.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="48006-120">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="48006-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="48006-121">Response</span></span>
<span data-ttu-id="48006-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48006-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
