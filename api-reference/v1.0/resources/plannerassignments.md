---
title: plannerAssignments-Ressourcentyp
description: 'Die Ressource **PlannerAssignments** stellt Zuordnungen einer PlannerTask Ressource dar. Dieser Typ ist vom Typ öffnen. Jeder Eigenschaftsname dieses Typs '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: bf079cbf91e0c9b8b1a8c92403324b301bbde923
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966818"
---
# <a name="plannerassignments-resource-type"></a>plannerAssignments-Ressourcentyp

Die **plannerAssignments**-Ressource stellt Zuweisungen einer [plannerTask](plannertask.md)-Ressource dar. Es handelt sich um einen offenen Typ. Jeder Eigenschaftenname in diesem Typ ist die ID eines Benutzerobjekts, dem eine Aufgabe zugewiesen ist. Die Benutzer können Aufgaben zugewiesen werden, indem neue Eigenschaften mit dem Namen ihrer ID erstellt werden, wobei ein [plannerAssignment](plannerassignment.md)-Objekt mit der orderHint-Eigenschaft als Wert gefüllt wird. Die Zuweisung der zugewiesenen Personen zur Aufgabe kann aufgehoben werden, indem die Eigenschaft mit dem Namen ihrer ID auf „null“ festgelegt wird.


## <a name="properties"></a>Eigenschaften
Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client jedoch die IDs von zugewiesenen Benutzern als Eigenschaftennamen angeben. Die Eigenschaft muss auf ein **plannerAssignment**-Objekt festgelegt werden, um zugewiesene Personen zu erstellen oder zu ändern, und auf „null“, um sie zu entfernen.

Beispiel:

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
