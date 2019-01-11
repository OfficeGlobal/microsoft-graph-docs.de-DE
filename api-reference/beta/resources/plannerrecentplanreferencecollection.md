---
title: Ressourcentyp plannerRecentPlanReferenceCollection
description: Die Ressource **PlannerRecentPlanReferenceCollection** stellt die Auflistung von Verweisen auf Pläne, die von einem Benutzer zuletzt angezeigt wurden. Diese Ressource ist ein offener Typ und ist Teil des PlannerUser-Objekts. Der Name der Eigenschaft ist die ID des entsprechenden Plans. Der Wert in der Eigenschaft-Wert-Paar ist das PlannerRecentPlanReference-Objekt.
localization_priority: Normal
ms.openlocfilehash: e77769cbe3a7e53dce518c73cd7c5228d1077dac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877343"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="b918c-106">Ressourcentyp plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="b918c-106">plannerRecentPlanReferenceCollection resource type</span></span>

> <span data-ttu-id="b918c-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b918c-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b918c-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b918c-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b918c-109">Die Ressource **PlannerRecentPlanReferenceCollection** stellt die Auflistung von Verweisen auf Pläne, die von einem Benutzer zuletzt angezeigt wurden.</span><span class="sxs-lookup"><span data-stu-id="b918c-109">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="b918c-110">Diese Ressource ist ein offener Typ und ist Teil des [PlannerUser](planneruser.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b918c-110">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="b918c-111">Der Name der Eigenschaft ist die ID des entsprechenden Plans.</span><span class="sxs-lookup"><span data-stu-id="b918c-111">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="b918c-112">Der Wert in der Eigenschaft-Wert-Paar ist das [PlannerRecentPlanReference](plannerrecentplanreference.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="b918c-112">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="b918c-113">Hinzufügen von neuen verweisen auf diese Auflistung wird automatisch die ältesten Einträge entfernt, wenn die Größe der Auflistung einen festgelegten Höchstwert überschreitet.</span><span class="sxs-lookup"><span data-stu-id="b918c-113">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="b918c-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b918c-114">Properties</span></span>
<span data-ttu-id="b918c-115">Sie können die Eigenschaften dieses Typs open definieren.</span><span class="sxs-lookup"><span data-stu-id="b918c-115">You can define the properties of this open type.</span></span> <span data-ttu-id="b918c-116">Werden die Eigenschaftennamen `id` Werte der [PlannerPlan](plannerplan.md) Ressourcen und deren Werte muss [PlannerRecentPlanReference](plannerrecentplanreference.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="b918c-116">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="b918c-117">Wenn ein Element in der Liste der Favoriten entfernen möchten, legen Sie den Wert der Eigenschaft `null`.</span><span class="sxs-lookup"><span data-stu-id="b918c-117">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b918c-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b918c-118">JSON representation</span></span>

<span data-ttu-id="b918c-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b918c-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
