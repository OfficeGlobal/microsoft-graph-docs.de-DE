# <a name="get-icon"></a><span data-ttu-id="3e972-101">Symbol abrufen</span><span class="sxs-lookup"><span data-stu-id="3e972-101">Get Icon</span></span>

<span data-ttu-id="3e972-102">Dient zum Abrufen der Eigenschaften und der Beziehungen des Symbolobjekts.</span><span class="sxs-lookup"><span data-stu-id="3e972-102">Retrieve the properties and relationships of icon object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e972-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3e972-103">Prerequisites</span></span>
<span data-ttu-id="3e972-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="3e972-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="3e972-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e972-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="3e972-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e972-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort/fields/icon
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3e972-107">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3e972-107">Optional query parameters</span></span>
<span data-ttu-id="3e972-108">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3e972-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e972-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e972-109">Request headers</span></span>
| <span data-ttu-id="3e972-110">Name</span><span class="sxs-lookup"><span data-stu-id="3e972-110">Name</span></span>      |<span data-ttu-id="3e972-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e972-111">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e972-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e972-112">Authorization</span></span>  | <span data-ttu-id="3e972-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3e972-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e972-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e972-115">Request body</span></span>
<span data-ttu-id="3e972-116">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3e972-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e972-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e972-117">Response</span></span>

<span data-ttu-id="3e972-118">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [Icon](../resources/icon.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e972-118">If successful, this method returns a `200 OK` response code and [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e972-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e972-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e972-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e972-120">Request</span></span>
<span data-ttu-id="3e972-121">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3e972-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="3e972-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e972-122">Response</span></span>
<span data-ttu-id="3e972-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e972-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.icon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->