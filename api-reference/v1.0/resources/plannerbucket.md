---
title: plannerBucket-Ressourcentyp
description: ) für Aufgaben in einem Plan in Office 365. Er ist in einem PlannerPlan enthalten und kann eine Auflistung von PlannerTasks haben.
ms.openlocfilehash: 44bce1606fa7561bc52098fe0e6ba8f70d737a58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017055"
---
# <a name="plannerbucket-resource-type"></a>plannerBucket-Ressourcentyp

Die **plannerBucket**-Ressource stellt einen Bucket (bzw. eine „benutzerdefinierte Spalte“) für Aufgaben in einem Plan in Office 365 dar. Sie ist in einem [plannerPlan](plannerplan.md) enthalten und kann eine Sammlung von [plannerTasks](plannertask.md) haben.



## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerBucket abrufen](../api/plannerbucket-get.md) | [plannerBucket](plannerbucket.md) |Dient zum Lesen der Eigenschaften und Beziehungen des **plannerBucket**-Objekts.|
|[plannerTasks auflisten](../api/plannerbucket-list-tasks.md) |[plannerTask](plannertask.md)-Sammlung| Dient zum Abrufen einer **plannerTask**-Objektsammlung.|
|[Create](../api/planner-post-buckets.md) | [plannerBucket](plannerbucket.md)   | Dient zum Erstellen eines neuen **plannerBucket**-Objekts. |
|[Update](../api/plannerbucket-update.md) | [plannerBucket](plannerbucket.md)   |Dient zum Aktualisieren eines **plannerBucket**-Objekts. |
|[Delete](../api/plannerbucket-delete.md) | Keine |Dient zum Löschen eines **plannerBucket**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt. ID des Bucket. Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet. [Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.|
|name|String|Name des Buckets.|
|orderHint|String|Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.|
|planId|String|Plan-ID, zu der der Bucket gehört.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|tasks|[plannerTask](plannertask.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Die Sammlung von Aufgaben im Bucket.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->