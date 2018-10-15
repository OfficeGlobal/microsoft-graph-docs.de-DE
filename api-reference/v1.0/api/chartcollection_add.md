# <a name="chartcollection-add"></a><span data-ttu-id="a1d61-101">ChartCollection: hinzufügen</span><span class="sxs-lookup"><span data-stu-id="a1d61-101">ChartCollection: add</span></span>

<span data-ttu-id="a1d61-102">Erstellt ein neues Diagramm.</span><span class="sxs-lookup"><span data-stu-id="a1d61-102">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1d61-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a1d61-103">Permissions</span></span>
<span data-ttu-id="a1d61-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a1d61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a1d61-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a1d61-106">Permission type</span></span>      | <span data-ttu-id="a1d61-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a1d61-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1d61-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a1d61-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a1d61-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1d61-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a1d61-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a1d61-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1d61-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1d61-111">Not supported.</span></span>    |
|<span data-ttu-id="a1d61-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a1d61-112">Application</span></span> | <span data-ttu-id="a1d61-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1d61-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1d61-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1d61-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="a1d61-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a1d61-115">Request headers</span></span>
| <span data-ttu-id="a1d61-116">Name</span><span class="sxs-lookup"><span data-stu-id="a1d61-116">Name</span></span>       | <span data-ttu-id="a1d61-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1d61-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a1d61-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a1d61-118">Authorization</span></span>  | <span data-ttu-id="a1d61-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a1d61-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1d61-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="a1d61-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="a1d61-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="a1d61-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1d61-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a1d61-124">Request body</span></span>
<span data-ttu-id="a1d61-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="a1d61-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a1d61-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="a1d61-126">Parameter</span></span>    | <span data-ttu-id="a1d61-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a1d61-127">Type</span></span>   |<span data-ttu-id="a1d61-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1d61-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1d61-129">type</span><span class="sxs-lookup"><span data-stu-id="a1d61-129">type</span></span>|<span data-ttu-id="a1d61-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1d61-130">string</span></span>|<span data-ttu-id="a1d61-131">Stellt den Typ eines Diagramms dar.</span><span class="sxs-lookup"><span data-stu-id="a1d61-131">Represents the name of a chart object.</span></span>  <span data-ttu-id="a1d61-132">Die möglichen Werte sind: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="a1d61-132">The possible values are `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, or `PieOfPie`.</span></span>|
|<span data-ttu-id="a1d61-133">sourceData</span><span class="sxs-lookup"><span data-stu-id="a1d61-133">sourceData</span></span>|<span data-ttu-id="a1d61-134">Json</span><span class="sxs-lookup"><span data-stu-id="a1d61-134">Json</span></span>|<span data-ttu-id="a1d61-135">Das den Quelldaten entsprechende Range-Objekt.</span><span class="sxs-lookup"><span data-stu-id="a1d61-135">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="a1d61-136">seriesBy</span><span class="sxs-lookup"><span data-stu-id="a1d61-136">seriesBy</span></span>|<span data-ttu-id="a1d61-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1d61-137">string</span></span>|<span data-ttu-id="a1d61-138">Optional.</span><span class="sxs-lookup"><span data-stu-id="a1d61-138">Optional.</span></span> <span data-ttu-id="a1d61-139">Gibt an, wie die Spalten oder Zeilen als Datenreihen im Diagramm verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="a1d61-139">Returns or sets the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="a1d61-140">Mögliche Werte sind: `Auto`, `Columns`,`Rows`.</span><span class="sxs-lookup"><span data-stu-id="a1d61-140">The possible values are `Auto`, `Columns`, `Rows`, , , , , , , , , or .</span></span>|

## <a name="response"></a><span data-ttu-id="a1d61-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1d61-141">Response</span></span>

<span data-ttu-id="a1d61-142">Wenn erfolgreich, gibt diese Methode einen `200 OK` Antwortcode und ein [WorkbookChart](../resources/chart.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a1d61-142">If successful, this method returns `200 OK` response code and [groupSetting](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1d61-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1d61-143">Example</span></span>
<span data-ttu-id="a1d61-144">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="a1d61-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a1d61-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1d61-145">Request</span></span>
<span data-ttu-id="a1d61-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a1d61-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```

##### <a name="response"></a><span data-ttu-id="a1d61-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1d61-147">Response</span></span>
<span data-ttu-id="a1d61-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1d61-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
