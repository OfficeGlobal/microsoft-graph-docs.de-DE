# <a name="list-rangeview-rows"></a><span data-ttu-id="257c5-101">rangeView-Zeilen auflisten</span><span class="sxs-lookup"><span data-stu-id="257c5-101">List rangeView rows</span></span>

<span data-ttu-id="257c5-102">Abrufen einer Liste von rangeView-Objekten.</span><span class="sxs-lookup"><span data-stu-id="257c5-102">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="257c5-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="257c5-103">Permissions</span></span>
<span data-ttu-id="257c5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="257c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="257c5-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="257c5-106">Permission type</span></span>      | <span data-ttu-id="257c5-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="257c5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="257c5-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="257c5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="257c5-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="257c5-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="257c5-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="257c5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="257c5-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="257c5-111">Not supported.</span></span>    |
|<span data-ttu-id="257c5-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="257c5-112">Application</span></span> | <span data-ttu-id="257c5-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="257c5-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="257c5-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="257c5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="257c5-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="257c5-115">Optional query parameters</span></span>
<span data-ttu-id="257c5-116">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="257c5-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="257c5-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="257c5-117">Request headers</span></span>
| <span data-ttu-id="257c5-118">Name</span><span class="sxs-lookup"><span data-stu-id="257c5-118">Name</span></span>      |<span data-ttu-id="257c5-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="257c5-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="257c5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="257c5-120">Authorization</span></span>  | <span data-ttu-id="257c5-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="257c5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="257c5-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="257c5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="257c5-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="257c5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="257c5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="257c5-126">Request body</span></span>
<span data-ttu-id="257c5-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="257c5-127">Do not supply a request body for this method.</span></span>
### <a name="response"></a><span data-ttu-id="257c5-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="257c5-128">Response</span></span>
<span data-ttu-id="257c5-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [workbookRangeView](../resources/workbookrangeview.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="257c5-129">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="257c5-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="257c5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="257c5-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="257c5-131">Request</span></span>
<span data-ttu-id="257c5-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="257c5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/rows
```
##### <a name="response"></a><span data-ttu-id="257c5-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="257c5-133">Response</span></span>
<span data-ttu-id="257c5-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="257c5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 247

{
  "value": [
    {
      "cellAddresses": "cellAddresses-value",
      "columnCount": 99,
      "formulas": "formulas-value",
      "formulasLocal": "formulasLocal-value",
      "formulasR1C1": "formulasR1C1-value",
      "index": 99
    }
  ]
}
```
