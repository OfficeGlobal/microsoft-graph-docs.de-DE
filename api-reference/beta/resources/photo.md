# <a name="photo-resource-type"></a>Photo-Ressourcentyp

Die **photo**-Ressource stellt Foto- und Kameraeigenschaften auf einem [DriveItem](driveitem.md) bereit, z. B. EXIF-Metadaten.

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1024,
  "exposureNumerator": 1024,
  "fNumber": 1024,
  "focalLength": 1024,
  "iso": 1024,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>Eigenschaften
| Eigenschaft                | Typ                      | Beschreibung                                                     |
|:------------------------|:--------------------------|:----------------------------------------------------------------|
| **takenDateTime**       | DateTimeOffset            | Stellt das Datum und die Uhrzeit für die Aufnahme des Fotos dar. Schreibgeschützt.               |
| **cameraMake**          | String                    | Kamerahersteller Schreibgeschützt.                                            |
| **cameraModel**         | String                    | Kameramodell. Schreibgeschützt.                                                   |
| **fNumber**             | Gleitkommawert mit doppelter Genauigkeit                    | Die Blendenzahl der Kamera. Schreibgeschützt.                               |
| **exposureDenominator** | Int32                     | Der Nenner der Bruchzahl für die Belichtungszeit der Kamera. Schreibgeschützt. |
| **exposureNumerator**   | Int32                     | Der Zähler der Bruchzahl für die Belichtungszeit der Kamera. Schreibgeschützt.   |
| **focalLength**         | Gleitkommawert mit doppelter Genauigkeit                    | Die Brennweite der Kamera. Schreibgeschützt.                               |
| **iso**                 | Int32                     | Der ISO-Wert der Kamera. Schreibgeschützt.                                  |


## <a name="remarks"></a>Bemerkungen
Von OneDrive for Business und SharePoint wird nur die **TakenDateTime**-Eigenschaft zurückgegeben.

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "photo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
