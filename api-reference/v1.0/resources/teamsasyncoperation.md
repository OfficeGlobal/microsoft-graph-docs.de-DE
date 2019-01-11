---
title: Ressourcentyp teamsAsyncOperation
description: 'Ein Microsoft-Teams, asynchroner Vorgang ist ein Vorgang, der die Lebensdauer der einzelnen API-Anforderung transcends. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 607730ff48213b45177560046dc6f38afe1bcc75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873619"
---
# <a name="teamsasyncoperation-resource-type"></a>Ressourcentyp teamsAsyncOperation



Ein Microsoft-Teams, asynchroner Vorgang ist ein Vorgang, der die Lebensdauer der einzelnen API-Anforderung transcends. Diese Vorgänge sind langer oder zu teuer, in dem Zeitrahmen ihrer ursprünglichen Anforderung abgeschlossen.

Wenn ein asynchroner Vorgang gestartet wird, gibt die Methode eine 202 akzeptierte Antwortcode zurück. Die Antwort enthält außerdem einen Location-Header, der den Speicherort der die TeamsAsyncOperation enthält. Überprüfen Sie regelmäßig den Status des Vorgangs, indem er eine GET-Anforderung an diesen Speicherort; Warten Sie > 30 Sekunden zwischen überprüft.
Wenn die Anforderung erfolgreich abgeschlossen wird, der Status wird werden "succeeded" und der TargetResourceLocation verweist auf die erstellte/geänderte Ressource.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ   | Beschreibung |
|:---------------|:--------|:----------|
|id|string |Eindeutige Vorgangs-Id.|
|Vorgangstyp|[teamsAsyncOperationType](teamsasyncoperationtype.md) |Gibt an, welche Art von Vorgang beschrieben wird.|
|createdDateTime|DateTimeOffset |Die Uhrzeit der Erstellung des Vorgangs.|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| Ausführungsstatus.|
|lastActionDateTime|DateTimeOffset |Zeitpunkt, wann die asynchrone Operation zuletzt aktualisiert wurde.|
|attemptsCount|Int32|Anzahl der Häufigkeit, mit die der Vorgang versucht wurde, vor der erfolgreichen oder fehlgeschlagenen markiert werden.|
|targetResourceId|GUID |Die ID des Objekts, das erstellt oder aufgrund dieses asynchronen Vorgangs, in der Regel ein [Team](../resources/team.md)geändert hat.|
|targetResourceLocation|string|Die Position des Objekts, das erstellt oder aufgrund dieses asynchronen Vorgangs geändert hat. Diese URL sollte als ein nicht transparenter Wert behandelt und nicht in ihre Pfadkomponenten analysiert werden.|
|error|[operationError](operationerror.md)|Alle Fehler, die bewirkt, dass die asynchrone Operation ein Fehler auftritt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsasyncoperation"
}-->

```json
{
    "id": "string",
    "operationType": "archiveTeam",
    "createdDateTime": "2018-01-01T00:00:00.0000000Z",
    "status": "succeeded",
    "lastActionDateTime": "2018-01-01T00:00:00.0000000Z",
    "attemptsCount": 1,
    "targetResourceId": "fa4aa5a2-a75b-4769-86f4-9e2742a18fda",
    "targetResourceLocation": "/groups('fa4aa5a2-a75b-4769-86f4-9e2742a18fda')/team",
    "error": null
}
```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
