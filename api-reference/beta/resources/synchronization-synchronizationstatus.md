---
title: Ressourcentyp synchronizationStatus
description: Stellt den aktuellen Status der SynchronizationJob.
localization_priority: Normal
ms.openlocfilehash: 404fe4f7f58b8189b3059c212aa1ce858350bb01
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523764"
---
# <a name="synchronizationstatus-resource-type"></a>Ressourcentyp synchronizationStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt den aktuellen Status der [SynchronizationJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Eigenschaften

| Eigenschaft                              | Typ      | Beschreibung    |
|:--------------------------------------|:----------|:---------------|
|code|String|Allgemeine Statuscode des Synchronisierungsauftrags. Mögliche Werte sind: `NotConfigured`, `NotRun`, `Active`, `Paused` und `Quarantine`.|
|countSuccessiveCompleteFailures|Int64|Häufigkeit der aufeinander folgenden diesen Auftrag ist fehlgeschlagen.|
|escrowsPruned|Boolescher Wert|`true`Wenn der Auftrag Artikel mit Treuhandservice (Fehler auf Objektebene) während der ersten Synchronisierung gelöscht wurden. Artikel mit Treuhandservice können gelöscht werden, wenn während der ersten Synchronisierung des Schwellenwerts für Fehler erreichen, die normalerweise den Auftrag in Quarantäne eingetragen wird. Statt in Quarantäne Synchronisierungsvorgangs löscht den Auftrag Fehler und wird fortgesetzt, bis die anfängliche Synchronisierung abgeschlossen ist. Wenn die anfängliche Synchronisierung abgeschlossen ist, wird der Auftrag anhalten und warten, bis der Kunde, um den Fehler zu bereinigen.|
|lastExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Details der letzten Ausführung des Auftrags.|
|lastSuccessfulExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Details der letzten Ausführung dieser Auftrag, die Fehler aufweisen, nicht.|
|lastSuccessfulExecutionWithExports|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Details der letzten Ausführung des Auftrags, der exportierte Objekte in das Zielverzeichnis.|
|progress|[SynchronizationProgress](synchronization-synchronizationprogress.md) -Auflistung|Details zu den Fortschritt eines Auftrags an.|
|Quarantäne|[synchronizationQuarantine](synchronization-quarantine.md)|Wenn der Auftrag in Quarantäne ist, Quarantänedetails.|
|steadyStateFirstAchievedTime|DateTimeOffset|Der Zeitpunkt, wann stabilen Zustand (keine weitere Änderungen an den Prozess) zuerst erreicht wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|steadyStateLastAchievedTime|DateTimeOffset|Die Uhrzeit, wann zuletzt stabilen Zustand (keine weitere Änderungen an den Prozess) erreicht wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|synchronizedEntryCountByType|[StringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) -Auflistung|Anzahl der synchronisierten Objekte nach Objekttyp aufgeführt.|
|troubleshootingUrl|String|Im Fall eines Fehlers, die URL durch die Schritte zur Problembehandlung für das Problem.|

### <a name="synchronization-status-code-details"></a>Synchronisierung Status Code details

| Wert                              | Beschreibung    |
|:-----------------------------------|:---------------|
|Nicht konfiguriert                       |Auftrag wurde nicht konfiguriert und nie ausführen. Es wurde keine Autorisierung bereitgestellt. |
|NotRun                              |Auftrag konfiguriert wurde, und möglicherweise gestartet, aber der ersten Ausführung noch nicht abgeschlossen wurde.|
|Aktiv                              |Auftrag wird in regelmäßigen Abständen ausgeführt.|
|Angehalten                              |Auftrag (normalerweise von einem Administrator) angehalten wurde und wird derzeit nicht ausgeführt, aber der Status des Auftrags wird beibehalten.|
|Quarantäne                          |Auftrag ist in Quarantäne. Dies kann vorkommen, wenn eine große Menge von Fehlern oder kritische Fehler wie widerrufen/Abgelaufene Anmeldeinformationen vorhanden ist. In Quarantäne, versucht Synchronisierungsvorgangs mit Geringere Häufigkeit den Auftrag ausgeführt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
}-->

```json
{
  "code": "String",
  "countSuccessiveCompleteFailures": 1024,
  "escrowsPruned": true,
  "lastExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecutionWithExports": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "progress": [{"@odata.type": "microsoft.graph.synchronizationProgress"}],
  "quarantine": {"@odata.type": "microsoft.graph.synchronizationQuarantine"},
  "steadyStateFirstAchievedTime": "String (timestamp)",
  "steadyStateLastAchievedTime": "String (timestamp)",
  "synchronizedEntryCountByType": [{"@odata.type": "microsoft.graph.stringKeyLongValuePair"}],
  "troubleshootingUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
