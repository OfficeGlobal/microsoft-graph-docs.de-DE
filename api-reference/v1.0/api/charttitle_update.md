# <a name="update-charttitle"></a><span data-ttu-id="948e7-101">ChartTitle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="948e7-101">Update charttitle</span></span>

<span data-ttu-id="948e7-102">Dient zum Aktualisieren der Eigenschaften des ChartTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="948e7-102">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="948e7-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="948e7-103">Permissions</span></span>
<span data-ttu-id="948e7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="948e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="948e7-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="948e7-106">Permission type</span></span>      | <span data-ttu-id="948e7-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="948e7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="948e7-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="948e7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="948e7-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="948e7-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="948e7-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="948e7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="948e7-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="948e7-111">Not supported.</span></span>    |
|<span data-ttu-id="948e7-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="948e7-112">Application</span></span> | <span data-ttu-id="948e7-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="948e7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="948e7-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="948e7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="948e7-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="948e7-115">Optional request headers</span></span>
| <span data-ttu-id="948e7-116">Name</span><span class="sxs-lookup"><span data-stu-id="948e7-116">Name</span></span>       | <span data-ttu-id="948e7-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="948e7-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="948e7-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="948e7-118">Authorization</span></span>  | <span data-ttu-id="948e7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="948e7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="948e7-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="948e7-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="948e7-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="948e7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="948e7-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="948e7-124">Request body</span></span>
<span data-ttu-id="948e7-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="948e7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="948e7-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="948e7-128">Property</span></span>     | <span data-ttu-id="948e7-129">Typ</span><span class="sxs-lookup"><span data-stu-id="948e7-129">Type</span></span>   |<span data-ttu-id="948e7-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="948e7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="948e7-131">Overlay</span><span class="sxs-lookup"><span data-stu-id="948e7-131">overlay</span></span>|<span data-ttu-id="948e7-132">boolesch</span><span class="sxs-lookup"><span data-stu-id="948e7-132">boolean</span></span>|<span data-ttu-id="948e7-133">Boolescher Wert, der angibt, ob der Diagrammtitel das Diagramm überlagert.</span><span class="sxs-lookup"><span data-stu-id="948e7-133">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="948e7-134">Text</span><span class="sxs-lookup"><span data-stu-id="948e7-134">text</span></span>|<span data-ttu-id="948e7-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="948e7-135">string</span></span>|<span data-ttu-id="948e7-136">Stellt den Titeltext eines Diagramms dar.</span><span class="sxs-lookup"><span data-stu-id="948e7-136">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="948e7-137">sichtbar</span><span class="sxs-lookup"><span data-stu-id="948e7-137">visible</span></span>|<span data-ttu-id="948e7-138">boolesch</span><span class="sxs-lookup"><span data-stu-id="948e7-138">boolean</span></span>|<span data-ttu-id="948e7-139">Ein boolescher Wert, der die Sichtbarkeit eines Diagrammtitelobjekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="948e7-139">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="948e7-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="948e7-140">Response</span></span>

<span data-ttu-id="948e7-141">Wenn erfolgreich, gibt diese Methode einen `200 OK` Antwortcode und ein aktualisiertes [WorkbookChartTitle](../resources/charttitle.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="948e7-141">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="948e7-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="948e7-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="948e7-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="948e7-143">Request</span></span>
<span data-ttu-id="948e7-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="948e7-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="948e7-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="948e7-145">Response</span></span>
<span data-ttu-id="948e7-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="948e7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->