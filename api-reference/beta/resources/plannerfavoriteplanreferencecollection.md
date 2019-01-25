---
title: Ressourcentyp plannerFavoritePlanReferenceCollection
description: " der Wert ist das PlannerFavoritePlanReference-Objekt."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: c473d4101a1247420e641b532ea04dfbc1a26d2c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519486"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="f9b2c-103">Ressourcentyp plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="f9b2c-103">plannerFavoritePlanReferenceCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9b2c-104">Die Ressource **PlannerFavoritePlanReferenceCollection** stellt die Auflistung von Verweisen auf Pläne, die von einem Benutzer als Favoriten markiert sind.</span><span class="sxs-lookup"><span data-stu-id="f9b2c-104">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="f9b2c-105">Diese Ressource ist ein offener Typ und ist Teil des [PlannerUser](planneruser.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f9b2c-105">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="f9b2c-106">Der Name der Eigenschaft in der Eigenschaft-Wert-Paar ist die ID des entsprechenden Plans. der Wert ist das [PlannerFavoritePlanReference](plannerfavoriteplanreference.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="f9b2c-106">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="f9b2c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f9b2c-107">Properties</span></span>
<span data-ttu-id="f9b2c-108">Sie können die Eigenschaften dieses Typs open definieren.</span><span class="sxs-lookup"><span data-stu-id="f9b2c-108">You can define the properties of this open type.</span></span> <span data-ttu-id="f9b2c-109">Werden die Eigenschaftennamen `id` Werte der [PlannerPlan](plannerplan.md) Ressourcen und deren Werte muss [PlannerFavoritePlanReference](plannerfavoriteplanreference.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="f9b2c-109">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="f9b2c-110">Wenn ein Element in der Liste der Favoriten entfernen möchten, legen Sie den Wert der Eigenschaft `null`.</span><span class="sxs-lookup"><span data-stu-id="f9b2c-110">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f9b2c-111">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f9b2c-111">JSON representation</span></span>

<span data-ttu-id="f9b2c-112">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f9b2c-112">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerfavoriteplanreferencecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
