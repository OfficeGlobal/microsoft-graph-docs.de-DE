---
title: Ressourcentyp plannerFavoritePlanReference
description: 'Die Ressource **PlannerFavoritePlanReference** Repesents Geben Sie einen Verweis auf eine PlannerPlan, die markiert wurde als Favoriten des Benutzers. '
localization_priority: Normal
ms.openlocfilehash: b17846eaa1b9a9859d23735d18a191cae4872542
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871323"
---
# <a name="plannerfavoriteplanreference-resource-type"></a>Ressourcentyp plannerFavoritePlanReference

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Ressource **PlannerFavoritePlanReference** Repesents Geben Sie einen Verweis auf eine [PlannerPlan](plannerplan.md) , die markiert wurde als Favoriten des Benutzers. Clients Beachten Sie, dass Einträge **PlannerFavoritePlanReference** **PlannerPlans** , die gelöscht werden, die der Benutzer zugreifen kann nicht mehr oder die mit einem anderen Titel aktualisiert wurden, verweisen können.

Es wird empfohlen, dass Clients benachrichtigen Sie Benutzer bei Diskrepanzen und die Einträge auf dem aktuellen Stand halten.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|orderHint|Zeichenfolge|Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist unter [Verwenden von Anordnungshinweisen in Planner](planner-order-hint-format.md) definiert.|
|planTitle|Zeichenfolge|Titel des Plans zur Zeit, dass der Benutzer als Favoriten markiert.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReference"
}-->

```json
{
  "orderHint": "String",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
