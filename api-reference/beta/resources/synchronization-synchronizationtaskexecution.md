---
title: Ressourcentyp synchronizationTaskExecution
description: Enthält eine Zusammenfassung der Ergebnisse der Synchronisierungsauftrag ausführen.
localization_priority: Normal
ms.openlocfilehash: 99b6c66b15577ee4c6cbbf5ffe44e17cf0672696
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851506"
---
# <a name="synchronizationtaskexecution-resource-type"></a>Ressourcentyp synchronizationTaskExecution

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Enthält eine Zusammenfassung der Ergebnisse der Synchronisierungsauftrag ausführen.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|activityIdentifier           |Zeichenfolge |Bezeichner des Auftrags ausgeführt.|
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
|state                        |Zeichenfolge |Zusammenfassen das Ergebnis dieser Ausführung von Code. Mögliche Werte sind: `Succeeded`, `Failed` und `EntryLevelErrors`.|
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
