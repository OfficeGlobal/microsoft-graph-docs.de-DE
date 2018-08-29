# <a name="list-names"></a><span data-ttu-id="aa16f-101">Namen auflisten</span><span class="sxs-lookup"><span data-stu-id="aa16f-101">List names</span></span>

<span data-ttu-id="aa16f-102">Dient zum Abrufen einer Liste von benannten Elementen, die mit dem Arbeitsblatt verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="aa16f-102">Retrieve a list of named item associated with the worksheet.</span></span> 
## <a name="permissions"></a><span data-ttu-id="aa16f-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aa16f-103">Permissions</span></span>
<span data-ttu-id="aa16f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa16f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aa16f-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aa16f-106">Permission type</span></span>      | <span data-ttu-id="aa16f-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aa16f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa16f-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aa16f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="aa16f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa16f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa16f-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aa16f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa16f-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa16f-111">Not supported.</span></span>    |
|<span data-ttu-id="aa16f-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aa16f-112">Application</span></span> | <span data-ttu-id="aa16f-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa16f-113">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa16f-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa16f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets({id|name})/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aa16f-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="aa16f-115">Optional query parameters</span></span>
<span data-ttu-id="aa16f-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aa16f-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa16f-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aa16f-117">Request headers</span></span>
| <span data-ttu-id="aa16f-118">Name</span><span class="sxs-lookup"><span data-stu-id="aa16f-118">Name</span></span>      |<span data-ttu-id="aa16f-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa16f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aa16f-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="aa16f-120">Authorization</span></span>  | <span data-ttu-id="aa16f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa16f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa16f-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="aa16f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="aa16f-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="aa16f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa16f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aa16f-126">Request body</span></span>
<span data-ttu-id="aa16f-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aa16f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa16f-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa16f-128">Response</span></span>

<span data-ttu-id="aa16f-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [WorkbookNamedItem](../resources/nameditem.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa16f-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa16f-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa16f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa16f-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa16f-131">Request</span></span>
<span data-ttu-id="aa16f-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa16f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tables"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/names
```
##### <a name="response"></a><span data-ttu-id="aa16f-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa16f-133">Response</span></span>
<span data-ttu-id="aa16f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa16f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem",
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
