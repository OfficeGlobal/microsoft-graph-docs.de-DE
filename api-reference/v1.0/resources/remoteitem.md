# <a name="remoteitem-resource-type"></a>RemoteItem-Ressourcentyp

Der **RemoteItem**-Ressourcentyp gibt an, dass ein [DriveItem](driveitem.md)-Element auf ein Element in einem anderen Laufwerk verweist. Diese Ressource stellt die eindeutigen IDs des Quelllaufwerks und des Zielelements bereit.

[**DriveItems**](driveitem.md) mit einem **remoteItem**-Facet ungleich Null sind Ressourcen, die freigegeben, zu OneDrive-Umgebungen von Benutzern hinzugefügt oder für Elemente von heterogenen Elementsammlungen (wie z. B. Suchergebnisse) zurückgegeben wurden. 

**Hinweis:** Im Gegensatz zu Ordnern im gleichen Laufwerk wird beim Verschieben eines DriveItem-Elements in ein Remote-Element möglicherweise der `id`-Wert geändert.
## <a name="json-representation"></a>JSON-Darstellung

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.remoteItem", optionalProperties: ["name", "fileSystemInfo", "file", "folder"] } -->
```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname        | Typ                                          | Beschreibung                                                              |
|:---------------------|:----------------------------------------------|:-------------------------------------------------------------------------|
| createdBy            | [IdentitySet](identityset.md)                 | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.   |
| createdDateTime      | Timestamp                                     | Datum und Uhrzeit der Elementerstellung. Schreibgeschützt. |
| file                 | [Datei](file.md)                               | Gibt an, dass das Remote-Element eine Datei ist. Schreibgeschützt.                     |
| fileSystemInfo       | [FileSystemInfo](filesysteminfo.md)           | Informationen über das Remote-Element aus dem lokalen Dateisystem. Schreibgeschützt. |
| folder               | [Ordner](folder.md)                           | Gibt an, dass das Remote-Element ein Ordner ist. Schreibgeschützt.                   |
| id                   | String                                        | Eindeutige ID für das Remote-Element in dem Laufwerk. Schreibgeschützt.           |
| lastModifiedBy       | [IdentitySet](identityset.md)                 | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt. |
| lastModifiedDateTime | Timestamp                                     | Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.  | 
| name                 | String                                        | Optional. Dateiname des Remote-Elements. Schreibgeschützt.                        |
| package              | [Paket](package.md)                         | Zeigt wenn vorhanden an, dass das Element ein Paket ist statt eines Ordners oder einer Datei. Pakete werden in einigen Kontexten wie Dateien, in anderen Kontexten wie Ordner behandelt. Schreibgeschützt. |
| parentReference      | [ItemReference](itemreference.md)             | Eigenschaften des übergeordneten Elements des Remote-Elements. Schreibgeschützt.                  |
| sharepointIds        | [SharepointIds](sharepointids.md)             | Bietet Interoperabilität zwischen Elementen in OneDrive for Business und SharePoint mit vollständigem Satz an Element-IDs. Schreibgeschützt.  |
| size                 | Int64                                         | Größe des Remote-Elements. Schreibgeschützt.                                      |
| specialFolder        | [SpecialFolder](specialfolder.md)             | Facet, das zurückgegeben wird, wenn das aktuelle Element auch als spezieller Ordner verfügbar ist. Schreibgeschützt. |
| webDavUrl            | Url                                           | DAV-kompatible URL für das Element.  |
| webUrl               | Url                                           | URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt. | 

## <a name="remarks"></a>Bemerkungen 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "remoteItem resource type provides a link to an item in another drive.",
  "keywords": "remoteitem symlink remote drive shared with me add to onedrive",
  "section": "documentation"
} -->