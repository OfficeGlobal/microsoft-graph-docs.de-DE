---
title: Ressourcentyp plannerFavoritePlanReferenceCollection
description: " der Wert ist das PlannerFavoritePlanReference-Objekt."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 333d7f354f056945de52687eefc8bb862ac48e75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967112"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="9b804-103">Ressourcentyp plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="9b804-103">plannerFavoritePlanReferenceCollection resource type</span></span>

> <span data-ttu-id="9b804-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9b804-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b804-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9b804-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b804-106">Die Ressource **PlannerFavoritePlanReferenceCollection** stellt die Auflistung von Verweisen auf Pläne, die von einem Benutzer als Favoriten markiert sind.</span><span class="sxs-lookup"><span data-stu-id="9b804-106">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="9b804-107">Diese Ressource ist ein offener Typ und ist Teil des [PlannerUser](planneruser.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9b804-107">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="9b804-108">Der Name der Eigenschaft in der Eigenschaft-Wert-Paar ist die ID des entsprechenden Plans. der Wert ist das [PlannerFavoritePlanReference](plannerfavoriteplanreference.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="9b804-108">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="9b804-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9b804-109">Properties</span></span>
<span data-ttu-id="9b804-110">Sie können die Eigenschaften dieses Typs open definieren.</span><span class="sxs-lookup"><span data-stu-id="9b804-110">You can define the properties of this open type.</span></span> <span data-ttu-id="9b804-111">Werden die Eigenschaftennamen `id` Werte der [PlannerPlan](plannerplan.md) Ressourcen und deren Werte muss [PlannerFavoritePlanReference](plannerfavoriteplanreference.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="9b804-111">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="9b804-112">Wenn ein Element in der Liste der Favoriten entfernen möchten, legen Sie den Wert der Eigenschaft `null`.</span><span class="sxs-lookup"><span data-stu-id="9b804-112">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9b804-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9b804-113">JSON representation</span></span>

<span data-ttu-id="9b804-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9b804-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
}-->

```json
{
  "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586866870001551087",
    "planTitle": "Customer reviews"
  },
  "uZWtCtli30CGoWLIWSat1mQAC0ai": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586848705198093378",
    "planTitle": "Order Management (December 2017)"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
