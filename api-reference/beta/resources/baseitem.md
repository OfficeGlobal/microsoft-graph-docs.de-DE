# <a name="baseitem-resource-type"></a>baseItem-Ressourcentyp

Die **baseItem**-Ressource ist eine abstrakte Ressource, die einen gemeinsamen Satz von Eigenschaften enthält, die auch von mehreren anderen Ressourcen verwendet werden. Folgende Ressourcen werden u. a. von abgeleitet **baseItem** abgeleitet:

* [drive](drive.md)
* [driveItem](driveitem.md)
* [site](site.md)
* [sharedDriveItem](shareddriveitem.md)

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **baseItem**-Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseItem"
}-->

```json
{
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft             | Typ              | Beschreibung                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| id                   | string            | Der eindeutige Bezeichner des Laufwerks. Schreibgeschützt.                                         |
| createdBy            | [identitySet][]   | Die Identität des Benutzers, des Geräts oder der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.        |
| createdDateTime      | dateTimeOffset    | Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.                                             |
| eTag                 | string            | ETag für das Element. Schreibgeschützt.                                                          |
| lastModifiedBy       | [identitySet][]   | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt. |
| lastModifiedDateTime | dateTimeOffset    | Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.                                   |
| name                 | string            | Der Name des Elements. Lese-/Schreibzugriff.                                                      |
| parentReference      | [itemReference][] | Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.                              |
| webUrl               | string (URL)      | URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.                              |

[identitySet]: identitySet.md
[itemReference]: itemreference.md

## <a name="remarks"></a>Bemerkungen

Der Typ `baseItem` wird voraussichtlich nicht direkt verwendet.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/baseItem",
  "tocBookmarks": {
    "Site": "#"
  }
} -->
