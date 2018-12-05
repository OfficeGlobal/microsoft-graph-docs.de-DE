---
title: Ressourcentyp synchronizationQuarantine
description: Enthält Informationen zu den Quarantäne Status einer SynchronizationJob.
ms.openlocfilehash: b29da9644968ffe17abb02010f8aa5c304ca7905
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058940"
---
# <a name="synchronizationquarantine-resource-type"></a>Ressourcentyp synchronizationQuarantine

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Enthält Informationen zu den Quarantäne Status einer [SynchronizationJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|currentBegan|DateTimeOffset|Datum und Uhrzeit, wann die Quarantäne letzten, ausgewertet und eingeführt. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|nextAttempt|DateTimeOffset|Datum und Uhrzeit beim nächste Versuch die Quarantäne für die Überprüfung erfolgt. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|Grund|String|Ein Code, der angibt, warum die Quarantäne eingeführt wurde. Mögliche Werte sind: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException` und `Unknown`.|
|seriesBegan|DateTimeOffset|Datum und Uhrzeit, als die Quarantäne zunächst, in dieser Reihe (eine Datenreihe beginnt eingeführt wurde, wenn eine Quarantäne wird zuerst eingeführt und wird zurückgesetzt, sobald die Quarantäne transformiert ist). Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|seriesCount|Int64|Wie oft dieser Serie aus der Quarantäne wurde erneut ausgewertet und Links in Kraft (eine Datenreihe beginnt, wenn Quarantäne wird zuerst eingeführt und wird als Quarantäne transformiert wird zurückgesetzt).|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}-->

```json
{
  "currentBegan": "String (timestamp)",
  "nextAttempt": "String (timestamp)",
  "reason": "String",
  "seriesBegan": "String (timestamp)",
  "seriesCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->