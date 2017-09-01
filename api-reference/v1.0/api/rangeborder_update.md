# <a name="update-rangeborder"></a><span data-ttu-id="eb669-101">rangeborder aktualisieren</span><span class="sxs-lookup"><span data-stu-id="eb669-101">Update rangeborder</span></span>

<span data-ttu-id="eb669-102">Dient zum Aktualisieren der Eigenschaften des rangeborder-Objekts.</span><span class="sxs-lookup"><span data-stu-id="eb669-102">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb669-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eb669-103">Permissions</span></span>
<span data-ttu-id="eb669-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eb669-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eb669-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb669-106">Permission type</span></span>      | <span data-ttu-id="eb669-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb669-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb669-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb669-108">Delegated (work or school account)</span></span> | <span data-ttu-id="eb669-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb669-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eb669-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb669-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb669-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb669-111">Not supported.</span></span>    |
|<span data-ttu-id="eb669-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb669-112">Application</span></span> | <span data-ttu-id="eb669-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb669-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb669-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb669-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="eb669-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb669-115">Optional request headers</span></span>
| <span data-ttu-id="eb669-116">Name</span><span class="sxs-lookup"><span data-stu-id="eb669-116">Name</span></span>       | <span data-ttu-id="eb669-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb669-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="eb669-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb669-118">Authorization</span></span>  | <span data-ttu-id="eb669-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eb669-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb669-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb669-121">Request body</span></span>
<span data-ttu-id="eb669-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="eb669-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eb669-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eb669-125">Property</span></span>     | <span data-ttu-id="eb669-126">Typ</span><span class="sxs-lookup"><span data-stu-id="eb669-126">Type</span></span>   |<span data-ttu-id="eb669-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb669-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb669-128">color</span><span class="sxs-lookup"><span data-stu-id="eb669-128">color</span></span>|<span data-ttu-id="eb669-129">string</span><span class="sxs-lookup"><span data-stu-id="eb669-129">string</span></span>|<span data-ttu-id="eb669-130">HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.</span><span class="sxs-lookup"><span data-stu-id="eb669-130">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="eb669-131">style</span><span class="sxs-lookup"><span data-stu-id="eb669-131">style</span></span>|<span data-ttu-id="eb669-132">string</span><span class="sxs-lookup"><span data-stu-id="eb669-132">string</span></span>|<span data-ttu-id="eb669-p104">Eine der Konstanten der Linienart, die die Linienart für den Rahmen angibt. Mögliche Werte: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="eb669-p104">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="eb669-135">weight</span><span class="sxs-lookup"><span data-stu-id="eb669-135">weight</span></span>|<span data-ttu-id="eb669-136">string</span><span class="sxs-lookup"><span data-stu-id="eb669-136">string</span></span>|<span data-ttu-id="eb669-p105">Gibt die Stärke des Rahmens um einen Bereich an. Mögliche Werte: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="eb669-p105">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="eb669-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb669-139">Response</span></span>

<span data-ttu-id="eb669-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [RangeBorder](../resources/rangeborder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb669-140">If successful, this method returns a `200 OK` response code and updated [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eb669-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb669-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb669-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb669-142">Request</span></span>
<span data-ttu-id="eb669-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb669-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/borders(<sideIndex>)
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="eb669-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb669-144">Response</span></span>
<span data-ttu-id="eb669-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb669-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->