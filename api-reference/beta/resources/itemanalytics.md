---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemAnalytics
ms.openlocfilehash: b50df7d1fdf67cffd508c3b5891d07c599521c8a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060487"
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
