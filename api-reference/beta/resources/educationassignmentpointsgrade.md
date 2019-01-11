---
title: Ressourcentyp educationAssignmentPointsGrade
description: Wenn eine Zuordnung zu einem Punkt Note festgelegt ist, wird jede Übermittlung dieses Objekt die **submission.grade** -Eigenschaft zugeordnet haben. Dadurch wird eine Unterklasse von EducationAssignmentGrade,
localization_priority: Normal
ms.openlocfilehash: 2084a1bda6784165576c3ec454fa9ee88601c952
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861404"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>Ressourcentyp educationAssignmentPointsGrade

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Wenn eine Zuordnung zu einem Punkt Note festgelegt ist, wird jede Übermittlung dieses Objekt die **submission.grade** -Eigenschaft zugeordnet haben. Dadurch wird eine Unterklasse von [EducationAssignmentGrade](educationassignmentgrade.md), die die, die Daten für diese Eigenschaft hinzufügen. Die maximale Punkte in die **assignments.grading** -Eigenschaft gespeichert ist.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|points|Single|Anzahl von Punkten a Lehrer ist dieses Objekt Übermittlung erteilen.|

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
