# <a name="create-rangeborder"></a><span data-ttu-id="3e502-101">RangeBorder erstellen</span><span class="sxs-lookup"><span data-stu-id="3e502-101">Create RangeBorder</span></span>

<span data-ttu-id="3e502-102">Verwenden Sie diese API zum Erstellen eines neuen RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="3e502-102">Use this API to create a new RangeBorder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e502-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3e502-103">Prerequisites</span></span>
<span data-ttu-id="3e502-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="3e502-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="3e502-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e502-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="3e502-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e502-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders
POST /workbook/worksheets/{id|name}/range(<address>)/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="3e502-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e502-107">Request headers</span></span>
| <span data-ttu-id="3e502-108">Name</span><span class="sxs-lookup"><span data-stu-id="3e502-108">Name</span></span>       | <span data-ttu-id="3e502-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e502-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3e502-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e502-110">Authorization</span></span>  | <span data-ttu-id="3e502-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3e502-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="3e502-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e502-113">Request body</span></span>
<span data-ttu-id="3e502-114">Geben Sie im Anforderungstext eine JSON-Darstellung des [RangeBorder](../resources/rangeborder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3e502-114">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3e502-115">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e502-115">Response</span></span>

<span data-ttu-id="3e502-116">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [RangeBorder](../resources/rangeborder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e502-116">If successful, this method returns `201, Created` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e502-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e502-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e502-118">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e502-118">Request</span></span>
<span data-ttu-id="3e502-119">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e502-119">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
<span data-ttu-id="3e502-120">Geben Sie im Anforderungstext eine JSON-Darstellung des [RangeBorder](../resources/rangeborder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3e502-120">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3e502-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e502-121">Response</span></span>
<span data-ttu-id="3e502-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e502-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->