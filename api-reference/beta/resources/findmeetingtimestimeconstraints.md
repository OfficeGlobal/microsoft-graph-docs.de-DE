---
title: findMeetingTimesTimeConstraints-Ressourcentyp
description: Schränkt Vorschläge für Besprechungstermine entsprechend der angegebenen Art der Aktivität und der offenen Zeitfenster auf bestimmte Stunden und Tage der Woche ein.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e5790faf49fea03040dca05d457fededf5fdd683
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057386"
---
# <a name="findmeetingtimestimeconstraints-resource-type"></a>findMeetingTimesTimeConstraints-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Schränkt die Vorschläge für Besprechungszeiten auf die Art der Aktivität und bestimmte Zeiträume ein. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.findMeetingTimesTimeConstraints"
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
|activityDomain|activityDomain|Die Art der Aktivität. Diese Angabe ist optional. Mögliche Werte sind: `work`, `personal`, `unrestricted` oder `unknown`.|
|timeslots|[searchWindowTimeSlot](searchwindowtimeslot.md) -Sammlung|Ein Array von Zeitbereichen, in denen nach möglichen Besprechungszeiten gesucht werden soll.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "findMeetingTimesTimeConstraints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/findmeetingtimestimeconstraints.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->