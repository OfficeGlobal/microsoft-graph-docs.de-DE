# <a name="image-resource-type"></a>Image-Ressourcentyp

Die **Image**-Ressourc gruppiert bildbezogene Eigenschaften in einer einzelnen Struktur. Wenn ein [**DriveItem**](driveitem.md) ein **image**-Facet ungleich Null aufweist, stellt das Element eine Bitmapdatei dar.

**Hinweis:** Wenn der Dienst die Breite und Höhe des Bilds nicht bestimmen kann, ist die **Image**-Ressource möglicherweise leer.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.image"
}-->

```json
{
  "height": 1024,
  "width": 1024
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ  | Beschreibung                                |
|:-----------|:------|:-------------------------------------------|
| **height** | Int32 | Optional. Die Höhe des Bilds in Pixel. Schreibgeschützt. |
| **width**  | Int32 | Optional. Die Breite des Bilds in Pixel. Schreibgeschützt.  |


## <a name="remarks"></a>Bemerkungen

In OneDrive for Business wird diese Ressource für Elemente zurückgegeben, von denen basierend auf der Dateierweiterung davon ausgegangen wird, dass es sich um Bilder handelt. Diese Ressource gibt keine Eigenschaften in OneDrive for Business zurück.

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "image resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
