---
title: Ressourcentyp plannerPlanContextDetailsCollection
description: " der Wert ist das PlannerPlanContextDetails-Objekt."
author: TarkanSevilmis
ms.openlocfilehash: 725239a83f1c059aeef39f68b0d4d58ce8c91013
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346767"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="4f605-103">Ressourcentyp plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="4f605-103">plannerPlanContextDetailsCollection resource type</span></span>

> <span data-ttu-id="4f605-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4f605-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f605-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4f605-105">Use of these APIs in production applications is not supported.</span></span>


<span data-ttu-id="4f605-106">Die Ressource **PlannerPlanContextDetailsCollection** stellt die Auflistung von externen Kontexten mit denen ein Plans verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="4f605-106">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="4f605-107">Diese Ressource ist ein offener Typ und ist Teil des [PlannerPlanDetails](plannerplandetails.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4f605-107">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="4f605-108">Der Name der Eigenschaft in der Eigenschaft-Wert-Paar ist ein app-spezifischen Bezeichner des Kontexts. der Wert ist das [PlannerPlanContextDetails](plannerplancontextdetails.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="4f605-108">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="4f605-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4f605-109">Properties</span></span>
<span data-ttu-id="4f605-110">Eigenschaften vom Typ open können vom Client definiert werden.</span><span class="sxs-lookup"><span data-stu-id="4f605-110">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="4f605-111">In diesem Fall sollte der Client einen charakteristischen Bezeichner verwenden, der den externen Kontext wie der Name der Eigenschaft darstellt.</span><span class="sxs-lookup"><span data-stu-id="4f605-111">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="4f605-112">Die Eigenschaftswerte muss [PlannerPlanContextDetails](plannerplancontextdetails.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="4f605-112">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="4f605-113">Basierend auf OData, Eigenschaftennamen im offenen Typen die folgenden Zeichen nicht enthalten: `.`, `:`, `@`, `%`.</span><span class="sxs-lookup"><span data-stu-id="4f605-113">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="4f605-114">Diese Zeichen mit URL-Codierung Format codiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="4f605-114">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="4f605-115">Um ein Element in der Liste der Favoriten zu entfernen, muss der Wert aus der Auflistung [PlannerPlanContextCollection](plannerplancontextcollection.md) stattdessen entfernt werden die wird automatisch den Eintrag in diesem Objekt zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="4f605-115">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
