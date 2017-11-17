# <a name="file-resource-type"></a>File-Ressourcentyp

Die **File**-Ressource gruppiert dateibezogene Datenelemente in einer einzelnen Struktur.

Wenn ein [**DriveItem**](driveitem.md) ein **file**-Facet ungleich Null aufweist, stellt das Element eine Datei dar. Neben anderen Eigenschaften weisen Dateien eine **content**-Beziehung auf, die den Bytedatenstrom der Datei enthält.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.file"
}-->

```json
{
  "hashes": {"@odata.type": "microsoft.graph.hashes"},
  "mimeType": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ                    | Beschreibung                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| hashes   | [HashesType](hashes.md) | Hashes des binären Inhalts der Datei, wenn verfügbar. Schreibgeschützt.                                                                                    |
| mimeType | string                  | Der MIME-Typ für die Datei. Dieser wird von der Logik auf dem Server bestimmt und stimmt möglicherweise nicht mit dem Wert überein, der bereitgestellt wurde, als die Datei hochgeladen wurde. Schreibgeschützt. |

## <a name="remarks"></a>Bemerkungen 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "file resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
