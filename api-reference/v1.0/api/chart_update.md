# <a name="update-chart"></a><span data-ttu-id="1e78e-101">Diagramm aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1e78e-101">Update chart</span></span>

<span data-ttu-id="1e78e-102">Dient zum Aktualisieren der Eigenschaften des Diagrammobjekts.</span><span class="sxs-lookup"><span data-stu-id="1e78e-102">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e78e-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1e78e-103">Permissions</span></span>
<span data-ttu-id="1e78e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1e78e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1e78e-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1e78e-106">Permission type</span></span>      | <span data-ttu-id="1e78e-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1e78e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e78e-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1e78e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1e78e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e78e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1e78e-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1e78e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e78e-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e78e-111">Not supported.</span></span>    |
|<span data-ttu-id="1e78e-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1e78e-112">Application</span></span> | <span data-ttu-id="1e78e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e78e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e78e-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e78e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1e78e-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1e78e-115">Optional request headers</span></span>
| <span data-ttu-id="1e78e-116">Name</span><span class="sxs-lookup"><span data-stu-id="1e78e-116">Name</span></span>       | <span data-ttu-id="1e78e-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e78e-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1e78e-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1e78e-118">Authorization</span></span>  | <span data-ttu-id="1e78e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1e78e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e78e-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="1e78e-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="1e78e-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="1e78e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e78e-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e78e-124">Request body</span></span>
<span data-ttu-id="1e78e-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="1e78e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1e78e-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1e78e-128">Property</span></span>     | <span data-ttu-id="1e78e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="1e78e-129">Type</span></span>   |<span data-ttu-id="1e78e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e78e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e78e-131">height</span><span class="sxs-lookup"><span data-stu-id="1e78e-131">height</span></span>|<span data-ttu-id="1e78e-132">doppelt</span><span class="sxs-lookup"><span data-stu-id="1e78e-132">double</span></span>|<span data-ttu-id="1e78e-133">Die Höhe des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="1e78e-133">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="1e78e-134">left</span><span class="sxs-lookup"><span data-stu-id="1e78e-134">left</span></span>|<span data-ttu-id="1e78e-135">doppelt</span><span class="sxs-lookup"><span data-stu-id="1e78e-135">double</span></span>|<span data-ttu-id="1e78e-136">Der Abstand von der linken Seite des Diagramms zu dem Ursprung des Arbeitsblatts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="1e78e-136">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="1e78e-137">name</span><span class="sxs-lookup"><span data-stu-id="1e78e-137">name</span></span>|<span data-ttu-id="1e78e-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e78e-138">string</span></span>|<span data-ttu-id="1e78e-139">Gibt den Namen eines Diagrammobjekts an.</span><span class="sxs-lookup"><span data-stu-id="1e78e-139">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="1e78e-140">top</span><span class="sxs-lookup"><span data-stu-id="1e78e-140">top</span></span>|<span data-ttu-id="1e78e-141">doppelt</span><span class="sxs-lookup"><span data-stu-id="1e78e-141">double</span></span>|<span data-ttu-id="1e78e-142">Der Abstand (in Punkten) von dem oberen Rand des Objekts zum oberen Rand von Zeile 1 (auf einem Arbeitsblatt) oder zum oberen Diagrammbereich (in einem Diagramm).</span><span class="sxs-lookup"><span data-stu-id="1e78e-142">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="1e78e-143">width</span><span class="sxs-lookup"><span data-stu-id="1e78e-143">width</span></span>|<span data-ttu-id="1e78e-144">doppelt</span><span class="sxs-lookup"><span data-stu-id="1e78e-144">double</span></span>|<span data-ttu-id="1e78e-145">Die Breite des Diagrammobjekts (in Punkten).</span><span class="sxs-lookup"><span data-stu-id="1e78e-145">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="1e78e-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e78e-146">Response</span></span>

<span data-ttu-id="1e78e-147">Wenn die Methode erfolgreich verläuft, werden im Antworttext der `200 OK` Antwortcode und ein [WorkbookChart](../resources/chart.md)-Objekt zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e78e-147">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e78e-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1e78e-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e78e-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e78e-149">Request</span></span>
<span data-ttu-id="1e78e-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1e78e-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="1e78e-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e78e-151">Response</span></span>
<span data-ttu-id="1e78e-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e78e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->