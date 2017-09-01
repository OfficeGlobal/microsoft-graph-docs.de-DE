# <a name="update-charttitle"></a><span data-ttu-id="2d0df-101">ChartTitle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2d0df-101">Update charttitle</span></span>

<span data-ttu-id="2d0df-102">Dient zum Aktualisieren der Eigenschaften des ChartTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2d0df-102">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d0df-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2d0df-103">Permissions</span></span>
<span data-ttu-id="2d0df-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2d0df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2d0df-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d0df-106">Permission type</span></span>      | <span data-ttu-id="2d0df-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d0df-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d0df-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d0df-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2d0df-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d0df-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2d0df-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d0df-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d0df-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d0df-111">Not supported.</span></span>    |
|<span data-ttu-id="2d0df-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d0df-112">Application</span></span> | <span data-ttu-id="2d0df-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d0df-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d0df-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d0df-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="2d0df-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d0df-115">Optional request headers</span></span>
| <span data-ttu-id="2d0df-116">Name</span><span class="sxs-lookup"><span data-stu-id="2d0df-116">Name</span></span>       | <span data-ttu-id="2d0df-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d0df-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2d0df-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d0df-118">Authorization</span></span>  | <span data-ttu-id="2d0df-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2d0df-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d0df-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2d0df-121">Request body</span></span>
<span data-ttu-id="2d0df-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="2d0df-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2d0df-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2d0df-125">Property</span></span>     | <span data-ttu-id="2d0df-126">Typ</span><span class="sxs-lookup"><span data-stu-id="2d0df-126">Type</span></span>   |<span data-ttu-id="2d0df-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d0df-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d0df-128">Overlay</span><span class="sxs-lookup"><span data-stu-id="2d0df-128">overlay</span></span>|<span data-ttu-id="2d0df-129">boolean</span><span class="sxs-lookup"><span data-stu-id="2d0df-129">boolean</span></span>|<span data-ttu-id="2d0df-130">Boolescher Wert, der angibt, ob der Diagrammtitel das Diagramm überlagert.</span><span class="sxs-lookup"><span data-stu-id="2d0df-130">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="2d0df-131">text</span><span class="sxs-lookup"><span data-stu-id="2d0df-131">text</span></span>|<span data-ttu-id="2d0df-132">string</span><span class="sxs-lookup"><span data-stu-id="2d0df-132">string</span></span>|<span data-ttu-id="2d0df-133">Stellt den Titeltext eines Diagramms dar.</span><span class="sxs-lookup"><span data-stu-id="2d0df-133">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="2d0df-134">visible</span><span class="sxs-lookup"><span data-stu-id="2d0df-134">visible</span></span>|<span data-ttu-id="2d0df-135">boolean</span><span class="sxs-lookup"><span data-stu-id="2d0df-135">boolean</span></span>|<span data-ttu-id="2d0df-136">Ein boolescher Wert, der die Sichtbarkeit eines Diagrammtitelobjekts darstellt.</span><span class="sxs-lookup"><span data-stu-id="2d0df-136">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="2d0df-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d0df-137">Response</span></span>

<span data-ttu-id="2d0df-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartTitle](../resources/charttitle.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d0df-138">If successful, this method returns a `200 OK` response code and updated [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2d0df-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d0df-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d0df-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d0df-140">Request</span></span>
<span data-ttu-id="2d0df-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d0df-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="2d0df-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d0df-142">Response</span></span>
<span data-ttu-id="2d0df-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d0df-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartTitle"
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