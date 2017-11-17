# <a name="update-chartaxistitle"></a><span data-ttu-id="d02ea-101">ChartAxisTitle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d02ea-101">Update chartaxistitle</span></span>

<span data-ttu-id="d02ea-102">Dient zum Aktualisieren der Eigenschaften des ChartAxisTitle-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d02ea-102">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d02ea-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d02ea-103">Permissions</span></span>
<span data-ttu-id="d02ea-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d02ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d02ea-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d02ea-106">Permission type</span></span>      | <span data-ttu-id="d02ea-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d02ea-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d02ea-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d02ea-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d02ea-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d02ea-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d02ea-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d02ea-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d02ea-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d02ea-111">Not supported.</span></span>    |
|<span data-ttu-id="d02ea-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d02ea-112">Application</span></span> | <span data-ttu-id="d02ea-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d02ea-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d02ea-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d02ea-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="d02ea-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d02ea-115">Optional request headers</span></span>
| <span data-ttu-id="d02ea-116">Name</span><span class="sxs-lookup"><span data-stu-id="d02ea-116">Name</span></span>       | <span data-ttu-id="d02ea-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d02ea-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d02ea-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="d02ea-118">Authorization</span></span>  | <span data-ttu-id="d02ea-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d02ea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d02ea-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d02ea-121">Request body</span></span>
<span data-ttu-id="d02ea-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="d02ea-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d02ea-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d02ea-125">Property</span></span>     | <span data-ttu-id="d02ea-126">Typ</span><span class="sxs-lookup"><span data-stu-id="d02ea-126">Type</span></span>   |<span data-ttu-id="d02ea-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d02ea-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d02ea-128">text</span><span class="sxs-lookup"><span data-stu-id="d02ea-128">text</span></span>|<span data-ttu-id="d02ea-129">string</span><span class="sxs-lookup"><span data-stu-id="d02ea-129">string</span></span>|<span data-ttu-id="d02ea-130">Stellt den Achsentitel dar.</span><span class="sxs-lookup"><span data-stu-id="d02ea-130">Represents the axis title.</span></span>|
|<span data-ttu-id="d02ea-131">visible</span><span class="sxs-lookup"><span data-stu-id="d02ea-131">visible</span></span>|<span data-ttu-id="d02ea-132">boolean</span><span class="sxs-lookup"><span data-stu-id="d02ea-132">boolean</span></span>|<span data-ttu-id="d02ea-133">Ein boolescher Wert, der die Sichtbarkeit eines Achsentitels angibt.</span><span class="sxs-lookup"><span data-stu-id="d02ea-133">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="d02ea-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d02ea-134">Response</span></span>

<span data-ttu-id="d02ea-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [ChartAxisTitle](../resources/chartaxistitle.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d02ea-135">If successful, this method returns a `200 OK` response code and updated [ChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d02ea-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d02ea-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d02ea-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d02ea-137">Request</span></span>
<span data-ttu-id="d02ea-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d02ea-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="d02ea-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="d02ea-139">Response</span></span>
<span data-ttu-id="d02ea-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d02ea-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->