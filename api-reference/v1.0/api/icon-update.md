---
title: Update-Symbol
description: Dient zum Aktualisieren der Eigenschaften des Symbolobjekts.
ms.openlocfilehash: 0cb3b1af0369c86290c842232acc57792d1552ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019556"
---
# <a name="update-icon"></a><span data-ttu-id="28d9b-103">Update-Symbol</span><span class="sxs-lookup"><span data-stu-id="28d9b-103">Update icon</span></span>

<span data-ttu-id="28d9b-104">Dient zum Aktualisieren der Eigenschaften des Symbolobjekts.</span><span class="sxs-lookup"><span data-stu-id="28d9b-104">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="28d9b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="28d9b-105">Permissions</span></span>
<span data-ttu-id="28d9b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28d9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28d9b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28d9b-108">Permission type</span></span>      | <span data-ttu-id="28d9b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28d9b-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="28d9b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28d9b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="28d9b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28d9b-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="28d9b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28d9b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28d9b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28d9b-113">Not supported.</span></span>    | 
|<span data-ttu-id="28d9b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28d9b-114">Application</span></span> | <span data-ttu-id="28d9b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28d9b-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="28d9b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28d9b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="28d9b-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28d9b-117">Optional request headers</span></span>
| <span data-ttu-id="28d9b-118">Name</span><span class="sxs-lookup"><span data-stu-id="28d9b-118">Name</span></span>       | <span data-ttu-id="28d9b-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28d9b-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="28d9b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="28d9b-120">Authorization</span></span>  | <span data-ttu-id="28d9b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="28d9b-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="28d9b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28d9b-123">Request body</span></span>
<span data-ttu-id="28d9b-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="28d9b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="28d9b-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28d9b-127">Property</span></span>     | <span data-ttu-id="28d9b-128">Typ</span><span class="sxs-lookup"><span data-stu-id="28d9b-128">Type</span></span>   |<span data-ttu-id="28d9b-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28d9b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28d9b-130">Index</span><span class="sxs-lookup"><span data-stu-id="28d9b-130">index</span></span>|<span data-ttu-id="28d9b-131">int</span><span class="sxs-lookup"><span data-stu-id="28d9b-131">int</span></span>|<span data-ttu-id="28d9b-132">Stellt den Index des Symbols im angegebenen Satz dar.</span><span class="sxs-lookup"><span data-stu-id="28d9b-132">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="28d9b-133">set</span><span class="sxs-lookup"><span data-stu-id="28d9b-133">set</span></span>|<span data-ttu-id="28d9b-134">string</span><span class="sxs-lookup"><span data-stu-id="28d9b-134">string</span></span>|<span data-ttu-id="28d9b-135">Repräsentiert den Satz an, dem das Symbol gehört.</span><span class="sxs-lookup"><span data-stu-id="28d9b-135">Represents the set that the icon is part of.</span></span> <span data-ttu-id="28d9b-136">Die möglichen Werte sind: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars` , `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="28d9b-136">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="28d9b-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="28d9b-137">Response</span></span>

<span data-ttu-id="28d9b-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [Icon](../resources/icon.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28d9b-138">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="28d9b-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28d9b-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28d9b-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28d9b-140">Request</span></span>
<span data-ttu-id="28d9b-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28d9b-141">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="28d9b-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="28d9b-142">Response</span></span>
<span data-ttu-id="28d9b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28d9b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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