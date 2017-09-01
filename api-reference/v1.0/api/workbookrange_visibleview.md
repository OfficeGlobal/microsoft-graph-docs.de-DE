# <a name="workbookrange-visibleview"></a><span data-ttu-id="723fc-101">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="723fc-101">workbookRange: visibleView</span></span>


## <a name="permissions"></a><span data-ttu-id="723fc-102">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="723fc-102">Permissions</span></span>
<span data-ttu-id="723fc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="723fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="723fc-105">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="723fc-105">Permission type</span></span>      | <span data-ttu-id="723fc-106">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="723fc-106">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="723fc-107">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="723fc-107">Delegated (work or school account)</span></span> | <span data-ttu-id="723fc-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="723fc-108">Files.ReadWrite</span></span>    |
|<span data-ttu-id="723fc-109">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="723fc-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="723fc-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="723fc-110">Not supported.</span></span>    |
|<span data-ttu-id="723fc-111">Anwendung</span><span class="sxs-lookup"><span data-stu-id="723fc-111">Application</span></span> | <span data-ttu-id="723fc-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="723fc-112">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="723fc-113">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="723fc-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="723fc-114">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="723fc-114">Request headers</span></span>
| <span data-ttu-id="723fc-115">Name</span><span class="sxs-lookup"><span data-stu-id="723fc-115">Name</span></span>       | <span data-ttu-id="723fc-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="723fc-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="723fc-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="723fc-117">Authorization</span></span>  | <span data-ttu-id="723fc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="723fc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="723fc-120">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="723fc-120">Workbook-Session-Id</span></span>  | <span data-ttu-id="723fc-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="723fc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="723fc-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="723fc-123">Request body</span></span>

### <a name="response"></a><span data-ttu-id="723fc-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="723fc-124">Response</span></span>
<span data-ttu-id="723fc-125">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das [workbookRangeView](../resources/workbookrangeview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="723fc-125">If successful, this method returns `200, OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="723fc-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="723fc-126">Example</span></span>
<span data-ttu-id="723fc-127">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="723fc-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="723fc-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="723fc-128">Request</span></span>
<span data-ttu-id="723fc-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="723fc-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="723fc-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="723fc-130">Response</span></span>
<span data-ttu-id="723fc-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="723fc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```