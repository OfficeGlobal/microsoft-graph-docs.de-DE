---
title: plannerUser-Ressourcentyp
description: 'Die Ressource **PlannerUser** bietet Zugriff auf Ressourcen Planner für einen Benutzer. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1b240092e7476884399f88fad61551763f33fe69
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928283"
---
# <a name="planneruser-resource-type"></a>plannerUser-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Ressource **PlannerUser** bietet Zugriff auf Ressourcen Planner für einen [Benutzer](user.md). 


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Aufgaben auflisten](../api/planneruser-list-tasks.md) |[plannerTask](plannertask.md)-Sammlung| Rufen Sie die [PlannerTasks](plannertask.md) die ihm zugewiesen wurde.|
|[Liste favoritePlans](../api/planneruser-list-favoriteplans.md) |[plannerPlan](plannerplan.md)-Sammlung| Rufen Sie die [PlannerPlans](plannerplan.md) durch den Benutzer als bevorzugten markiert.|
|[Liste recentPlans](../api/planneruser-list-recentplans.md) |[plannerPlan](plannerplan.md)-Sammlung| Rufen Sie die [PlannerPlans](plannerplan.md) zuletzt vom Benutzer angezeigt.|
|[Update](../api/planneruser-update.md) | [plannerUser](planneruser.md)| Aktualisieren eines **PlannerUser** -Objekts. |


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|Zeichenfolge| Schreibgeschützt. Bezeichner des der plannerUser|
|favoritePlanReferences|[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md)| Eine Auflistung mit der Verweise auf die Pläne, die der Benutzer als Favoriten gekennzeichnet hat.|
|recentPlanReferences|[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md)| Eine Auflistung mit Verweisen auf die Pläne, die zuletzt vom Benutzer in apps angezeigt wurden, die zuletzt verwendete Pläne zu unterstützen.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|tasks|[plannerTask](plannertask.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Gibt die dem Benutzer zugewiesenen [plannerTasks](plannertask.md) zurück.|
|favoritePlans|[plannerPlan](plannerplan.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Gibt die [PlannerPlans](plannerplan.md) , die der Benutzer als Favoriten gekennzeichnet.|
|recentPlans|[plannerPlan](plannerplan.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Gibt die [PlannerPlans](plannerplan.md) , die zuletzt vom Benutzer in apps angezeigt wurden, die zuletzt verwendete Pläne zu unterstützen. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "favoritePlanReferences": {"@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"},
  "id": "String (identifier)",
  "recentPlanReferences": {"@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
