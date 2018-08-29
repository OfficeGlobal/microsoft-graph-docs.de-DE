# <a name="workbookrangeview-itemat"></a><span data-ttu-id="beca7-101">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="beca7-101">workbookRangeView: itemAt</span></span>


## <a name="permissions"></a><span data-ttu-id="beca7-102">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="beca7-102">Permissions</span></span>
<span data-ttu-id="beca7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="beca7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="beca7-105">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="beca7-105">Permission type</span></span>      | <span data-ttu-id="beca7-106">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="beca7-106">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="beca7-107">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="beca7-107">Delegated (work or school account)</span></span> | <span data-ttu-id="beca7-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="beca7-108">Files.ReadWrite</span></span> |
|<span data-ttu-id="beca7-109">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="beca7-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beca7-110">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beca7-110">Not supported.</span></span>    |
|<span data-ttu-id="beca7-111">Anwendung</span><span class="sxs-lookup"><span data-stu-id="beca7-111">Application</span></span> | <span data-ttu-id="beca7-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beca7-112">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="beca7-113">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="beca7-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="beca7-114">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="beca7-114">Request headers</span></span>
| <span data-ttu-id="beca7-115">Name</span><span class="sxs-lookup"><span data-stu-id="beca7-115">Name</span></span>       | <span data-ttu-id="beca7-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="beca7-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="beca7-117">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="beca7-117">Authorization</span></span>  | <span data-ttu-id="beca7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="beca7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="beca7-120">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="beca7-120">Workbook-Session-Id</span></span>  | <span data-ttu-id="beca7-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="beca7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="beca7-123">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="beca7-123">Function parameters</span></span>
<span data-ttu-id="beca7-124">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="beca7-124">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="beca7-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="beca7-125">Parameter</span></span>    | <span data-ttu-id="beca7-126">Typ</span><span class="sxs-lookup"><span data-stu-id="beca7-126">Type</span></span>   |<span data-ttu-id="beca7-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="beca7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="beca7-128">Index</span><span class="sxs-lookup"><span data-stu-id="beca7-128">index</span></span>|<span data-ttu-id="beca7-129">Int32</span><span class="sxs-lookup"><span data-stu-id="beca7-129">Int32</span></span>|<span data-ttu-id="beca7-130">Index des Elements, das zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="beca7-130">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="beca7-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="beca7-131">Response</span></span>

<span data-ttu-id="beca7-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [workbookRangeView](../resources/workbookrangeview.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="beca7-132">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beca7-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="beca7-133">Example</span></span>
<span data-ttu-id="beca7-134">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="beca7-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="beca7-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="beca7-135">Request</span></span>
<span data-ttu-id="beca7-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="beca7-136">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="beca7-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="beca7-137">Response</span></span>
<span data-ttu-id="beca7-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="beca7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
