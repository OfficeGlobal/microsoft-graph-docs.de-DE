---
title: Ressourcentyp educationAssignmentPointsGradeType
description: Mit der **assignments.grading** -Eigenschaft verwendet. Dies ist eine Unterklasse der EducationAssignmentGradeType.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: b603ccec0ddd5be5003353a5062e51554cb61c53
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952664"
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
