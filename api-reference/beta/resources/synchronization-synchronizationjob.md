---
title: Ressourcentyp synchronizationJob
description: Führt eine Synchronisierung von in regelmäßigen Abständen im Hintergrund ausgeführt, abrufen, damit die Änderungen in ein Verzeichnis und pushen von in ein anderes Verzeichnis. Der Synchronisierungsauftrag ist immer spezifisch für eine bestimmte Instanz einer Anwendung in Ihrem Mandanten. Im Rahmen der Synchronisierung Einrichtung müssen Sie die Autorisierung zum Lesen und Schreiben von Objekten in Ihrem Zielverzeichnis übergeben, und passen den Auftrag Synchronisierungsschema.
ms.openlocfilehash: 0e6428f2a088e5326f4412e743489c4d94b10296
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065577"
---
# <a name="synchronizationjob-resource-type"></a>Ressourcentyp synchronizationJob

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Führt eine Synchronisierung von in regelmäßigen Abständen im Hintergrund ausgeführt, abrufen, damit die Änderungen in ein Verzeichnis und pushen von in ein anderes Verzeichnis. Der Synchronisierungsauftrag ist immer spezifisch für eine bestimmte Instanz einer Anwendung in Ihrem Mandanten. Im Rahmen der Synchronisierung Einrichtung müssen Sie die Autorisierung zum Lesen und Schreiben von Objekten in Ihrem Zielverzeichnis übergeben, und passen den Auftrag Synchronisierungsschema.

## <a name="methods"></a>Methoden

| Methode        | Rückgabetyp               | Beschreibung                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationjob-list.md)             |[SynchronizationJob](synchronization-synchronizationjob.md) -Auflistung  |Vorhandene Aufträge für eine Instanz einer Anwendung (Service Principal) auflisten.|
|[Abrufen von synchronizationJob](../api/synchronization-synchronizationjob-get.md) | [synchronizationJob](synchronization-synchronizationjob.md) |Lesen Sie Eigenschaften und die Beziehungen eines SynchronizationJob-Objekts.|
|[Create](../api/synchronization-synchronizationjob-post.md)         |[synchronizationJob](synchronization-synchronizationjob.md)   |Erstellen Sie neuen Auftrag für eine bestimmte Anwendung.|
|[Start](../api/synchronization-synchronizationjob-start.md)          |Keines   |Starten Sie die Synchronisierung. Wenn der Auftrag angehalten ist, der weiterhin an der Stelle, an dem der Auftrag angehalten wurde. Wenn der Auftrag in Quarantäne befindet, wird der Quarantänestatus gelöscht.|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |Keines   |Erzwingen, dass des Auftrags beginnen soll, und alle Objekte im Verzeichnis erneut verarbeitet.|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |Keines   |Synchronisierung vorübergehend anhalten. Der Fortschritt Auftragsstatus, einschließlich wird beibehalten, und der Auftrag wird weiterhin aus, wo es beim [Starten](../api/synchronization-synchronizationjob-start.md) aufgerufen wird unterbrochen.|
|[Delete](../api/synchronization-synchronizationjob-delete.md)        |Keine   |Anhalten Sie Synchronisierung, und löschen Sie alle den Status des Auftrags zugeordnet.|
|[Abrufen von synchrnoizationSchema](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |Rufen Sie den Auftrag effektive Synchronisierungsschema ab.|
|[SynchroizationSchema aktualisieren](../api/synchronization-synchronizationschema-update.md)    |Keines   |Aktualisieren des Schemas für den Auftrag-Synchronisierung. |
|[Überprüfen von Anmeldeinformationen](../api/synchronization-synchronizationjob-validatecredentials.md)|Keines|Testen Sie die angegebene Anmeldeinformationen gegen Zielverzeichnis.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ      | Beschreibung    |
|:--------------|:----------|:---------------|
|id             |String                     |Auftrags-ID eindeutig Synchronisierung. Schreibgeschützt.|
|Zeitplan       |[synchronizationSchedule](synchronization-synchronizationschedule.md)|Zeitplan zum Ausführen des Auftrags verwendet. Schreibgeschützt.|
|status         |[synchronizationStatus](synchronization-synchronizationstatus.md)     |Status des Auftrags, die bei der letzten des Auftrags Ausführung enthält, aktuellen Auftragsstatus und Fehler.|
|templateId     |Zeichenfolge    |Bezeichner der [Synchronisierung Vorlage](synchronization-synchronizationtemplate.md) basiert auf diesen Auftrag.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Schema|[synchronizationSchema](synchronization-synchronizationschema.md)| Die Synchronisierungsschema-für den Auftrag konfiguriert.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "templateId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->