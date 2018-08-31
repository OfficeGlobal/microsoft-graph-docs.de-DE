# <a name="update-chartlegend"></a><span data-ttu-id="c98d8-101">ChartLegend aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c98d8-101">Update chartlegend</span></span>

<span data-ttu-id="c98d8-102">Dient zum Aktualisieren der Eigenschaften des ChartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c98d8-102">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c98d8-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c98d8-103">Permissions</span></span>
<span data-ttu-id="c98d8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c98d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c98d8-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c98d8-106">Permission type</span></span>      | <span data-ttu-id="c98d8-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c98d8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c98d8-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c98d8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c98d8-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c98d8-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c98d8-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c98d8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c98d8-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c98d8-111">Not supported.</span></span>    |
|<span data-ttu-id="c98d8-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c98d8-112">Application</span></span> | <span data-ttu-id="c98d8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c98d8-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c98d8-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c98d8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="c98d8-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c98d8-115">Optional request headers</span></span>
| <span data-ttu-id="c98d8-116">Name</span><span class="sxs-lookup"><span data-stu-id="c98d8-116">Name</span></span>       | <span data-ttu-id="c98d8-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c98d8-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c98d8-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c98d8-118">Authorization</span></span>  | <span data-ttu-id="c98d8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c98d8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c98d8-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="c98d8-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="c98d8-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="c98d8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c98d8-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c98d8-124">Request body</span></span>
<span data-ttu-id="c98d8-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="c98d8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c98d8-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c98d8-128">Property</span></span>     | <span data-ttu-id="c98d8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c98d8-129">Type</span></span>   |<span data-ttu-id="c98d8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c98d8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c98d8-131">Overlay</span><span class="sxs-lookup"><span data-stu-id="c98d8-131">overlay</span></span>|<span data-ttu-id="c98d8-132">boolean</span><span class="sxs-lookup"><span data-stu-id="c98d8-132">boolean</span></span>|<span data-ttu-id="c98d8-133">Boolescher Wert, der angibt, ob die Diagrammlegende mit dem Text des Diagramms überlappen soll.</span><span class="sxs-lookup"><span data-stu-id="c98d8-133">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="c98d8-134">Position</span><span class="sxs-lookup"><span data-stu-id="c98d8-134">position</span></span>|<span data-ttu-id="c98d8-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c98d8-135">string</span></span>|<span data-ttu-id="c98d8-136">Gibt die Position der Legende im Diagramm an.</span><span class="sxs-lookup"><span data-stu-id="c98d8-136">Represents the position of the legend on the chart. Possible values are: , , , , , .</span></span> <span data-ttu-id="c98d8-137">Mögliche Werte: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="c98d8-137">The possible values are `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`, , , , , , or .</span></span>|
|<span data-ttu-id="c98d8-138">sichtbar</span><span class="sxs-lookup"><span data-stu-id="c98d8-138">visible</span></span>|<span data-ttu-id="c98d8-139">boolean</span><span class="sxs-lookup"><span data-stu-id="c98d8-139">boolean</span></span>|<span data-ttu-id="c98d8-140">Ein boolescher Wert, der die Sichtbarkeit eines ChartLegend-Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="c98d8-140">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="c98d8-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="c98d8-141">Response</span></span>

<span data-ttu-id="c98d8-142">Wenn das Verfahren erfolgreich verläuft, werden im Antworttext der Antwortcode `200 OK` und ein [WorkbookChartLegend](../resources/chartlegend.md)-Objekt zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c98d8-142">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c98d8-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c98d8-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c98d8-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c98d8-144">Request</span></span>
<span data-ttu-id="c98d8-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c98d8-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="c98d8-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="c98d8-146">Response</span></span>
<span data-ttu-id="c98d8-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c98d8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->