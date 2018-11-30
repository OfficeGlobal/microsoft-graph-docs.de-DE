---
title: Ressourcentyp governanceSchedule
description: 'Stellt den Zeitplan für einen GovernanceRoleAssignmentRequest dar. Der Zeitplan für eine Rolle Zuordnung Anforderung steuert beim Ausführen dieses Vorgangs Rolle Zuordnung für die rollenzuweisung beenden und wie häufig die Rolle Zuordnung Operation durchzuführen. '
ms.openlocfilehash: 6eff3977aa7806c975f968b8706f2e8c21e5d99e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063203"
---
# <a name="governanceschedule-resource-type"></a>Ressourcentyp governanceSchedule

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt den Zeitplan für einen [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)dar. Der Zeitplan für eine Rolle Zuordnung Anforderung steuert beim Ausführen dieses Vorgangs Rolle Zuordnung für die rollenzuweisung beenden und wie häufig die Rolle Zuordnung Operation durchzuführen. 



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|startDateTime|DateTimeOffset|Die Anfangszeit der rollenzuweisung. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|Die Endzeit der rollenzuweisung. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. *Hinweis: Wenn der Wert ist `null`, es gibt eine permanente Zuordnung an.*|
|Typ|String|Die rollenzuweisung planen Typ. Nur `Once` wird jetzt unterstützt.
|duration|Duration|Die Dauer einer rollenzuweisung. Es ist eine TimeSpan-Format.|

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
