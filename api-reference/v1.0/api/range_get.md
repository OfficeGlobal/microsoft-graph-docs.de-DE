# <a name="get-range"></a><span data-ttu-id="7e6a1-101">Range abrufen</span><span class="sxs-lookup"><span data-stu-id="7e6a1-101">Get Range</span></span>

<span data-ttu-id="7e6a1-102">Dient zum Abrufen der Eigenschaften und der Beziehungen des Bereichsobjekts.</span><span class="sxs-lookup"><span data-stu-id="7e6a1-102">Retrieve the properties and relationships of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7e6a1-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7e6a1-103">Permissions</span></span>
<span data-ttu-id="7e6a1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7e6a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7e6a1-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7e6a1-106">Permission type</span></span>      | <span data-ttu-id="7e6a1-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7e6a1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e6a1-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7e6a1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7e6a1-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e6a1-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7e6a1-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7e6a1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e6a1-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e6a1-111">Not supported.</span></span>    |
|<span data-ttu-id="7e6a1-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7e6a1-112">Application</span></span> | <span data-ttu-id="7e6a1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e6a1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e6a1-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e6a1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range(address='<address>')
GET /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7e6a1-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7e6a1-115">Optional query parameters</span></span>
<span data-ttu-id="7e6a1-116">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7e6a1-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e6a1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7e6a1-117">Request headers</span></span>
| <span data-ttu-id="7e6a1-118">Name</span><span class="sxs-lookup"><span data-stu-id="7e6a1-118">Name</span></span>      |<span data-ttu-id="7e6a1-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e6a1-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7e6a1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e6a1-120">Authorization</span></span>  | <span data-ttu-id="7e6a1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7e6a1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e6a1-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="7e6a1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7e6a1-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="7e6a1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e6a1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7e6a1-126">Request body</span></span>
<span data-ttu-id="7e6a1-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7e6a1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e6a1-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e6a1-128">Response</span></span>

<span data-ttu-id="7e6a1-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Range](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e6a1-129">If successful, this method returns a `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7e6a1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7e6a1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e6a1-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e6a1-131">Request</span></span>
<span data-ttu-id="7e6a1-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7e6a1-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```
##### <a name="response"></a><span data-ttu-id="7e6a1-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e6a1-133">Response</span></span>
<span data-ttu-id="7e6a1-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e6a1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->