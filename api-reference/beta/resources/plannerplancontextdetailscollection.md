---
title: Ressourcentyp plannerPlanContextDetailsCollection
description: " der Wert ist das PlannerPlanContextDetails-Objekt."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: ca1625a4bf137fc14cc780df4d4d1e5ec3bb226e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508748"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="78374-103">Ressourcentyp plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="78374-103">plannerPlanContextDetailsCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="78374-104">Die Ressource **PlannerPlanContextDetailsCollection** stellt die Auflistung von externen Kontexten mit denen ein Plans verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="78374-104">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="78374-105">Diese Ressource ist ein offener Typ und ist Teil des [PlannerPlanDetails](plannerplandetails.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="78374-105">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="78374-106">Der Name der Eigenschaft in der Eigenschaft-Wert-Paar ist ein app-spezifischen Bezeichner des Kontexts. der Wert ist das [PlannerPlanContextDetails](plannerplancontextdetails.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="78374-106">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="78374-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="78374-107">Properties</span></span>
<span data-ttu-id="78374-108">Eigenschaften vom Typ open können vom Client definiert werden.</span><span class="sxs-lookup"><span data-stu-id="78374-108">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="78374-109">In diesem Fall sollte der Client einen charakteristischen Bezeichner verwenden, der den externen Kontext wie der Name der Eigenschaft darstellt.</span><span class="sxs-lookup"><span data-stu-id="78374-109">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="78374-110">Die Eigenschaftswerte muss [PlannerPlanContextDetails](plannerplancontextdetails.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="78374-110">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="78374-111">Basierend auf OData, Eigenschaftennamen im offenen Typen die folgenden Zeichen nicht enthalten: `.`, `:`, `@`, `%`.</span><span class="sxs-lookup"><span data-stu-id="78374-111">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="78374-112">Diese Zeichen mit URL-Codierung Format codiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="78374-112">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="78374-113">Um ein Element in der Liste der Favoriten zu entfernen, muss der Wert aus der Auflistung [PlannerPlanContextCollection](plannerplancontextcollection.md) stattdessen entfernt werden die wird automatisch den Eintrag in diesem Objekt zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="78374-113">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextdetailscollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
