# <a name="update-chartgridlines"></a><span data-ttu-id="413e6-101">ChartGridlines aktualisieren</span><span class="sxs-lookup"><span data-stu-id="413e6-101">Update chartgridlines</span></span>

<span data-ttu-id="413e6-102">Dient zum Aktualisieren der Eigenschaften des ChartGridlines-Objekts.</span><span class="sxs-lookup"><span data-stu-id="413e6-102">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="413e6-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="413e6-103">Permissions</span></span>
<span data-ttu-id="413e6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="413e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="413e6-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="413e6-106">Permission type</span></span>      | <span data-ttu-id="413e6-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="413e6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="413e6-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="413e6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="413e6-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="413e6-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="413e6-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="413e6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="413e6-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="413e6-111">Not supported.</span></span>    |
|<span data-ttu-id="413e6-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="413e6-112">Application</span></span> | <span data-ttu-id="413e6-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="413e6-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="413e6-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="413e6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/majorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorGridlines
```
## <a name="request-headers"></a><span data-ttu-id="413e6-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="413e6-115">Request headers</span></span>
| <span data-ttu-id="413e6-116">Name</span><span class="sxs-lookup"><span data-stu-id="413e6-116">Name</span></span>       | <span data-ttu-id="413e6-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="413e6-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="413e6-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="413e6-118">Authorization</span></span>  | <span data-ttu-id="413e6-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="413e6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="413e6-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="413e6-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="413e6-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="413e6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="413e6-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="413e6-124">Request body</span></span>
<span data-ttu-id="413e6-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="413e6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="413e6-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="413e6-128">Property</span></span>     | <span data-ttu-id="413e6-129">Typ</span><span class="sxs-lookup"><span data-stu-id="413e6-129">Type</span></span>   |<span data-ttu-id="413e6-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="413e6-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="413e6-131">sichtbar</span><span class="sxs-lookup"><span data-stu-id="413e6-131">visible</span></span>|<span data-ttu-id="413e6-132">boolesch</span><span class="sxs-lookup"><span data-stu-id="413e6-132">boolean</span></span>|<span data-ttu-id="413e6-133">Boolescher Wert, der angibt, ob die Achsengitternetzlinien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="413e6-133">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="413e6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="413e6-134">Response</span></span>

<span data-ttu-id="413e6-135">Wenn erfolgreich, gibt diese Methode einen `200 OK` Antwortcode und ein aktualisiertes [WorkbookChartGridlines](../resources/chartgridlines.md) -Objekt zurück.</span><span class="sxs-lookup"><span data-stu-id="413e6-135">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/chartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="413e6-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="413e6-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="413e6-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="413e6-137">Request</span></span>
<span data-ttu-id="413e6-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="413e6-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartgridlines"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="413e6-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="413e6-139">Response</span></span>
<span data-ttu-id="413e6-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="413e6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartGridlines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartgridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->