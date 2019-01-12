---
title: Ressourcentyp plannerPlanContextDetailsCollection
description: " der Wert ist das PlannerPlanContextDetails-Objekt."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 017734f3d5f5fb1a0ed56f390a7c945e43b707a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981476"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="e1ed7-103">Ressourcentyp plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="e1ed7-103">plannerPlanContextDetailsCollection resource type</span></span>

> <span data-ttu-id="e1ed7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e1ed7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1ed7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e1ed7-105">Use of these APIs in production applications is not supported.</span></span>


<span data-ttu-id="e1ed7-106">Die Ressource **PlannerPlanContextDetailsCollection** stellt die Auflistung von externen Kontexten mit denen ein Plans verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="e1ed7-106">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="e1ed7-107">Diese Ressource ist ein offener Typ und ist Teil des [PlannerPlanDetails](plannerplandetails.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e1ed7-107">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="e1ed7-108">Der Name der Eigenschaft in der Eigenschaft-Wert-Paar ist ein app-spezifischen Bezeichner des Kontexts. der Wert ist das [PlannerPlanContextDetails](plannerplancontextdetails.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="e1ed7-108">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="e1ed7-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e1ed7-109">Properties</span></span>
<span data-ttu-id="e1ed7-110">Eigenschaften vom Typ open können vom Client definiert werden.</span><span class="sxs-lookup"><span data-stu-id="e1ed7-110">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="e1ed7-111">In diesem Fall sollte der Client einen charakteristischen Bezeichner verwenden, der den externen Kontext wie der Name der Eigenschaft darstellt.</span><span class="sxs-lookup"><span data-stu-id="e1ed7-111">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="e1ed7-112">Die Eigenschaftswerte muss [PlannerPlanContextDetails](plannerplancontextdetails.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="e1ed7-112">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="e1ed7-113">Basierend auf OData, Eigenschaftennamen im offenen Typen die folgenden Zeichen nicht enthalten: `.`, `:`, `@`, `%`.</span><span class="sxs-lookup"><span data-stu-id="e1ed7-113">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="e1ed7-114">Diese Zeichen mit URL-Codierung Format codiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="e1ed7-114">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="e1ed7-115">Um ein Element in der Liste der Favoriten zu entfernen, muss der Wert aus der Auflistung [PlannerPlanContextCollection](plannerplancontextcollection.md) stattdessen entfernt werden die wird automatisch den Eintrag in diesem Objekt zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="e1ed7-115">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
