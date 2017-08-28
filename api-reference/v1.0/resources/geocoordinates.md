# <a name="geocoordinates-resource-type"></a>GeoCoordinates-Ressourcentyp

Die **GeoCoordinates**-Ressource liefert geografische Koordinaten und die Erhebung eines Orts basierend auf Metadaten, die in der Datei enthalten sind. Wenn ein [**DriveItem**](driveitem.md) ein **location**-Facet ungleich Null aufweist, stellt das Element eine Datei dar, die mit einem bekannten Ort verknüpft ist.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft  | Typ   | Beschreibung                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| altitude  | Gleitkommawert mit doppelter Genauigkeit | Optional. Die Höhe oberhalb des Meeresspiegels in Fuß. Schreibgeschützt. |
| latitude  | Gleitkommawert mit doppelter Genauigkeit | Optional. Der Breitengrad für das Element als Kommazahl. Schreibgeschützt.   |
| longitude | Gleitkommawert mit doppelter Genauigkeit | Optional. Der Längengrad für das Element als Kommazahl. Schreibgeschützt.  |

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "geoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
