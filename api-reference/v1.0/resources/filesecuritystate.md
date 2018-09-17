# <a name="filesecuritystate-resource-type"></a>Ressourcentyp fileSecurityState

Enthält Informationen über die Datei (nicht den Vorgang) im Zusammenhang mit der Warnung.

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Komplexer Typ mit Datei-Hashes (kryptographisch und der ortsabhängig).|
|Name|Zeichenfolge|Der Dateiname (ohne Pfad).|
|Pfad|Zeichenfolge|Dateiname (ohne Pfad)|
|riskScore|Zeichenfolge|Vom Anbieter generierte/berechnete Risikobewertung der Warnungs-Datei. Empfohlener Wertebereich von 0-1, was einem Prozentsatz entspricht.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->