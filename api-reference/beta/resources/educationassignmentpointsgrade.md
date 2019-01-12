---
title: Ressourcentyp educationAssignmentPointsGrade
description: Wenn eine Zuordnung zu einem Punkt Note festgelegt ist, wird jede Übermittlung dieses Objekt die **submission.grade** -Eigenschaft zugeordnet haben. Dadurch wird eine Unterklasse von EducationAssignmentGrade,
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: d96b84380bc7a6d2298117b5dfeaee25d943efb2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982386"
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
