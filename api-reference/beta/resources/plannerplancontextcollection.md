---
title: Ressourcentyp plannerPlanContextCollection
description: Die Ressource **PlannerPlanContextCollection** stellt die Auflistung von externen Kontexten mit denen ein Plans verknüpft ist. Diese Ressource ist ein offener Typ und ist Teil des PlannerPlan-Objekts. Der Wert in der Eigenschaft-Wert-Paar ist das PlannerPlanContext-Objekt.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6ec515a164c5b0fca6334930b55a4b5d4e73b7d9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516497"
---
# <a name="plannerplancontextcollection-resource-type"></a>Ressourcentyp plannerPlanContextCollection

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Die Ressource **PlannerPlanContextCollection** stellt die Auflistung von externen Kontexten mit denen ein Plans verknüpft ist. Diese Ressource ist ein offener Typ und ist Teil des [PlannerPlan](plannerplan.md) -Objekts. Der Wert in der Eigenschaft-Wert-Paar ist das [PlannerPlanContext](plannerplancontext.md) -Objekt.


## <a name="properties"></a>Eigenschaften
Sie können die Eigenschaften dieses Typs open definieren. Die Eigenschaftswerte sollte charakteristischen Bezeichner, der den externen Kontext wie der Name der Eigenschaft darstellt. Die Eigenschaftswerte muss [PlannerPlanContext](plannerplancontext.md) -Objekte. Basierend auf OData-Anforderungen, Eigenschaftennamen im offenen Typen die folgenden Zeichen nicht enthalten: `.`, `:`, `%`, `@`. Diese Zeichen mit URL-Codierung codiert werden müssen. Wenn ein Element in der Liste der Favoriten entfernen möchten, legen Sie den Wert der Eigenschaft `null`.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextcollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
