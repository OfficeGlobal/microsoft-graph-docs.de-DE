# <a name="chartcollection-add"></a><span data-ttu-id="0e955-101">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="0e955-101">ChartCollection: add</span></span>

<span data-ttu-id="0e955-102">Erstellt ein neues Diagramm.</span><span class="sxs-lookup"><span data-stu-id="0e955-102">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e955-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0e955-103">Permissions</span></span>
<span data-ttu-id="0e955-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0e955-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0e955-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e955-106">Permission type</span></span>      | <span data-ttu-id="0e955-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e955-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e955-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e955-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0e955-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e955-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e955-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e955-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e955-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e955-111">Not supported.</span></span>    |
|<span data-ttu-id="0e955-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e955-112">Application</span></span> | <span data-ttu-id="0e955-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e955-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e955-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e955-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="0e955-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e955-115">Request headers</span></span>
| <span data-ttu-id="0e955-116">Name</span><span class="sxs-lookup"><span data-stu-id="0e955-116">Name</span></span>       | <span data-ttu-id="0e955-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e955-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0e955-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e955-118">Authorization</span></span>  | <span data-ttu-id="0e955-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0e955-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e955-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e955-121">Request body</span></span>
<span data-ttu-id="0e955-122">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="0e955-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0e955-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="0e955-123">Parameter</span></span>    | <span data-ttu-id="0e955-124">Typ</span><span class="sxs-lookup"><span data-stu-id="0e955-124">Type</span></span>   |<span data-ttu-id="0e955-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e955-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e955-126">type</span><span class="sxs-lookup"><span data-stu-id="0e955-126">type</span></span>|<span data-ttu-id="0e955-127">string</span><span class="sxs-lookup"><span data-stu-id="0e955-127">string</span></span>|<span data-ttu-id="0e955-p103">Stellt die Art des Diagramms dar.  Mögliche Werte: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span><span class="sxs-lookup"><span data-stu-id="0e955-p103">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="0e955-130">sourceData</span><span class="sxs-lookup"><span data-stu-id="0e955-130">sourceData</span></span>|<span data-ttu-id="0e955-131">string</span><span class="sxs-lookup"><span data-stu-id="0e955-131">string</span></span>|<span data-ttu-id="0e955-132">Das den Quelldaten entsprechende Range-Objekt.</span><span class="sxs-lookup"><span data-stu-id="0e955-132">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="0e955-133">seriesBy</span><span class="sxs-lookup"><span data-stu-id="0e955-133">seriesBy</span></span>|<span data-ttu-id="0e955-134">string</span><span class="sxs-lookup"><span data-stu-id="0e955-134">string</span></span>|<span data-ttu-id="0e955-p104">Optional. Gibt an, wie Spalten oder Zeilen als Datenreihen im Diagramm verwendet werden.  Mögliche Werte: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="0e955-p104">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="0e955-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e955-138">Response</span></span>

<span data-ttu-id="0e955-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [Chart](../resources/chart.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e955-139">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e955-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e955-140">Example</span></span>
<span data-ttu-id="0e955-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="0e955-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0e955-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e955-142">Request</span></span>
<span data-ttu-id="0e955-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e955-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0e955-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e955-144">Response</span></span>
<span data-ttu-id="0e955-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e955-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
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
