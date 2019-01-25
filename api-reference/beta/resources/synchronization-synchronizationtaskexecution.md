---
title: Ressourcentyp synchronizationTaskExecution
description: Enthält eine Zusammenfassung der Ergebnisse der Synchronisierungsauftrag ausführen.
localization_priority: Normal
ms.openlocfilehash: 37a0fd57269cef6d3cb03c5cc5c38d3024fe198d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510554"
---
# <a name="synchronizationtaskexecution-resource-type"></a>Ressourcentyp synchronizationTaskExecution

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Enthält eine Zusammenfassung der Ergebnisse der Synchronisierungsauftrag ausführen.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|activityIdentifier           |String |Bezeichner des Auftrags ausgeführt.|
|countEntitled                |Int64  |Anzahl der verarbeiteten Einträge, die für diese Anwendung zugewiesen wurden.|
|countEntitledForProvisioning |Int64  |Anzahl der verarbeiteten Einträge, die für die Bereitstellung zugewiesen wurden.|
|countEscrowed                |Int64  |Anzahl der Einträge, die escrowed (Fehler) waren.|
|countEscrowedRaw             |Int64  |Anzahl der Einträge, die vom System generierte Artikel mit Treuhandservice einschließlich escrowed wurden.|
|countExported                |Int64  |Anzahl der exportierten Posten.|
|countExports                 |Int64  |Anzahl der Einträge, die erwartet wurden, exportiert werden sollen.|
|countImported                |Int64  |Anzahl der importierten Einträge.|
|countImportedDeltas          |Int64  |Anzahl der importierten Delta-Änderungen.|
|countImportedReferenceDeltas |Int64  |Anzahl der importierten Delta-Änderungen, die Verweis ändert betreffen.|
|error                        |[synchronizationError](synchronization-synchronizationerror.md)|Wenn ein Fehler aufgetreten ist, enthält ein **SynchronizationError** -Objekt mit Details.|
|state                        |String |Zusammenfassen das Ergebnis dieser Ausführung von Code. Mögliche Werte sind: `Succeeded`, `Failed` und `EntryLevelErrors`.|
|timeBegan                    |DateTimeOffset|Uhrzeit diesen Auftrag Ausführung begonnen hat. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|timeEnded                    |DateTimeOffset|Zeitpunkt der Ausführung dieser Auftrag beendet wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTaskExecution"
}-->

```json
{
  "activityIdentifier": "String",
  "countEntitled": 1024,
  "countEntitledForProvisioning": 1024,
  "countEscrowed": 1024,
  "countEscrowedRaw": 1024,
  "countExported": 1024,
  "countExports": 1024,
  "countImported": 1024,
  "countImportedDeltas": 1024,
  "countImportedReferenceDeltas": 1024,
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "state": "String",
  "timeBegan": "String (timestamp)",
  "timeEnded": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtaskexecution.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
