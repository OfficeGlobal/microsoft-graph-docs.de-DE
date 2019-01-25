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
# <a name="plannerplancontextdetailscollection-resource-type"></a>Ressourcentyp plannerPlanContextDetailsCollection

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Die Ressource **PlannerPlanContextDetailsCollection** stellt die Auflistung von externen Kontexten mit denen ein Plans verknüpft ist. Diese Ressource ist ein offener Typ und ist Teil des [PlannerPlanDetails](plannerplandetails.md) -Objekts. Der Name der Eigenschaft in der Eigenschaft-Wert-Paar ist ein app-spezifischen Bezeichner des Kontexts. der Wert ist das [PlannerPlanContextDetails](plannerplancontextdetails.md) -Objekt.


## <a name="properties"></a>Eigenschaften
Eigenschaften vom Typ open können vom Client definiert werden. In diesem Fall sollte der Client einen charakteristischen Bezeichner verwenden, der den externen Kontext wie der Name der Eigenschaft darstellt. Die Eigenschaftswerte muss [PlannerPlanContextDetails](plannerplancontextdetails.md) -Objekte. Basierend auf OData, Eigenschaftennamen im offenen Typen die folgenden Zeichen nicht enthalten: `.`, `:`, `@`, `%`. Diese Zeichen mit URL-Codierung Format codiert werden müssen. Um ein Element in der Liste der Favoriten zu entfernen, muss der Wert aus der Auflistung [PlannerPlanContextCollection](plannerplancontextcollection.md) stattdessen entfernt werden die wird automatisch den Eintrag in diesem Objekt zu entfernen.


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
