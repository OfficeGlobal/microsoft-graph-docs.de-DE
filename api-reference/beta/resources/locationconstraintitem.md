---
title: Ressourcentyp „locationConstraintItem“
description: Die vom Client definierten Bedingungen für den Ort einer Besprechung.
ms.openlocfilehash: f29ff1283d876e726e27473485a183956137f981
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058454"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="48c7a-103">Ressourcentyp „locationConstraintItem“</span><span class="sxs-lookup"><span data-stu-id="48c7a-103">locationConstraintItem resource type</span></span>

> <span data-ttu-id="48c7a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="48c7a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48c7a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="48c7a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48c7a-106">Die vom Client definierten Bedingungen für den Ort einer Besprechung</span><span class="sxs-lookup"><span data-stu-id="48c7a-106">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="48c7a-107">Abgeleitet von [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="48c7a-107">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="48c7a-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="48c7a-108">JSON representation</span></span>

<span data-ttu-id="48c7a-109">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="48c7a-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="48c7a-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="48c7a-110">Properties</span></span>
| <span data-ttu-id="48c7a-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="48c7a-111">Property</span></span>     | <span data-ttu-id="48c7a-112">Typ</span><span class="sxs-lookup"><span data-stu-id="48c7a-112">Type</span></span>   |<span data-ttu-id="48c7a-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48c7a-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="48c7a-114">address</span><span class="sxs-lookup"><span data-stu-id="48c7a-114">address</span></span> | [<span data-ttu-id="48c7a-115">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="48c7a-115">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="48c7a-116">Die Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="48c7a-116">The street address of the location.</span></span> |
| <span data-ttu-id="48c7a-117">Koordinaten</span><span class="sxs-lookup"><span data-stu-id="48c7a-117">coordinates</span></span> | [<span data-ttu-id="48c7a-118">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="48c7a-118">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="48c7a-119">Die geografischen Koordinaten und die Erhebung des Orts.</span><span class="sxs-lookup"><span data-stu-id="48c7a-119">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="48c7a-120">displayName</span><span class="sxs-lookup"><span data-stu-id="48c7a-120">displayName</span></span>  | <span data-ttu-id="48c7a-121">String</span><span class="sxs-lookup"><span data-stu-id="48c7a-121">String</span></span> | <span data-ttu-id="48c7a-122">Der Name, der mit dem Ort verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="48c7a-122">The name associated with the location.</span></span>                       |
| <span data-ttu-id="48c7a-123">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="48c7a-123">locationEmailAddress</span></span> | <span data-ttu-id="48c7a-124">String</span><span class="sxs-lookup"><span data-stu-id="48c7a-124">String</span></span> | <span data-ttu-id="48c7a-125">Optionale E-Mail-Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="48c7a-125">Optional email address of the location.</span></span> |
| <span data-ttu-id="48c7a-126">locationUri</span><span class="sxs-lookup"><span data-stu-id="48c7a-126">locationUri</span></span> | <span data-ttu-id="48c7a-127">String</span><span class="sxs-lookup"><span data-stu-id="48c7a-127">String</span></span> | <span data-ttu-id="48c7a-128">Optionaler URI, der den Ort darstellt.</span><span class="sxs-lookup"><span data-stu-id="48c7a-128">Optional URI representing the location.</span></span> |
| <span data-ttu-id="48c7a-129">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="48c7a-129">resolveAvailability</span></span> | <span data-ttu-id="48c7a-130">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="48c7a-130">Boolean</span></span> | <span data-ttu-id="48c7a-p102">Wenn „true“ gesetzt ist und die angegebene Ressource gebucht ist, sucht [findMeetingTimes](../api/user-findmeetingtimes.md) nach einer anderen, freien Ressource. Wenn „false“ gesetzt ist und die angegebene Ressource gebucht ist, gibt **findMeetingTimes** die Ressource mit dem höchsten Wert aus dem Cache des Benutzers zurück, ohne zu prüfen, ob diese Ressource frei ist. Der Standardwert ist „true“.</span><span class="sxs-lookup"><span data-stu-id="48c7a-p102">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->