# <a name="thumbnail-resource-type"></a>thumbnail-Ressourcentyp

Der **thumbnail**-Ressourcentyp stellt eine Miniaturansicht für ein Bild, ein Video, ein Dokument oder eine beliebige Datei oder einen Ordner auf OneDrive dar, der über eine grafische Darstellung verfügt.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ   | Beschreibung                                  |
|:---------|:-------|:---------------------------------------------|
| height   | Int32  | Die Höhe der Miniaturansicht in Pixel.      |
| url      | String | Die URL, die zum Abrufen der Miniaturansichtsinhalte verwendet wird. |
| width    | Int32  | Die Breite der Miniaturansicht in Pixel.       |


## <a name="relationships"></a>Beziehungen

| Name    | Typ   | Beschreibung         |
|:--------|:-------|:--------------------|
| Inhalt | Stream | Der Inhaltsstream. |


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "url": "string",
  "height": 1024,
  "width": 1024,
  "content": "stream"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
