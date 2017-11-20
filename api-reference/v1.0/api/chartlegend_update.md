# <a name="update-chartlegend"></a><span data-ttu-id="a156c-101">ChartLegend aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a156c-101">Update chartlegend</span></span>

<span data-ttu-id="a156c-102">Dient zum Aktualisieren der Eigenschaften des ChartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a156c-102">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a156c-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a156c-103">Permissions</span></span>
<span data-ttu-id="a156c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a156c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a156c-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a156c-106">Permission type</span></span>      | <span data-ttu-id="a156c-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a156c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a156c-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a156c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a156c-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a156c-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a156c-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a156c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a156c-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a156c-111">Not supported.</span></span>    |
|<span data-ttu-id="a156c-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a156c-112">Application</span></span> | <span data-ttu-id="a156c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a156c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a156c-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a156c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="a156c-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a156c-115">Optional request headers</span></span>
| <span data-ttu-id="a156c-116">Name</span><span class="sxs-lookup"><span data-stu-id="a156c-116">Name</span></span>       | <span data-ttu-id="a156c-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a156c-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a156c-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="a156c-118">Authorization</span></span>  | <span data-ttu-id="a156c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a156c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a156c-121">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="a156c-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="a156c-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="a156c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a156c-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a156c-124">Request body</span></span>
<span data-ttu-id="a156c-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="a156c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a156c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a156c-128">Property</span></span>     | <span data-ttu-id="a156c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a156c-129">Type</span></span>   |<span data-ttu-id="a156c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a156c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a156c-131">Overlay</span><span class="sxs-lookup"><span data-stu-id="a156c-131">overlay</span></span>|<span data-ttu-id="a156c-132">boolean</span><span class="sxs-lookup"><span data-stu-id="a156c-132">boolean</span></span>|<span data-ttu-id="a156c-133">Boolescher Wert, der angibt, ob die Diagrammlegende mit dem Text des Diagramms überlappen soll.</span><span class="sxs-lookup"><span data-stu-id="a156c-133">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="a156c-134">Position</span><span class="sxs-lookup"><span data-stu-id="a156c-134">position</span></span>|<span data-ttu-id="a156c-135">string</span><span class="sxs-lookup"><span data-stu-id="a156c-135">string</span></span>|<span data-ttu-id="a156c-p105">Gibt die Position der Legende im Diagramm an. Mögliche Werte: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="a156c-p105">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="a156c-138">visible</span><span class="sxs-lookup"><span data-stu-id="a156c-138">visible</span></span>|<span data-ttu-id="a156c-139">boolean</span><span class="sxs-lookup"><span data-stu-id="a156c-139">boolean</span></span>|<span data-ttu-id="a156c-140">Ein boolescher Wert, der die Sichtbarkeit eines ChartLegend-Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="a156c-140">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="a156c-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="a156c-141">Response</span></span>

<span data-ttu-id="a156c-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartLegend](../resources/chartlegend.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a156c-142">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a156c-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a156c-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a156c-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a156c-144">Request</span></span>
<span data-ttu-id="a156c-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a156c-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="a156c-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="a156c-146">Response</span></span>
<span data-ttu-id="a156c-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a156c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLegend"
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