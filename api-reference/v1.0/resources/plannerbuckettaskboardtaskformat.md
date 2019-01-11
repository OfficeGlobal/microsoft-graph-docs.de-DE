---
title: plannerBucketTaskBoardTaskFormat-Ressourcentyp
description: Die **plannerBucketTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Buckets“ des Task Board verwendet werden (eine Ansicht, die nach den Aufgaben in den Buckets organisiert ist, denen sie zugewiesen sind). Jeder Aufgabe ist ein **plannerBucketTaskBoardTaskFormat**-Objekt zugeordnet.
localization_priority: Normal
ms.openlocfilehash: a4fae04147bb97a7128f7b8ad881ac9b34cb7d8c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836078"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a>plannerBucketTaskBoardTaskFormat-Ressourcentyp

Die **plannerBucketTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Buckets“ des Task Board verwendet werden (eine Ansicht, die nach den Aufgaben in den Buckets organisiert ist, denen sie zugewiesen sind). Jeder [Aufgabe](plannertask.md) ist ein **plannerBucketTaskBoardTaskFormat**-Objekt zugeordnet.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerBucketTaskBoardTaskFormat abrufen](../api/plannerbuckettaskboardtaskformat-get.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerBucketTaskBoardTaskFormat**-Objekts.|
|[Update](../api/plannerbuckettaskboardtaskformat-update.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)  |Dient zum Aktualisieren des **plannerBucketTaskBoardTaskFormat**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|Zeichenfolge| Schreibgeschützt. Die ID der Ressource. Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet. [Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.|
|orderHint|Zeichenfolge|Hinweis, der zum Anordnen von Aufgaben in der Ansicht „Buckets“ des Task Board verwendet wird. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
