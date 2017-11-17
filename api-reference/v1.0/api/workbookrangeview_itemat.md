# <a name="workbookrangeview-itemat"></a><span data-ttu-id="c7cbf-101">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="c7cbf-101">workbookRangeView: itemAt</span></span>


## <a name="permissions"></a><span data-ttu-id="c7cbf-102">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c7cbf-102">Permissions</span></span>
<span data-ttu-id="c7cbf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7cbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c7cbf-105">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c7cbf-105">Permission type</span></span>      | <span data-ttu-id="c7cbf-106">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c7cbf-106">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7cbf-107">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c7cbf-107">Delegated (work or school account)</span></span> | <span data-ttu-id="c7cbf-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7cbf-108">Files.ReadWrite</span></span> |
|<span data-ttu-id="c7cbf-109">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c7cbf-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7cbf-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7cbf-110">Not supported.</span></span>    |
|<span data-ttu-id="c7cbf-111">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c7cbf-111">Application</span></span> | <span data-ttu-id="c7cbf-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7cbf-112">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7cbf-113">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7cbf-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="c7cbf-114">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c7cbf-114">Request headers</span></span>
| <span data-ttu-id="c7cbf-115">Name</span><span class="sxs-lookup"><span data-stu-id="c7cbf-115">Name</span></span>       | <span data-ttu-id="c7cbf-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7cbf-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c7cbf-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7cbf-117">Authorization</span></span>  | <span data-ttu-id="c7cbf-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c7cbf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7cbf-120">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c7cbf-120">Workbook-Session-Id</span></span>  | <span data-ttu-id="c7cbf-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c7cbf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7cbf-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c7cbf-123">Request body</span></span>
<span data-ttu-id="c7cbf-124">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="c7cbf-124">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="c7cbf-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="c7cbf-125">Parameter</span></span>    | <span data-ttu-id="c7cbf-126">Typ</span><span class="sxs-lookup"><span data-stu-id="c7cbf-126">Type</span></span>   |<span data-ttu-id="c7cbf-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7cbf-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7cbf-128">Index</span><span class="sxs-lookup"><span data-stu-id="c7cbf-128">index</span></span>|<span data-ttu-id="c7cbf-129">Int32</span><span class="sxs-lookup"><span data-stu-id="c7cbf-129">Int32</span></span>|<span data-ttu-id="c7cbf-130">Index des Elements, das zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="c7cbf-130">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="c7cbf-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7cbf-131">Response</span></span>

<span data-ttu-id="c7cbf-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRangeView](../resources/workbookrangeview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7cbf-132">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7cbf-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c7cbf-133">Example</span></span>
<span data-ttu-id="c7cbf-134">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c7cbf-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c7cbf-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7cbf-135">Request</span></span>
<span data-ttu-id="c7cbf-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c7cbf-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="c7cbf-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7cbf-137">Response</span></span>
<span data-ttu-id="c7cbf-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7cbf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
