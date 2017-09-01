# <a name="workbookrangeview-range"></a><span data-ttu-id="fc513-101">workbookRangeView: Bereich</span><span class="sxs-lookup"><span data-stu-id="fc513-101">workbookRangeView: range</span></span>
<span data-ttu-id="fc513-102">Geben Sie den Bereich zurück, der der rangeView-Ressource zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="fc513-102">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc513-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fc513-103">Permissions</span></span>
<span data-ttu-id="fc513-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fc513-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="fc513-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fc513-106">Permission type</span></span>      | <span data-ttu-id="fc513-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fc513-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc513-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fc513-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fc513-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc513-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc513-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fc513-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc513-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc513-111">Not supported.</span></span>    |
|<span data-ttu-id="fc513-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fc513-112">Application</span></span> | <span data-ttu-id="fc513-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc513-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc513-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc513-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="fc513-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fc513-115">Request headers</span></span>
| <span data-ttu-id="fc513-116">Name</span><span class="sxs-lookup"><span data-stu-id="fc513-116">Name</span></span>       | <span data-ttu-id="fc513-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc513-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc513-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc513-118">Authorization</span></span>  | <span data-ttu-id="fc513-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fc513-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc513-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="fc513-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="fc513-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="fc513-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc513-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fc513-124">Request body</span></span>

### <a name="response"></a><span data-ttu-id="fc513-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc513-125">Response</span></span>
<span data-ttu-id="fc513-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das [workbookRange](../resources/range.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc513-126">If successful, this method returns `200, OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc513-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fc513-127">Example</span></span>
<span data-ttu-id="fc513-128">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="fc513-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc513-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc513-129">Request</span></span>
<span data-ttu-id="fc513-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fc513-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="fc513-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc513-131">Response</span></span>
<span data-ttu-id="fc513-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc513-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
