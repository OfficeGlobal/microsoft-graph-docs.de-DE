---
title: Update-Symbol
description: Dient zum Aktualisieren der Eigenschaften des Symbolobjekts.
ms.openlocfilehash: 5b9d049eb4d7bf3c596392c289738538799f8386
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064783"
---
# <a name="update-icon"></a><span data-ttu-id="410a0-103">Update-Symbol</span><span class="sxs-lookup"><span data-stu-id="410a0-103">Update icon</span></span>

> <span data-ttu-id="410a0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="410a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="410a0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="410a0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="410a0-106">Dient zum Aktualisieren der Eigenschaften des Symbolobjekts.</span><span class="sxs-lookup"><span data-stu-id="410a0-106">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="410a0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="410a0-107">Permissions</span></span>
<span data-ttu-id="410a0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="410a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="410a0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="410a0-110">Permission type</span></span>      | <span data-ttu-id="410a0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="410a0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="410a0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="410a0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="410a0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="410a0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="410a0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="410a0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="410a0-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="410a0-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="410a0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="410a0-116">Application</span></span> | <span data-ttu-id="410a0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="410a0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="410a0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="410a0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="410a0-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="410a0-119">Optional request headers</span></span>
| <span data-ttu-id="410a0-120">Name</span><span class="sxs-lookup"><span data-stu-id="410a0-120">Name</span></span>       | <span data-ttu-id="410a0-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="410a0-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="410a0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="410a0-122">Authorization</span></span>  | <span data-ttu-id="410a0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="410a0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="410a0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="410a0-125">Request body</span></span>
<span data-ttu-id="410a0-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="410a0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="410a0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="410a0-129">Property</span></span>     | <span data-ttu-id="410a0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="410a0-130">Type</span></span>   |<span data-ttu-id="410a0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="410a0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="410a0-132">Index</span><span class="sxs-lookup"><span data-stu-id="410a0-132">index</span></span>|<span data-ttu-id="410a0-133">int</span><span class="sxs-lookup"><span data-stu-id="410a0-133">int</span></span>|<span data-ttu-id="410a0-134">Stellt den Index des Symbols im angegebenen Satz dar.</span><span class="sxs-lookup"><span data-stu-id="410a0-134">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="410a0-135">set</span><span class="sxs-lookup"><span data-stu-id="410a0-135">set</span></span>|<span data-ttu-id="410a0-136">string</span><span class="sxs-lookup"><span data-stu-id="410a0-136">string</span></span>|<span data-ttu-id="410a0-p105">Stellt den Satz dar, zu dem das Symbol gehört. Mögliche Werte: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="410a0-p105">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="410a0-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="410a0-139">Response</span></span>

<span data-ttu-id="410a0-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [Icon](../resources/icon.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="410a0-140">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="410a0-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="410a0-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="410a0-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="410a0-142">Request</span></span>
<span data-ttu-id="410a0-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="410a0-143">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="410a0-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="410a0-144">Response</span></span>
<span data-ttu-id="410a0-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="410a0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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