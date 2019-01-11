---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityStat
localization_priority: Normal
ms.openlocfilehash: d0917d0100d33abee1095e2a7d06a4732d382937
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854250"
---
# <a name="itemactivitystat-resource-type"></a>Ressourcentyp itemActivityStat

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
| isTrending       | Boolean                 | Gibt an, ob das Element "Trend." Schreibgeschützt.
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

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivityStat object provides information about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActivityStat"
} -->
