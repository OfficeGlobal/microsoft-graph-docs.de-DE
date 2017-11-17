# <a name="list-names"></a><span data-ttu-id="8b929-101">Namen auflisten</span><span class="sxs-lookup"><span data-stu-id="8b929-101">List names</span></span>

<span data-ttu-id="8b929-102">Dient zum Abrufen einer Liste von benannten Elementen, die mit dem Arbeitsblatt verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="8b929-102">Retrieve a list of named item associated with the worksheet.</span></span> 
## <a name="permissions"></a><span data-ttu-id="8b929-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8b929-103">Permissions</span></span>
<span data-ttu-id="8b929-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8b929-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8b929-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b929-106">Permission type</span></span>      | <span data-ttu-id="8b929-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b929-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b929-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b929-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8b929-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b929-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b929-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b929-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b929-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b929-111">Not supported.</span></span>    |
|<span data-ttu-id="8b929-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b929-112">Application</span></span> | <span data-ttu-id="8b929-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b929-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b929-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b929-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets({id|name})/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8b929-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8b929-115">Optional query parameters</span></span>
<span data-ttu-id="8b929-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8b929-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b929-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b929-117">Request headers</span></span>
| <span data-ttu-id="8b929-118">Name</span><span class="sxs-lookup"><span data-stu-id="8b929-118">Name</span></span>      |<span data-ttu-id="8b929-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b929-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8b929-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b929-120">Authorization</span></span>  | <span data-ttu-id="8b929-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8b929-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b929-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b929-123">Request body</span></span>
<span data-ttu-id="8b929-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8b929-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b929-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b929-125">Response</span></span>

<span data-ttu-id="8b929-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [NamedItem](../resources/nameditem.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b929-126">If successful, this method returns a `200 OK` response code and collection of [NamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b929-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b929-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b929-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b929-128">Request</span></span>
<span data-ttu-id="8b929-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b929-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tables"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/names
```
##### <a name="response"></a><span data-ttu-id="8b929-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b929-130">Response</span></span>
<span data-ttu-id="8b929-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b929-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "name": "myrange",
      "scope": "worksheet"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tables",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
