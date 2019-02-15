---
title: Ressourcentyp „locationConstraintItem“
description: Die vom Client definierten Bedingungen für den Ort einer Besprechung.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8e0b14096d8be66a6aab6d4e73cf0941d7db7b5c
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057001"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="2cc16-103">Ressourcentyp „locationConstraintItem“</span><span class="sxs-lookup"><span data-stu-id="2cc16-103">locationConstraintItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cc16-104">Die vom Client definierten Bedingungen für den Ort einer Besprechung.</span><span class="sxs-lookup"><span data-stu-id="2cc16-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="2cc16-105">Abgeleitet von [locationDataModel](locationdatamodel.md).</span><span class="sxs-lookup"><span data-stu-id="2cc16-105">Derived from [locationDataModel](locationdatamodel.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cc16-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2cc16-106">JSON representation</span></span>

<span data-ttu-id="2cc16-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2cc16-107">Here is a JSON representation of the resource</span></span>

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
  "locationUri": "string"
}

```
## <a name="properties"></a><span data-ttu-id="2cc16-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2cc16-108">Properties</span></span>
| <span data-ttu-id="2cc16-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2cc16-109">Property</span></span>     | <span data-ttu-id="2cc16-110">Typ</span><span class="sxs-lookup"><span data-stu-id="2cc16-110">Type</span></span>   |<span data-ttu-id="2cc16-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2cc16-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2cc16-112">address</span><span class="sxs-lookup"><span data-stu-id="2cc16-112">address</span></span> | [<span data-ttu-id="2cc16-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2cc16-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="2cc16-114">Die Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="2cc16-114">The street address of the location.</span></span> |
| <span data-ttu-id="2cc16-115">Koordinaten</span><span class="sxs-lookup"><span data-stu-id="2cc16-115">coordinates</span></span> | [<span data-ttu-id="2cc16-116">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="2cc16-116">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="2cc16-117">Die geografischen Koordinaten und die Erhebung des Orts.</span><span class="sxs-lookup"><span data-stu-id="2cc16-117">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="2cc16-118">displayName</span><span class="sxs-lookup"><span data-stu-id="2cc16-118">displayName</span></span>  | <span data-ttu-id="2cc16-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2cc16-119">String</span></span> | <span data-ttu-id="2cc16-120">Der Name, der mit dem Ort verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="2cc16-120">The name associated with the location.</span></span>                       |
| <span data-ttu-id="2cc16-121">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="2cc16-121">locationEmailAddress</span></span> | <span data-ttu-id="2cc16-122">String</span><span class="sxs-lookup"><span data-stu-id="2cc16-122">String</span></span> | <span data-ttu-id="2cc16-123">Optionale E-Mail-Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="2cc16-123">Optional email address of the location.</span></span> |
| <span data-ttu-id="2cc16-124">locationUri</span><span class="sxs-lookup"><span data-stu-id="2cc16-124">locationUri</span></span> | <span data-ttu-id="2cc16-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2cc16-125">String</span></span> | <span data-ttu-id="2cc16-126">Optionaler URI, der den Ort darstellt.</span><span class="sxs-lookup"><span data-stu-id="2cc16-126">Optional URI representing the location.</span></span> |
| <span data-ttu-id="2cc16-127">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="2cc16-127">resolveAvailability</span></span> | <span data-ttu-id="2cc16-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2cc16-128">Boolean</span></span> | <span data-ttu-id="2cc16-p101">Wenn „true“ gesetzt ist und die angegebene Ressource gebucht ist, sucht [findMeetingTimes](../api/user-findmeetingtimes.md) nach einer anderen, freien Ressource. Wenn „false“ gesetzt ist und die angegebene Ressource gebucht ist, gibt **findMeetingTimes** die Ressource mit dem höchsten Wert aus dem Cache des Benutzers zurück, ohne zu prüfen, ob diese Ressource frei ist. Der Standardwert ist „true“.</span><span class="sxs-lookup"><span data-stu-id="2cc16-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

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
