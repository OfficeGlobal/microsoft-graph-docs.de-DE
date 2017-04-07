# <a name="uploadsession-resource-type"></a>Uploadsession-Ressourcentyp

Die **UploadSession** Ressource enthält Informationen zum Hochladen von großen Dateien auf OneDrive, OneDrive for Business oder SharePoint-Dokumentbibliotheken.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "expirationDateTime": "timestamp",
  "nextExpectedRanges": ["string"],
  "uploadUrl": "url"
}

```
## <a name="properties"></a>Eigenschaften


| Eigenschaft             | Typ              |Beschreibung|
|:-------------------|:------------------|:----------|
| expirationDateTime | DateTimeOffset    | Datum und Uhrzeit in UTC, wenn die Upload Sitzung abläuft. Die vollständige Datei muss hochgeladen werden, bevor dieser Ablaufzeitpunkt erreicht wird. |
| nextExpectedRanges | String collection | Eine Zusammenstellung von Bytebereichen, die dem Server für die Datei fehlen. Diese Bereiche sind Null indiziert und haben das Format "Anfang-Ende" (z. B. zeigt "0-26" die ersten 27 Bytes der Datei an). |
| uploadUrl          | String            | Der URL-Endpunkt, der PUT-Anfragen für Bytebereiche der Datei akzeptiert. |

## <a name="additional-resources"></a>Zusätzliche Ressourcen

Unter [Hochladen große Dateien mit einer Sitzung Upload](../api/item_createUploadSession.md) finden Sie Details zum Hochladen von Dateien mit einer Sitzung.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "uploadSession resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->