# <a name="update-chartgridlines"></a><span data-ttu-id="ff8ce-101">ChartGridlines aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ff8ce-101">Update chartgridlines</span></span>

<span data-ttu-id="ff8ce-102">Dient zum Aktualisieren der Eigenschaften des ChartGridlines-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-102">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff8ce-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ff8ce-103">Permissions</span></span>
<span data-ttu-id="ff8ce-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ff8ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ff8ce-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff8ce-106">Permission type</span></span>      | <span data-ttu-id="ff8ce-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff8ce-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff8ce-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff8ce-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ff8ce-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff8ce-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ff8ce-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff8ce-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff8ce-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff8ce-111">Not supported.</span></span>    |
|<span data-ttu-id="ff8ce-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff8ce-112">Application</span></span> | <span data-ttu-id="ff8ce-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff8ce-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff8ce-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff8ce-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/minorgridlines
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/majorgridlines
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/majorgridlines
```
## <a name="optional-request-headers"></a><span data-ttu-id="ff8ce-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff8ce-115">Optional request headers</span></span>
| <span data-ttu-id="ff8ce-116">Name</span><span class="sxs-lookup"><span data-stu-id="ff8ce-116">Name</span></span>       | <span data-ttu-id="ff8ce-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff8ce-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ff8ce-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff8ce-118">Authorization</span></span>  | <span data-ttu-id="ff8ce-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff8ce-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff8ce-121">Request body</span></span>
<span data-ttu-id="ff8ce-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ff8ce-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff8ce-125">Property</span></span>     | <span data-ttu-id="ff8ce-126">Typ</span><span class="sxs-lookup"><span data-stu-id="ff8ce-126">Type</span></span>   |<span data-ttu-id="ff8ce-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff8ce-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff8ce-128">visible</span><span class="sxs-lookup"><span data-stu-id="ff8ce-128">visible</span></span>|<span data-ttu-id="ff8ce-129">boolean</span><span class="sxs-lookup"><span data-stu-id="ff8ce-129">boolean</span></span>|<span data-ttu-id="ff8ce-130">Boolescher Wert, der angibt, ob die Achsengitternetzlinien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-130">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="ff8ce-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff8ce-131">Response</span></span>

<span data-ttu-id="ff8ce-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartGridlines](../resources/chartgridlines.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-132">If successful, this method returns a `200 OK` response code and updated [ChartGridlines](../resources/chartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff8ce-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff8ce-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff8ce-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff8ce-134">Request</span></span>
<span data-ttu-id="ff8ce-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartgridlines"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/minorgridlines
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="ff8ce-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff8ce-136">Response</span></span>
<span data-ttu-id="ff8ce-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff8ce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartGridLines"
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