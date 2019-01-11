---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
localization_priority: Normal
ms.openlocfilehash: 03626b5dad041181558af076b5dc0ac05b684e13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842413"
---
# <a name="itemanalytics-resource-type"></a>Ressourcentyp itemAnalytics

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Ressource **ItemAnalytics** bietet Analytics zu Aktivitäten, die für ein Element durchgeführt wurde. Diese Ressource ist derzeit nur auf SharePoint und OneDrive für Unternehmen verfügbar.

Sie können auch [GetActivitiesByInterval][] API verwenden, Analytics über einen benutzerdefinierten Zeitbereich oder Intervall abgerufen.

>**Hinweis:** Die Ressource **ItemAnalytics** ist noch nicht in allen [nationalen Bereitstellungen](/graph/deployments)verfügbar.

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemAnalytics",
  "@type.aka": "oneDrive.analytics"
}-->

```json
{
  "allTime": {"@odata.type": "microsoft.graph.itemActivityStat"},
  "lastSevenDays": {"@odata.type": "microsoft.graph.itemActivityStat"}
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ                 | Beschreibung
|:--------------|:---------------------|:--------------------------------------
| allTime       | [itemActivityStat][] | Analytics über die Lebensdauer des Elements.
| lastSevenDays | [itemActivityStat][] | Analyse für den letzten sieben Tagen.

[itemActivityStat]: itemactivitystat.md


[getActivitiesByInterval]: ../api/itemactivity-getbyinterval.md

<!-- {
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics"
} -->
