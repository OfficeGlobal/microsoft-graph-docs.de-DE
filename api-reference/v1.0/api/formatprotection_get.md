# <a name="get-formatprotection"></a><span data-ttu-id="1a985-101">FormatProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="1a985-101">Get FormatProtection</span></span>

<span data-ttu-id="1a985-102">Dient zum Abrufen der Eigenschaften und der Beziehungen des formatProtection-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1a985-102">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a985-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1a985-103">Prerequisites</span></span>
<span data-ttu-id="1a985-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="1a985-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="1a985-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a985-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="1a985-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a985-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a985-107">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1a985-107">Optional query parameters</span></span>
<span data-ttu-id="1a985-108">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1a985-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a985-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a985-109">Request headers</span></span>
| <span data-ttu-id="1a985-110">Name</span><span class="sxs-lookup"><span data-stu-id="1a985-110">Name</span></span>      |<span data-ttu-id="1a985-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a985-111">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a985-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a985-112">Authorization</span></span>  | <span data-ttu-id="1a985-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a985-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a985-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a985-115">Request body</span></span>
<span data-ttu-id="1a985-116">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1a985-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a985-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a985-117">Response</span></span>

<span data-ttu-id="1a985-118">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [FormatProtection](../resources/formatprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a985-118">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a985-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1a985-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a985-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a985-120">Request</span></span>
<span data-ttu-id="1a985-121">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1a985-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
```
##### <a name="response"></a><span data-ttu-id="1a985-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a985-122">Response</span></span>
<span data-ttu-id="1a985-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a985-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->