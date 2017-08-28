# <a name="update-icon"></a><span data-ttu-id="36180-101">Update-Symbol</span><span class="sxs-lookup"><span data-stu-id="36180-101">Update icon</span></span>

<span data-ttu-id="36180-102">Dient zum Aktualisieren der Eigenschaften des Symbolobjekts.</span><span class="sxs-lookup"><span data-stu-id="36180-102">Update the properties of icon object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36180-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="36180-103">Prerequisites</span></span>
<span data-ttu-id="36180-104">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="36180-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="36180-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36180-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="36180-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="36180-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="36180-107">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="36180-107">Optional request headers</span></span>
| <span data-ttu-id="36180-108">Name</span><span class="sxs-lookup"><span data-stu-id="36180-108">Name</span></span>       | <span data-ttu-id="36180-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36180-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="36180-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="36180-110">Authorization</span></span>  | <span data-ttu-id="36180-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="36180-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36180-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="36180-113">Request body</span></span>
<span data-ttu-id="36180-p102">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="36180-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="36180-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="36180-117">Property</span></span>     | <span data-ttu-id="36180-118">Typ</span><span class="sxs-lookup"><span data-stu-id="36180-118">Type</span></span>   |<span data-ttu-id="36180-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36180-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36180-120">Index</span><span class="sxs-lookup"><span data-stu-id="36180-120">index</span></span>|<span data-ttu-id="36180-121">int</span><span class="sxs-lookup"><span data-stu-id="36180-121">int</span></span>|<span data-ttu-id="36180-122">Stellt den Index des Symbols im angegebenen Satz dar.</span><span class="sxs-lookup"><span data-stu-id="36180-122">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="36180-123">set</span><span class="sxs-lookup"><span data-stu-id="36180-123">set</span></span>|<span data-ttu-id="36180-124">string</span><span class="sxs-lookup"><span data-stu-id="36180-124">string</span></span>|<span data-ttu-id="36180-p103">Stellt den Satz dar, zu dem das Symbol gehört. Mögliche Werte: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="36180-p103">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="36180-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="36180-127">Response</span></span>

<span data-ttu-id="36180-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [Icon](../resources/icon.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36180-128">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36180-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="36180-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36180-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="36180-130">Request</span></span>
<span data-ttu-id="36180-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36180-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_icon"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```
##### <a name="response"></a><span data-ttu-id="36180-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="36180-132">Response</span></span>
<span data-ttu-id="36180-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36180-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.icon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->