---
title: Prozess Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 36acd6ed0f6e2cee5095d445de3ba4ff024a024a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869468"
---
# <a name="process-resource-type"></a>Prozess Ressourcentyp

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Statusinformationen über den Prozess im Zusammenhang mit der Benachrichtigung enthält.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|accountName|Zeichenfolge|Benutzerkonto für Beispiel, Kontoname, SID und So weiter Bezeichner (Konto Benutzerkontext, unter dem Prozess steht).|
|commandLine|Zeichenfolge|Vollständiger Prozess Aufruf Commandline einschließlich aller Parameter.|
|createdDateTime|DateTimeOffset|Zeitpunkt, an dem der Prozess gestartet wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|fileHash|[fileHash](filehash.md)|Komplexer Typ mit Dateihashes (cryptographic und der Speicherort).|
|integrityLevel|processIntegrityLevel|Die Integritätsebene des Prozesses. Mögliche Werte sind: `unknown`, `untrusted`, `low`, `medium`, `high` und `system`.|
|isElevated|Boolescher Wert|True, wenn der Prozess erweitert wird.|
|name|Zeichenfolge|Der Name der Bilddatei des Prozesses.|
|parentProcessCreatedDateTime|DateTimeOffset|DateTime, an dem der übergeordnete Prozess gestartet wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|Diese Eigenschaft|Int32|Die Prozess-ID (PID) des übergeordneten Vorgangs.|
|parentProcessName|Zeichenfolge|Der Name der Bilddatei des übergeordneten Vorgangs.|
|Pfad|Zeichenfolge|Vollständiger Pfad, einschließlich Dateiname.|
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
