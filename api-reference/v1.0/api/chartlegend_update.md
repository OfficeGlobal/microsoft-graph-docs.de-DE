# <a name="update-chartlegend"></a><span data-ttu-id="5d138-101">ChartLegend aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5d138-101">Update chartlegend</span></span>

<span data-ttu-id="5d138-102">Dient zum Aktualisieren der Eigenschaften des ChartLegend-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5d138-102">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d138-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5d138-103">Permissions</span></span>
<span data-ttu-id="5d138-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d138-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5d138-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d138-106">Permission type</span></span>      | <span data-ttu-id="5d138-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d138-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d138-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d138-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5d138-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d138-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5d138-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d138-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d138-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d138-111">Not supported.</span></span>    |
|<span data-ttu-id="5d138-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d138-112">Application</span></span> | <span data-ttu-id="5d138-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d138-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d138-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d138-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="5d138-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d138-115">Optional request headers</span></span>
| <span data-ttu-id="5d138-116">Name</span><span class="sxs-lookup"><span data-stu-id="5d138-116">Name</span></span>       | <span data-ttu-id="5d138-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d138-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5d138-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d138-118">Authorization</span></span>  | <span data-ttu-id="5d138-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5d138-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d138-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d138-121">Request body</span></span>
<span data-ttu-id="5d138-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="5d138-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5d138-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d138-125">Property</span></span>     | <span data-ttu-id="5d138-126">Typ</span><span class="sxs-lookup"><span data-stu-id="5d138-126">Type</span></span>   |<span data-ttu-id="5d138-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d138-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d138-128">Overlay</span><span class="sxs-lookup"><span data-stu-id="5d138-128">overlay</span></span>|<span data-ttu-id="5d138-129">boolean</span><span class="sxs-lookup"><span data-stu-id="5d138-129">boolean</span></span>|<span data-ttu-id="5d138-130">Boolescher Wert, der angibt, ob die Diagrammlegende mit dem Text des Diagramms überlappen soll.</span><span class="sxs-lookup"><span data-stu-id="5d138-130">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="5d138-131">Position</span><span class="sxs-lookup"><span data-stu-id="5d138-131">position</span></span>|<span data-ttu-id="5d138-132">string</span><span class="sxs-lookup"><span data-stu-id="5d138-132">string</span></span>|<span data-ttu-id="5d138-p104">Gibt die Position der Legende im Diagramm an. Mögliche Werte: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="5d138-p104">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="5d138-135">visible</span><span class="sxs-lookup"><span data-stu-id="5d138-135">visible</span></span>|<span data-ttu-id="5d138-136">boolean</span><span class="sxs-lookup"><span data-stu-id="5d138-136">boolean</span></span>|<span data-ttu-id="5d138-137">Ein boolescher Wert, der die Sichtbarkeit eines ChartLegend-Objekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="5d138-137">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="5d138-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d138-138">Response</span></span>

<span data-ttu-id="5d138-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartLegend](../resources/chartlegend.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d138-139">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d138-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d138-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d138-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d138-141">Request</span></span>
<span data-ttu-id="5d138-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d138-142">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="5d138-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d138-143">Response</span></span>
<span data-ttu-id="5d138-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d138-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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