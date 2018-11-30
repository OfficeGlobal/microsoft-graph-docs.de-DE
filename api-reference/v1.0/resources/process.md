---
title: Prozess Ressourcentyp
description: Statusinformationen über den Prozess im Zusammenhang mit der Benachrichtigung enthält.
ms.openlocfilehash: 67bc65cfa47cda877578d89aa20c4e34b3a0c501
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018942"
---
# <a name="process-resource-type"></a>Prozess Ressourcentyp

Statusinformationen über den Prozess im Zusammenhang mit der Benachrichtigung enthält.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|accountName|String|Benutzerkonto für Beispiel, Kontoname, SID und So weiter Bezeichner (Konto Benutzerkontext, unter dem Prozess steht).|
|commandLine|String|Vollständiger Prozess Aufruf Commandline einschließlich aller Parameter.|
|createdDateTime|DateTimeOffset|Zeitpunkt, an dem der Prozess gestartet wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|fileHash|[fileHash](filehash.md)|Komplexer Typ mit Dateihashes (cryptographic und der Speicherort).|
|integrityLevel|processIntegrityLevel|Die Integritätsebene des Prozesses. Mögliche Werte sind: `unknown`, `untrusted`, `low`, `medium`, `high` und `system`.|
|isElevated|Boolesch|True, wenn der Prozess erweitert wird.|
|name|String|Der Name der Bilddatei des Prozesses.|
|parentProcessCreatedDateTime|DateTimeOffset|DateTime, an dem der übergeordnete Prozess gestartet wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|Diese Eigenschaft|Int32|Die Prozess-ID (PID) des übergeordneten Vorgangs.|
|parentProcessName|String|Der Name der Bilddatei des übergeordneten Vorgangs.|
|Pfad|String|Vollständiger Pfad, einschließlich Dateiname.|
|processId|Int32|Die Prozess-ID (PID) des Prozesses.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->