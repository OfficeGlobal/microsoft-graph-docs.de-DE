---
title: Ressourcentyp „locationConstraintItem“
description: Die vom Client definierten Bedingungen für den Ort einer Besprechung.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7063eb0a7aa437b51a2bfecb482012771297f766
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936255"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="6ff1d-103">Ressourcentyp „locationConstraintItem“</span><span class="sxs-lookup"><span data-stu-id="6ff1d-103">locationConstraintItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ff1d-104">Die vom Client definierten Bedingungen für den Ort einer Besprechung.</span><span class="sxs-lookup"><span data-stu-id="6ff1d-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="6ff1d-105">Abgeleitet von [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="6ff1d-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ff1d-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ff1d-106">JSON representation</span></span>

<span data-ttu-id="6ff1d-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ff1d-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  
  ],
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationType": "string",
  "locationUri": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="6ff1d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ff1d-108">Properties</span></span>
| <span data-ttu-id="6ff1d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ff1d-109">Property</span></span>     | <span data-ttu-id="6ff1d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6ff1d-110">Type</span></span>   |<span data-ttu-id="6ff1d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ff1d-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6ff1d-112">address</span><span class="sxs-lookup"><span data-stu-id="6ff1d-112">address</span></span> | [<span data-ttu-id="6ff1d-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="6ff1d-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="6ff1d-114">Die Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="6ff1d-114">The street address of the location.</span></span> |
| <span data-ttu-id="6ff1d-115">Koordinaten</span><span class="sxs-lookup"><span data-stu-id="6ff1d-115">coordinates</span></span> | [<span data-ttu-id="6ff1d-116">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="6ff1d-116">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="6ff1d-117">Die geografischen Koordinaten und die Erhebung des Orts.</span><span class="sxs-lookup"><span data-stu-id="6ff1d-117">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="6ff1d-118">displayName</span><span class="sxs-lookup"><span data-stu-id="6ff1d-118">displayName</span></span>  | <span data-ttu-id="6ff1d-119">String</span><span class="sxs-lookup"><span data-stu-id="6ff1d-119">String</span></span> | <span data-ttu-id="6ff1d-120">Der Name, der mit dem Ort verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="6ff1d-120">The name associated with the location.</span></span>                       |
| <span data-ttu-id="6ff1d-121">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="6ff1d-121">locationEmailAddress</span></span> | <span data-ttu-id="6ff1d-122">String</span><span class="sxs-lookup"><span data-stu-id="6ff1d-122">String</span></span> | <span data-ttu-id="6ff1d-123">Optionale E-Mail-Adresse des Orts</span><span class="sxs-lookup"><span data-stu-id="6ff1d-123">Optional email address of the location.</span></span> |
| <span data-ttu-id="6ff1d-124">locationType</span><span class="sxs-lookup"><span data-stu-id="6ff1d-124">locationType</span></span> | <span data-ttu-id="6ff1d-125">locationType</span><span class="sxs-lookup"><span data-stu-id="6ff1d-125">locationType</span></span> | <span data-ttu-id="6ff1d-126">Der Typ des Orts.</span><span class="sxs-lookup"><span data-stu-id="6ff1d-126">The type of location.</span></span> <span data-ttu-id="6ff1d-127">Mögliche Werte sind: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="6ff1d-127">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="6ff1d-128">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6ff1d-128">Read-only.</span></span>|
| <span data-ttu-id="6ff1d-129">locationUri</span><span class="sxs-lookup"><span data-stu-id="6ff1d-129">locationUri</span></span> | <span data-ttu-id="6ff1d-130">String</span><span class="sxs-lookup"><span data-stu-id="6ff1d-130">String</span></span> | <span data-ttu-id="6ff1d-131">Optionaler URI, der den Ort darstellt.</span><span class="sxs-lookup"><span data-stu-id="6ff1d-131">Optional URI representing the location.</span></span> |
| <span data-ttu-id="6ff1d-132">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="6ff1d-132">resolveAvailability</span></span> | <span data-ttu-id="6ff1d-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ff1d-133">Boolean</span></span> | <span data-ttu-id="6ff1d-p102">Wenn „true“ gesetzt ist und die angegebene Ressource gebucht ist, sucht [findMeetingTimes](../api/user-findmeetingtimes.md) nach einer anderen, freien Ressource. Wenn „false“ gesetzt ist und die angegebene Ressource gebucht ist, gibt **findMeetingTimes** die Ressource mit dem höchsten Wert aus dem Cache des Benutzers zurück, ohne zu prüfen, ob diese Ressource frei ist. Der Standardwert ist „true“.</span><span class="sxs-lookup"><span data-stu-id="6ff1d-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |
| <span data-ttu-id="6ff1d-137">uniqueId</span><span class="sxs-lookup"><span data-stu-id="6ff1d-137">uniqueId</span></span> | <span data-ttu-id="6ff1d-138">String</span><span class="sxs-lookup"><span data-stu-id="6ff1d-138">String</span></span> | <span data-ttu-id="6ff1d-139">Nur für internen Gebrauch.</span><span class="sxs-lookup"><span data-stu-id="6ff1d-139">For internal use only.</span></span>|
| <span data-ttu-id="6ff1d-140">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="6ff1d-140">uniqueIdType</span></span> | <span data-ttu-id="6ff1d-141">String</span><span class="sxs-lookup"><span data-stu-id="6ff1d-141">String</span></span> | <span data-ttu-id="6ff1d-142">Ausschließlich für interne Zwecke.</span><span class="sxs-lookup"><span data-stu-id="6ff1d-142">For internal use only.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationconstraintitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
