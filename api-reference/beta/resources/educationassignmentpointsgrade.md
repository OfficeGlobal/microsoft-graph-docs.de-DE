---
title: Ressourcentyp educationAssignmentPointsGrade
description: Wenn eine Zuordnung zu einem Punkt Note festgelegt ist, wird jede Übermittlung dieses Objekt die **submission.grade** -Eigenschaft zugeordnet haben. Dadurch wird eine Unterklasse von EducationAssignmentGrade,
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5d2a5cf6f6f886185179c6f1a61c1bb1d9d1ecfc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523736"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>Ressourcentyp educationAssignmentPointsGrade

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Wenn eine Zuordnung zu einem Punkt Note festgelegt ist, wird jede Übermittlung dieses Objekt die **submission.grade** -Eigenschaft zugeordnet haben. Dadurch wird eine Unterklasse von [EducationAssignmentGrade](educationassignmentgrade.md), die die, die Daten für diese Eigenschaft hinzufügen. Die maximale Punkte in die **assignments.grading** -Eigenschaft gespeichert ist.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|points|Einzel|Anzahl von Punkten a Lehrer ist dieses Objekt Übermittlung erteilen.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
