# <a name="update-icon"></a><span data-ttu-id="9d515-101">Update-Symbol</span><span class="sxs-lookup"><span data-stu-id="9d515-101">Update icon</span></span>

<span data-ttu-id="9d515-102">Dient zum Aktualisieren der Eigenschaften des Symbolobjekts.</span><span class="sxs-lookup"><span data-stu-id="9d515-102">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9d515-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9d515-103">Permissions</span></span>
<span data-ttu-id="9d515-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d515-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d515-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9d515-106">Permission type</span></span>      | <span data-ttu-id="9d515-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9d515-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="9d515-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9d515-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9d515-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d515-109">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="9d515-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9d515-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d515-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d515-111">Not supported.</span></span>    | 
|<span data-ttu-id="9d515-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9d515-112">Application</span></span> | <span data-ttu-id="9d515-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d515-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9d515-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d515-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="9d515-115">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9d515-115">Optional request headers</span></span>
| <span data-ttu-id="9d515-116">Name</span><span class="sxs-lookup"><span data-stu-id="9d515-116">Name</span></span>       | <span data-ttu-id="9d515-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d515-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9d515-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9d515-118">Authorization</span></span>  | <span data-ttu-id="9d515-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9d515-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="9d515-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9d515-121">Request body</span></span>
<span data-ttu-id="9d515-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="9d515-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9d515-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9d515-125">Property</span></span>     | <span data-ttu-id="9d515-126">Typ</span><span class="sxs-lookup"><span data-stu-id="9d515-126">Type</span></span>   |<span data-ttu-id="9d515-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d515-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d515-128">Index</span><span class="sxs-lookup"><span data-stu-id="9d515-128">index</span></span>|<span data-ttu-id="9d515-129">int</span><span class="sxs-lookup"><span data-stu-id="9d515-129">int</span></span>|<span data-ttu-id="9d515-130">Stellt den Index des Symbols im angegebenen Satz dar.</span><span class="sxs-lookup"><span data-stu-id="9d515-130">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="9d515-131">Gruppe</span><span class="sxs-lookup"><span data-stu-id="9d515-131">set</span></span>|<span data-ttu-id="9d515-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9d515-132">string</span></span>|<span data-ttu-id="9d515-133">Repräsentiert die Gruppe, zu der das Symbol gehört.</span><span class="sxs-lookup"><span data-stu-id="9d515-133">Represents the set that the icon is part of. Possible values are: , , , , , , , , , , , , , , , , , , , , .</span></span> <span data-ttu-id="9d515-134">Die möglichen Werte sind: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="9d515-134">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="9d515-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d515-135">Response</span></span>

<span data-ttu-id="9d515-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [Icon](../resources/icon.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d515-136">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d515-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9d515-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d515-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d515-138">Request</span></span>
<span data-ttu-id="9d515-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9d515-139">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="9d515-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d515-140">Response</span></span>
<span data-ttu-id="9d515-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d515-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookIcon"
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