---
title: Ressourcentyp plannerRecentPlanReference
description: 'Die Ressource **PlannerRecentPlanReference** Repesents Geben Sie einen Verweis auf eine PlannerPlan, die kürzlich von einem Benutzer angezeigt wurde. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: bafaf6d20dc8f64ffe49eb4e2f998607708a2773
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943529"
---
# <a name="plannerrecentplanreference-resource-type"></a>Ressourcentyp plannerRecentPlanReference

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Ressource **PlannerRecentPlanReference** Repesents Geben Sie einen Verweis auf eine [PlannerPlan](plannerplan.md) , die kürzlich von einem Benutzer angezeigt wurde. Die **PlannerRecentPlanReferences** für einen Benutzer werden explizit verwaltet von apps. Alle Apps, die das letzte Pläne Feature implementiert sollte zu notieren, wenn der Benutzer zuletzt einen Plan und Update **PlannerRecentPlanReference** Einträge entsprechend angezeigt.
Apps Beachten Sie, dass Einträge **PlannerRecentPlanReference** **PlannerPlans** , die gelöscht werden, die der Benutzer zugreifen kann nicht mehr oder die mit einem anderen Titel aktualisiert wurden, verweisen können.
Es wird empfohlen, dass apps benachrichtigen Sie Benutzer bei Diskrepanzen und die Einträge auf dem aktuellen Stand halten.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|lastAccessedDateTime|DateTimeOffset|Das Datum und die Zeit, die vom Benutzer zuletzt des Plans angezeigt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|planTitle|Zeichenfolge|Der Titel des Plans zum Zeitpunkt der Benutzer es angezeigt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReference"
}-->

```json
{
  "lastAccessedDateTime": "String (timestamp)",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
