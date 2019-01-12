---
title: Ressourcentyp plannerPlanContextCollection
description: Die Ressource **PlannerPlanContextCollection** stellt die Auflistung von externen Kontexten mit denen ein Plans verknüpft ist. Diese Ressource ist ein offener Typ und ist Teil des PlannerPlan-Objekts. Der Wert in der Eigenschaft-Wert-Paar ist das PlannerPlanContext-Objekt.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 3281a7664561ac32c3908ca059209a1b89b4ea7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951810"
---
# <a name="plannerplancontextcollection-resource-type"></a><span data-ttu-id="591dd-105">Ressourcentyp plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="591dd-105">plannerPlanContextCollection resource type</span></span>

> <span data-ttu-id="591dd-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="591dd-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="591dd-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="591dd-107">Use of these APIs in production applications is not supported.</span></span>


<span data-ttu-id="591dd-108">Die Ressource **PlannerPlanContextCollection** stellt die Auflistung von externen Kontexten mit denen ein Plans verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="591dd-108">The **plannerPlanContextCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="591dd-109">Diese Ressource ist ein offener Typ und ist Teil des [PlannerPlan](plannerplan.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="591dd-109">This resource is an open type and is part of the [plannerPlan](plannerplan.md) object.</span></span> <span data-ttu-id="591dd-110">Der Wert in der Eigenschaft-Wert-Paar ist das [PlannerPlanContext](plannerplancontext.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="591dd-110">The value in the property-value pair is the [plannerPlanContext](plannerplancontext.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="591dd-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="591dd-111">Properties</span></span>
<span data-ttu-id="591dd-112">Sie können die Eigenschaften dieses Typs open definieren.</span><span class="sxs-lookup"><span data-stu-id="591dd-112">You can define the properties of this open type.</span></span> <span data-ttu-id="591dd-113">Die Eigenschaftswerte sollte charakteristischen Bezeichner, der den externen Kontext wie der Name der Eigenschaft darstellt.</span><span class="sxs-lookup"><span data-stu-id="591dd-113">The property values should be distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="591dd-114">Die Eigenschaftswerte muss [PlannerPlanContext](plannerplancontext.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="591dd-114">The property values must be [plannerPlanContext](plannerplancontext.md) objects.</span></span> <span data-ttu-id="591dd-115">Basierend auf OData-Anforderungen, Eigenschaftennamen im offenen Typen die folgenden Zeichen nicht enthalten: `.`, `:`, `%`, `@`.</span><span class="sxs-lookup"><span data-stu-id="591dd-115">Based on OData requirements, property names in open types cannot contain the following characters: `.`, `:`, `%`, `@`.</span></span> <span data-ttu-id="591dd-116">Diese Zeichen mit URL-Codierung codiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="591dd-116">These characters need to be encoded using URL encoding.</span></span> <span data-ttu-id="591dd-117">Wenn ein Element in der Liste der Favoriten entfernen möchten, legen Sie den Wert der Eigenschaft `null`.</span><span class="sxs-lookup"><span data-stu-id="591dd-117">To remove an item in the favorites list, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="591dd-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="591dd-118">JSON representation</span></span>

<span data-ttu-id="591dd-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="591dd-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextCollection"
}-->

```json
{
  "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
    "@odata.type": "#microsoft.graph.plannerPlanContext",
    "associationType": "Board",
    "createdDateTime": "2015-10-14T00:57:28.4698344Z",
    "displayNameSegments": [
        "Finance Team",
        "Budget Plans"
    ],
    "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
