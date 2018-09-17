# <a name="process-resource-type"></a>Ressourcentyp process

Enthält Zustandsinformationen über den Vorgang im Zusammenhang mit der Warnung.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|accountName|Zeichenfolge|Benutzerkontobezeichner (Benutzerkonto-Kontext, unter dem der Prozess gelaufen ist), z.B. AccountName, SID, etc.|
|commandLine|Zeichenfolge|Vollständiger Prozess-Aufruf-Eingabezeile einschließlich aller Parameter.|
|createdDateTime|DateTimeOffset|Zeitpunkt, an dem der Prozess gestartet wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|fileHash|[fileHash](filehash.md)|Komplexer Typ mit Datei-Hashes (kryptographisch und der ortsabhängig).|
|integrityLevel|processIntegrityLevel|Die Integritätsebene des Prozesses. Mögliche Werte sind: `unknown`, `untrusted`, `low`, `medium`, `high` und `system`.|
|isElevated|Boolesch|True, wenn der Prozess erhöht ist.|
|Name|Zeichenfolge|Der Name der Bilddatei des Prozesses.|
|parentProcessCreatedDateTime|DateTimeOffset|DateTime, an dem der übergeordnete Prozess gestartet wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|parentProcessId|Int32|Die Prozess-ID (PID) des übergeordneten Prozesses.|
|parentProcessName|Zeichenfolge|Der Name der Bilddatei des übergeordneten Vorgangs.|
|Pfad|Zeichenfolge|Vollständiger Pfad, einschließlich Dateiname.|
|processId|Int32|Die Prozess-ID (PID) des übergeordneten Prozesses.|

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