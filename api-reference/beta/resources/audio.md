# <a name="audio-resource-type"></a>Ressourcentyp Audio

Die Ressource **Audio** führt audiobezogene Eigenschaften für ein Element in einer einzelnen Struktur zusammen.

Wenn ein [**DriveItem**](driveitem.md)-Element ein **file**-Facet ungleich Null aufweist, stellt das Element eine Audiodatei dar. Die Eigenschaften der **Audio**-Ressource werden durch Extrahieren von Metadaten aus der Datei aufgefüllt. 

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.audio"
}-->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 1024,
  "composers": "string",
  "copyright": "string",
  "disc": 1024,
  "discCount": 1024,
  "duration": 1024,
  "genre": "string",
  "hasDrm": true,
  "isVariableBitrate": true,
  "title": "string",
  "track": 1024,
  "trackCount": 1024,
  "year": 1024
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ    | Beschreibung                                                          |
|:------------------|:--------|:---------------------------------------------------------------------|
| Album             | string  | Der Titel für das Album für diese Audiodatei.                          |
| albumArtist       | string  | Der auf dem Album für diese Audiodatei genannte Interpret.                    |
| Interpret            | string  | Der Interpret für die Audiodatei.                            |
| bitrate           | string  | In kbps ausgedrückte Bitrate.                                           |
| Komponisten         | string  | Der Name des Komponisten der Audiodatei.                          |
| Copyright         | string  | Copyright-Informationen für die Audiodatei.                            |
| disc              | number  | Die Anzahl der Datenträger, von denen diese Audiodatei stammt.                    |
| discCount         | number  | Die Gesamtzahl der Datenträger in diesem Album.                             |
| duration          | number  | Dauer der Audiodatei, ausgedrückt in Millisekunden                |
| Genre             | string  | Das Genre dieser Audiodatei                                        |
| hasDrm            | boolean | Zeigt an, ob die Datei durch digitale Rechteverwaltung geschützt ist.   |
| isVariableBitrate | boolean | Zeigt an, ob die Datei durch eine variable Bitrate verschlüsselt ist.            |
| title             | string  | Der Titel der Audiodatei.                                         |
| Track             | number  | Die Anzahl der Tracks auf der ursprünglichen CD für diese Audiodatei.    |
| trackCount        | number  | Die Gesamtanzahl der Tracks auf der ursprünglichen CD für diese Audiodatei. |
| Jahr              | number  | Das Jahr, in dem die Audiodatei aufgenommen wurden.                                |

## <a name="remarks"></a>Bemerkungen 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audio resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->