---
title: Ressourcentyp „timeConstraint“
description: Schränkt die Vorschläge für Besprechungszeiten auf bestimmte Stunden und Tage der Woche entsprechend der angegebenen Aktivität und den geöffneten Zeitschlitzen ein.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 680ada778ea64f982e9ed5fac11c935a6cce55d5
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/28/2019
ms.locfileid: "30937784"
---
# <a name="timeconstraint-resource-type"></a>Ressourcentyp „timeConstraint“

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Schränkt die Vorschläge für Besprechungszeiten auf bestimmte Stunden und Tage der Woche entsprechend der angegebenen Aktivität und den geöffneten Zeitschlitzen ein.


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}
```

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|activityDomain|activityDomain|Die Art der Aktivität, optional. Mögliche Werte sind: `work`, `personal`, `unrestricted`oder `unknown`.|
|timeslots|[timeSlot](timeslot.md) collection|Ein Array von Zeitfenstern|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeconstraint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->