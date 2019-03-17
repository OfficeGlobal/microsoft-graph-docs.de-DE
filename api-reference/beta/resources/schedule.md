---
title: Ressourcentyp planen
description: Eine Sammlung von schedulingGroups, Schichten, timeOffReasons und timesOff innerhalb eines Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: de3662fcf3c5a8e50493e365f6a10a8641a451df
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657511"
---
# <a name="schedule-resource-type"></a>Ressourcentyp planen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Auflistung von [schedulinggroup](schedulinggroup.md) -Objekten, [Shift](shift.md) -Objekten, [timeOffReason](timeoffreason.md) -Objekten und [timeOff](timeoff.md) -Objekten innerhalb eines [Teams](../resources/team.md). 

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Erstellen oder Ersetzen eines Zeitplans](../api/team-put-schedule.md) | [Zeitplan](schedule.md) | Erstellen oder ersetzen Sie `schedule`ein.|
|[Zeitplan abrufen](../api/schedule-get.md) | [Zeitplan](schedule.md) | Get a `schedule`.|
|[share](../api/schedule-share.md) | None | Teilen Sie `schedule` einen Zeitraum mit Schedule-Elementen.|

## <a name="properties"></a>Eigenschaften
|Name                   |Typ           |Beschreibung                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    |`string`  |ID des `schedule`.|
| aktiviert               |`bool`    | Gibt an, ob der Zeitplan für das Team aktiviert ist. Erforderlich.|
| timeZone              |`string`  | Gibt die Zeitzone des Zeit Plan Teams mit dem TZ-Datenbankformat an. Erforderlich.|
| provisionStatus       |`enum`    | Der Status der Terminplanung. |
| provisionStatusCode   |`string`  | Weitere Informationen dazu, warum die Planung fehlgeschlagen ist. |


## <a name="relationships"></a>Beziehungen
|Name                   |Typ           |Beschreibung                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| Verschiebungen   |`collection(shift)`  | Die Verschiebungen im Zeitplan. |
| timesOff   |`collection(timeOff)`  | Die Instanzen von Zeiten, die im Zeitplan deaktiviert sind. |
| timeOffReasons   |`collection(timeOffReason)`  | Die Gründe für eine Zeitdauer im Zeitplan. |
| schedulingGroups   |`collection(schedulingGroup)`  | Die logische Gruppierung von Benutzern im Zeitplan (in der Regel nach Rolle). |


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedule"
}-->

```json
{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/schedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
