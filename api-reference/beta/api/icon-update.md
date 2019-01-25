---
title: Update-Symbol
description: Dient zum Aktualisieren der Eigenschaften des Symbolobjekts.
localization_priority: Normal
ms.openlocfilehash: 995c67a54e6394e23ef58cc3dc730473b437c6f5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529705"
---
# <a name="update-icon"></a><span data-ttu-id="084e7-103">Update-Symbol</span><span class="sxs-lookup"><span data-stu-id="084e7-103">Update icon</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="084e7-104">Dient zum Aktualisieren der Eigenschaften des Symbolobjekts.</span><span class="sxs-lookup"><span data-stu-id="084e7-104">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="084e7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="084e7-105">Permissions</span></span>
<span data-ttu-id="084e7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="084e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="084e7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="084e7-108">Permission type</span></span>      | <span data-ttu-id="084e7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="084e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="084e7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="084e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="084e7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="084e7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="084e7-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="084e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="084e7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="084e7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="084e7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="084e7-114">Application</span></span> | <span data-ttu-id="084e7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="084e7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="084e7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="084e7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="084e7-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="084e7-117">Optional request headers</span></span>
| <span data-ttu-id="084e7-118">Name</span><span class="sxs-lookup"><span data-stu-id="084e7-118">Name</span></span>       | <span data-ttu-id="084e7-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="084e7-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="084e7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="084e7-120">Authorization</span></span>  | <span data-ttu-id="084e7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="084e7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="084e7-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="084e7-123">Request body</span></span>
<span data-ttu-id="084e7-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="084e7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="084e7-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="084e7-127">Property</span></span>     | <span data-ttu-id="084e7-128">Typ</span><span class="sxs-lookup"><span data-stu-id="084e7-128">Type</span></span>   |<span data-ttu-id="084e7-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="084e7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="084e7-130">Index</span><span class="sxs-lookup"><span data-stu-id="084e7-130">index</span></span>|<span data-ttu-id="084e7-131">int</span><span class="sxs-lookup"><span data-stu-id="084e7-131">int</span></span>|<span data-ttu-id="084e7-132">Stellt den Index des Symbols im angegebenen Satz dar.</span><span class="sxs-lookup"><span data-stu-id="084e7-132">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="084e7-133">set</span><span class="sxs-lookup"><span data-stu-id="084e7-133">set</span></span>|<span data-ttu-id="084e7-134">string</span><span class="sxs-lookup"><span data-stu-id="084e7-134">string</span></span>|<span data-ttu-id="084e7-p104">Stellt den Satz dar, zu dem das Symbol gehört. Mögliche Werte: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="084e7-p104">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="084e7-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="084e7-137">Response</span></span>

<span data-ttu-id="084e7-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [Icon](../resources/icon.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="084e7-138">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="084e7-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="084e7-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="084e7-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="084e7-140">Request</span></span>
<span data-ttu-id="084e7-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="084e7-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_icon"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```
##### <a name="response"></a><span data-ttu-id="084e7-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="084e7-142">Response</span></span>
<span data-ttu-id="084e7-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="084e7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/icon-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
