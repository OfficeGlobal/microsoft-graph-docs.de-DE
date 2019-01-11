---
title: Ressourcentyp „locationConstraintItem“
description: Die vom Client definierten Bedingungen für den Ort einer Besprechung.
localization_priority: Normal
ms.openlocfilehash: d9124377172c7598d45b0be9b9f3f9799bd3e1f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874319"
---
# <a name="locationconstraintitem-resource-type"></a><span data-ttu-id="3c741-103">Ressourcentyp „locationConstraintItem“</span><span class="sxs-lookup"><span data-stu-id="3c741-103">locationConstraintItem resource type</span></span>

<span data-ttu-id="3c741-104">Die vom Client definierten Bedingungen für den Ort einer Besprechung.</span><span class="sxs-lookup"><span data-stu-id="3c741-104">The conditions stated by a client for the location of a meeting.</span></span>

<span data-ttu-id="3c741-105">Abgeleitet von [location](location.md).</span><span class="sxs-lookup"><span data-stu-id="3c741-105">Derived from [location](location.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c741-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3c741-106">JSON representation</span></span>

<span data-ttu-id="3c741-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3c741-107">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.location",
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```
## <a name="properties"></a><span data-ttu-id="3c741-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3c741-108">Properties</span></span>
| <span data-ttu-id="3c741-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c741-109">Property</span></span>     | <span data-ttu-id="3c741-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3c741-110">Type</span></span>   |<span data-ttu-id="3c741-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c741-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3c741-112">address</span><span class="sxs-lookup"><span data-stu-id="3c741-112">address</span></span> | [<span data-ttu-id="3c741-113">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="3c741-113">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="3c741-114">Die Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="3c741-114">The street address of the location.</span></span> |
| <span data-ttu-id="3c741-115">displayName</span><span class="sxs-lookup"><span data-stu-id="3c741-115">displayName</span></span>  | <span data-ttu-id="3c741-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3c741-116">String</span></span> | <span data-ttu-id="3c741-117">Der Name, der mit dem Ort verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="3c741-117">The name associated with the location.</span></span>                       |
| <span data-ttu-id="3c741-118">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="3c741-118">locationEmailAddress</span></span> | <span data-ttu-id="3c741-119">String</span><span class="sxs-lookup"><span data-stu-id="3c741-119">String</span></span> | <span data-ttu-id="3c741-120">Optionale E-Mail-Adresse des Orts</span><span class="sxs-lookup"><span data-stu-id="3c741-120">Optional email address of the location.</span></span> |
| <span data-ttu-id="3c741-121">resolveAvailability</span><span class="sxs-lookup"><span data-stu-id="3c741-121">resolveAvailability</span></span> | <span data-ttu-id="3c741-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3c741-122">Boolean</span></span> | <span data-ttu-id="3c741-p101">Wenn „true“ gesetzt ist und die angegebene Ressource gebucht ist, sucht [findMeetingTimes](../api/user-findmeetingtimes.md) nach einer anderen, freien Ressource. Wenn „false“ gesetzt ist und die angegebene Ressource gebucht ist, gibt **findMeetingTimes** die Ressource mit dem höchsten Wert aus dem Cache des Benutzers zurück, ohne zu prüfen, ob diese Ressource frei ist. Der Standardwert ist „true“.</span><span class="sxs-lookup"><span data-stu-id="3c741-p101">If set to true and the specified resource is busy, [findMeetingTimes](../api/user-findmeetingtimes.md) looks for another resource that is free. If set to false and the specified resource is busy, **findMeetingTimes** returns the resource best ranked in the user's cache without checking if it's free. Default is true.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
