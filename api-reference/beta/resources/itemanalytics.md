---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemAnalytics
localization_priority: Normal
ms.openlocfilehash: 72e7f4de752ec04fbc5ebd98655254e2597fa499
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514964"
---
# <a name="itemanalytics-resource-type"></a>Ressourcentyp itemAnalytics

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "The ItemAnalytics object provides analytics about activities that took place on an item.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemAnalytics",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemanalytics.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
