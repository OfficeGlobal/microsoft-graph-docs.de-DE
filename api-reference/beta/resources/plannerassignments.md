---
title: plannerAssignments-Ressourcentyp
description: 'Die Ressource **PlannerAssignments** stellt Zuordnungen einer PlannerTask Ressource dar. Dieser Typ ist vom Typ öffnen. Jeder Eigenschaftsname dieses Typs '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2c379c786e3b94395aa3de7bc382e184db0fcc24
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507768"
---
# <a name="plannerassignments-resource-type"></a>plannerAssignments-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **plannerAssignments**-Ressource stellt Zuweisungen einer [plannerTask](plannertask.md)-Ressource dar. Es handelt sich um einen offenen Typ. Jeder Eigenschaftenname in diesem Typ ist die ID eines Benutzerobjekts, dem eine Aufgabe zugewiesen ist. Die Benutzer können Aufgaben zugewiesen werden, indem neue Eigenschaften mit dem Namen ihrer ID erstellt werden, wobei ein [plannerAssignment](plannerassignment.md)-Objekt mit der orderHint-Eigenschaft als Wert gefüllt wird. Die Zuweisung der zugewiesenen Personen zur Aufgabe kann aufgehoben werden, indem die Eigenschaft mit dem Namen ihrer ID auf „null“ festgelegt wird.


## <a name="properties"></a>Eigenschaften
Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client jedoch die IDs von zugewiesenen Benutzern als Eigenschaftennamen angeben. Die Eigenschaft muss auf ein **plannerAssignment**-Objekt festgelegt werden, um zugewiesene Personen zu erstellen oder zu ändern, und auf „null“, um sie zu entfernen.

Beispiel:

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignments"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": null,
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": { 
      "@odata.type": "microsoft.graph.plannerAssignment",
      "orderHint": "String"
    }
}
```
In diesem Beispiel wird der Benutzer mit der ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 aus der Liste der der Aufgabe zugewiesenen Personen entfernt; gleichzeitig wird die Anordnung der zugewiesenen Person mit der Benutzer-ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8 geändert. Wenn die Aufgabe nicht bereits dem Benutzer mit der ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8 zugewiesen ist, wird die Aufgabe durch Aktualisieren der Zuweisungen mit diesem Wert diesem Benutzer zugewiesen.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
