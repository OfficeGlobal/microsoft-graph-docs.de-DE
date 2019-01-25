---
title: Ressourcentyp educationAssignmentPointsGradeType
description: Mit der **assignments.grading** -Eigenschaft verwendet. Dies ist eine Unterklasse der EducationAssignmentGradeType.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 567bff38f8a20456dffffdd91775a1e32852fe20
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508895"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>Ressourcentyp educationAssignmentPointsGradeType

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mit der **assignments.grading** -Eigenschaft verwendet. Dies ist eine Unterklasse der [EducationAssignmentGradeType](educationassignmentgradetype.md).

Dies gibt an, dass die Zuordnung bewertet ist und speichert die maximale Anzahl von Punkten, die Studenten erreichen kann auf diese Arbeitsaufgabe. Wenn dies an einer Zuordnung festgelegt ist, erhält jede Übermittlung eine [EducationAssignmentPointsGrade](educationassignmentpointsgrade.md) -Eigenschaft für das Speichern von jeder Student Punkt zugeordnet.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|maxPoints|Einzel| Max Punkte mögliche für diese Zuordnung.  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType"
}-->

```json
{
  "maxPoints": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgradetype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
