---
title: Ressourcentyp governanceSchedule
description: 'Stellt den Zeitplan für einen GovernanceRoleAssignmentRequest dar. Der Zeitplan für eine Rolle Zuordnung Anforderung steuert beim Ausführen dieses Vorgangs Rolle Zuordnung für die rollenzuweisung beenden und wie häufig die Rolle Zuordnung Operation durchzuführen. '
localization_priority: Normal
ms.openlocfilehash: d7ccfe74804166ad2204ea02c072d79341cf75e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508027"
---
# <a name="governanceschedule-resource-type"></a>Ressourcentyp governanceSchedule

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt den Zeitplan für einen [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)dar. Der Zeitplan für eine Rolle Zuordnung Anforderung steuert beim Ausführen dieses Vorgangs Rolle Zuordnung für die rollenzuweisung beenden und wie häufig die Rolle Zuordnung Operation durchzuführen. 



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|startDateTime|DateTimeOffset|Die Anfangszeit der rollenzuweisung. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|Die Endzeit der rollenzuweisung. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. *Hinweis: Wenn der Wert ist `null`, es gibt eine permanente Zuordnung an.*|
|type|String|Die rollenzuweisung planen Typ. Nur `Once` wird jetzt unterstützt.
|duration|Dauer|Die Dauer einer rollenzuweisung. Es ist eine TimeSpan-Format.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSchedule"
}-->

```json
{
  "duration": "String (timespan)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
