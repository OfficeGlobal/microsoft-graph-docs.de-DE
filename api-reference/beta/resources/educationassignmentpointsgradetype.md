---
title: Ressourcentyp educationAssignmentPointsGradeType
description: Mit der **assignments.grading** -Eigenschaft verwendet. Dies ist eine Unterklasse der EducationAssignmentGradeType.
localization_priority: Normal
ms.openlocfilehash: f00014eab1dbf7bc8eb78a8898c6abba9977e8a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860970"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a>Ressourcentyp educationAssignmentPointsGradeType

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Mit der **assignments.grading** -Eigenschaft verwendet. Dies ist eine Unterklasse der [EducationAssignmentGradeType](educationassignmentgradetype.md).

Dies gibt an, dass die Zuordnung bewertet ist und speichert die maximale Anzahl von Punkten, die Studenten erreichen kann auf diese Arbeitsaufgabe. Wenn dies an einer Zuordnung festgelegt ist, erhält jede Übermittlung eine [EducationAssignmentPointsGrade](educationassignmentpointsgrade.md) -Eigenschaft für das Speichern von jeder Student Punkt zugeordnet.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|maxPoints|Single| Max Punkte mögliche für diese Zuordnung.  |

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
