---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: 1362116c0dbe997eda941cb790e00e9ddb078ae4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517631"
---
# <a name="itemactivitystat-resource-type"></a>Ressourcentyp itemActivityStat

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die Ressource **ItemActivityStat** enthält Informationen zu Aktivitäten, die innerhalb eines Zeitintervalls durchgeführt wurde.

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "baseType": "microsoft.graph.entity",
  "@type": "microsoft.graph.itemActivityStat",
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "incompleteData": {"@odata.type": "microsoft.graph.incompleteData"},
  "isTrending": true,
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "create": {"@odata.type": "microsoft.graph.itemActionStat"},
  "delete": {"@odata.type": "microsoft.graph.itemActionStat"},
  "edit": {"@odata.type": "microsoft.graph.itemActionStat"},
  "move": {"@odata.type": "microsoft.graph.itemActionStat"},
  "access": {"@odata.type": "microsoft.graph.itemActionStat"}
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft         | Typ                    | Beschreibung
|:-----------------|:------------------------|:----------------------------------------
| incompleteData   | [incompleteData][]      | Gibt an, dass die Statistiken in diesem Zeitraum auf unvollständiger Daten basieren. Schreibgeschützt.
| isTrending       | Boolescher Wert                 | Gibt an, ob das Element "Trend." Schreibgeschützt.
| startDateTime    | DateTimeOffset          | Wenn das Intervall gestartet wird. Schreibgeschützt.
| endDateTime      | DateTimeOffset          | Wenn das Intervall endet. Schreibgeschützt.
| create           | [itemActionStat][]      | Statistiken zum **Erstellen von** Aktionen in diesem Zeitraum. Schreibgeschützt.
| Bearbeiten             | [itemActionStat][]      | Statistiken zum **Bearbeiten von** Aktionen in diesem Zeitraum. Schreibgeschützt.
| Löschen           | [itemActionStat][]      | Statistiken zu **Löschaktionen in diesem Zeitraum** . Schreibgeschützt.
| verschieben             | [itemActionStat][]      | Statistiken zu **Verschieben** Aktionen in diesem Zeitraum. Schreibgeschützt.
| access           | [itemActionStat][]      | Statistiken zu **Access** -Aktionen in diesem Zeitraum. Schreibgeschützt.

[itemActionStat]: itemactionstat.md
[incompleteData]: incompletedata.md

## <a name="relationships"></a>Beziehungen

| Beziehungsname | Typ                        | Beschreibung
|:------------------|:----------------------------|:---------------------------
| Aktivitäten        | [itemActivity][]-Sammlung | Macht die **ItemActivities** in diese Ressource **ItemActivityStat** dargestellt.

[itemActivity]: itemactivity.md

## <a name="remarks"></a>Bemerkungen

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivitystat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
