# <a name="list-worksheets"></a><span data-ttu-id="63690-101">Arbeitsblätter auflisten</span><span class="sxs-lookup"><span data-stu-id="63690-101">List worksheets</span></span>

<span data-ttu-id="63690-102">Dient zum Abrufen einer Liste von Arbeitsblattobjekten.</span><span class="sxs-lookup"><span data-stu-id="63690-102">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="63690-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="63690-103">Permissions</span></span>
<span data-ttu-id="63690-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="63690-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="63690-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="63690-106">Permission type</span></span>      | <span data-ttu-id="63690-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="63690-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63690-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="63690-108">Delegated (work or school account)</span></span> | <span data-ttu-id="63690-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63690-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="63690-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="63690-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63690-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63690-111">Not supported.</span></span>    |
|<span data-ttu-id="63690-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="63690-112">Application</span></span> | <span data-ttu-id="63690-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63690-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63690-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="63690-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="63690-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="63690-115">Optional query parameters</span></span>
<span data-ttu-id="63690-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="63690-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63690-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="63690-117">Request headers</span></span>
| <span data-ttu-id="63690-118">Name</span><span class="sxs-lookup"><span data-stu-id="63690-118">Name</span></span>      |<span data-ttu-id="63690-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63690-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="63690-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="63690-120">Authorization</span></span>  | <span data-ttu-id="63690-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="63690-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="63690-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="63690-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="63690-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="63690-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63690-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="63690-126">Request body</span></span>
<span data-ttu-id="63690-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="63690-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63690-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="63690-128">Response</span></span>

<span data-ttu-id="63690-129">Wenn das Verfahrene erfolgreich verläuft, werden im Antworttext  der Antwortcode `200 OK` und eine Sammlung von [WorkbookWorksheet](../resources/worksheet.md)-Objekten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="63690-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="63690-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="63690-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63690-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="63690-131">Request</span></span>
<span data-ttu-id="63690-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="63690-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheets"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets
```
##### <a name="response"></a><span data-ttu-id="63690-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="63690-133">Response</span></span>
<span data-ttu-id="63690-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="63690-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "id": "id-value",
      "position": 99,
      "name": "name-value",
      "visibility": "visibility-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List worksheets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->