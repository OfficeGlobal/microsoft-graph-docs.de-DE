---
title: plannerOrderHintsByAssignee-Ressourcentyp
description: Die **PlannerOrderHintsByAssignee** ist eine Ressource, die Sortierung Hinweise für "assignees" in einer Ressource PlannerTask an, dass die Reihenfolge des Vorgangs in der Ansicht zugewiesen an der Aufgabe-Karte enthält.
localization_priority: Normal
ms.openlocfilehash: cdc254eab43972d321e01e646880b3087f3af6f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863945"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a>plannerOrderHintsByAssignee-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **plannerOrderHintsByAssignee**-Ressource enthält [Anordnungshinweise](planner-order-hint-format.md) für zugewiesene Personen in einer [plannerTask](plannertask.md)-Ressource, um die Anordnung der Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board anzugeben. Es handelt sich um einen offenen Typ. Die Eigenschaften sind die IDs der Benutzer, die der Aufgabe zugewiesen sind, und die Werte sind Anordnungshinweise.

## <a name="properties"></a>Eigenschaften
Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client IDs von Benutzern, die der Aufgabe zugewiesen sind, als Eigenschaftennamen und einen gültigen [Anordnungshinweis](planner-order-hint-format.md) als Wert angeben. Von diesem Typ können keine Eigenschaften entfernt werden. Der Dienst entfernt automatisch Werte, wenn die Zuweisungen in der enthaltenden [plannerTask](plannertask.md)-Ressource aktualisiert werden.

Beispiel:

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
