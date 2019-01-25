---
title: Ressourcentyp plannerRecentPlanReferenceCollection
description: Die Ressource **PlannerRecentPlanReferenceCollection** stellt die Auflistung von Verweisen auf Pläne, die von einem Benutzer zuletzt angezeigt wurden. Diese Ressource ist ein offener Typ und ist Teil des PlannerUser-Objekts. Der Name der Eigenschaft ist die ID des entsprechenden Plans. Der Wert in der Eigenschaft-Wert-Paar ist das PlannerRecentPlanReference-Objekt.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e27375e3f2395b3528873d8b83f0b5aa6f48d52e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514992"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="54596-106">Ressourcentyp plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="54596-106">plannerRecentPlanReferenceCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54596-107">Die Ressource **PlannerRecentPlanReferenceCollection** stellt die Auflistung von Verweisen auf Pläne, die von einem Benutzer zuletzt angezeigt wurden.</span><span class="sxs-lookup"><span data-stu-id="54596-107">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="54596-108">Diese Ressource ist ein offener Typ und ist Teil des [PlannerUser](planneruser.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="54596-108">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="54596-109">Der Name der Eigenschaft ist die ID des entsprechenden Plans.</span><span class="sxs-lookup"><span data-stu-id="54596-109">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="54596-110">Der Wert in der Eigenschaft-Wert-Paar ist das [PlannerRecentPlanReference](plannerrecentplanreference.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="54596-110">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="54596-111">Hinzufügen von neuen verweisen auf diese Auflistung wird automatisch die ältesten Einträge entfernt, wenn die Größe der Auflistung einen festgelegten Höchstwert überschreitet.</span><span class="sxs-lookup"><span data-stu-id="54596-111">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="54596-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="54596-112">Properties</span></span>
<span data-ttu-id="54596-113">Sie können die Eigenschaften dieses Typs open definieren.</span><span class="sxs-lookup"><span data-stu-id="54596-113">You can define the properties of this open type.</span></span> <span data-ttu-id="54596-114">Werden die Eigenschaftennamen `id` Werte der [PlannerPlan](plannerplan.md) Ressourcen und deren Werte muss [PlannerRecentPlanReference](plannerrecentplanreference.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="54596-114">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="54596-115">Wenn ein Element in der Liste der Favoriten entfernen möchten, legen Sie den Wert der Eigenschaft `null`.</span><span class="sxs-lookup"><span data-stu-id="54596-115">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="54596-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="54596-116">JSON representation</span></span>

<span data-ttu-id="54596-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="54596-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
}-->

```json
{
  "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-02T22:49:46.155Z",
    "planTitle": "Purchase Workflow"
  },
  "iKNMHkk3vEWpSF7F7iZWIGQAAMMw": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-03T21:59:28.975Z",
    "planTitle": "New Year's Office Party"
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreferencecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
