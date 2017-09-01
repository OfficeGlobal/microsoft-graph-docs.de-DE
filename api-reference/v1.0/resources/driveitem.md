# <a name="driveitem-resource-type"></a>Ressourcentyp „DriveItem“

Die **driveItem**-Ressource stellt eine Datei, einen Ordner oder ein anderes auf einem Laufwerk gespeichertes Element dar. Alle Dateisystemobjekte in OneDrive und SharePoint werden als **driveItem**-Ressourcen zurückgegeben.

Es gibt zwei Hauptmethoden zum Adressieren einer **driveItem**-Ressource:

* Durch den eindeutigen **driveItem**-Bezeichner unter Verwendung von `drive/items/{item-id}`
* Durch den Dateisystempfad unter Verwendung von `/drive/root:/path/to/file`

**DriveItem**-Ressourcen verfügen über als Eigenschaften modellierte Facets, die Daten zu den driveItem-Identitäten und -Funktionen bereitstellen. Beispiel:

* Ordner haben ein [ **„folder“-Facet**](folder.md)
* Dateien haben ein [ **„file“-Facet**](file.md)
* Bilder haben zusätzlich zu ihrem „file“-Facet ein [**„image“-Facet**](image.md).
* Mit einer Kamera aufgenommene Bilder (Fotos) haben ein [**„photo“-Facet**](photo.md), das die Elemente als Foto identifiziert und als Eigenschaften das Aufnahmedatum sowie das zur Aufnahme verwendete Gerät aufführt.

Elemente mit dem **folder**-Facet fungieren als Elementcontainer und besitzen daher einen `children`-Verweis auf eine Sammlung von **driveItems** im jeweiligen Ordner.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **driveItem**-Ressource.

Die **driveItem**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "children", "createdByUser", "lastModifiedByUser", "permissions", "thumbnails"],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.driveItem"
}-->

```json
{
  "audio": { "@odata.type": "microsoft.graph.audio" },
  "cTag": "string",
  "deleted": { "@odata.type": "microsoft.graph.deleted" },
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "photo": { "@odata.type": "microsoft.graph.photo" },
  "remoteItem": { "@odata.type": "microsoft.graph.remoteItem" },
  "root": { "@odata.type": "microsoft.graph.root" },
  "searchResult": { "@odata.type": "microsoft.graph.searchResult" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "video": { "@odata.type": "microsoft.graph.video" },
  "webDavUrl": "string",

  /* relationships */
  "content": { "@odata.type": "Edm.Stream" },
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "children": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],

  /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "eTag": "string",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": {"@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "string",

  /* instance annotations */
  "@microsoft.graph.conflictBehavior": "string",
  "@microsoft.graph.downloadUrl": "url",
  "@microsoft.graph.sourceUrl": "url"
}

```

## <a name="properties"></a>Eigenschaften

| Eigenschaft             | Typ                                | Beschreibung                                                                                                                                                               |
| :------------------- | :---------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| audio                | [audio](audio.md)                   | Audiometadaten, wenn das Element eine Audiodatei ist. Schreibgeschützt.                                                                                                                  |
| createdBy            | [identitySet](identityset.md)       | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.                                                                                          |
| createdDateTime      | DateTimeOffset                      | Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.                                                                                                                                |
| cTag                 | String                              | Ein ETag für den Inhalt des Elements. Dieses ETag wird nicht geändert, wenn nur die Metadaten geändert werden. **Hinweis:** Diese Eigenschaft wird nicht zurückgegeben, wenn das Element ein Ordner ist. Schreibgeschützt. |
| gelöscht              | [deleted](deleted.md)               | Informationen zum „gelöscht“-Zustand des Elements. Schreibgeschützt.                                                                                                               |
| description          | Zeichenfolge                              | Stellt eine für den Benutzer sichtbare Beschreibung des Elements bereit. Lese-/Schreibzugriff. Nur auf OneDrive Personal                                                                                    |
| eTag                 | String                              | ETag des gesamten Elements (Metadaten + Inhalt). Schreibgeschützt.                                                                                                                 |
| file                 | [file](file.md)                     | Dateimetadaten, wenn das Element eine Datei ist. Schreibgeschützt.                                                                                                                          |
| fileSystemInfo       | [fileSystemInfo](filesysteminfo.md) | Informationen zum Dateisystem des Clients. Lese-/Schreibzugriff.                                                                                                                            |
| folder               | [folder](folder.md)                 | Ordnermetadaten, wenn das Element ein Ordner ist. Schreibgeschützt.                                                                                                                      |
| id                   | String                              | Der eindeutige Bezeichner des Elements im Laufwerk. Schreibgeschützt.                                                                                                            |
| Abbildung                | [image](image.md)                   | Bildmetadaten, wenn das Element ein Bild ist. Schreibgeschützt.                                                                                                                       |
| lastModifiedBy       | [identitySet](identityset.md)       | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.                                                                                    |
| lastModifiedDateTime | DateTimeOffset                      | Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.                                                                                                                      |
| location             | [geoCoordinates](geoCoordinates.md) | Standortmetadaten, sofern das Element Standortdaten aufweist. Schreibgeschützt.                                                                                                              |
| name                 | String                              | Der Name des Elements (Dateiname und Erweiterung). Lese-/Schreibzugriff.                                                                                                                |
| package              | [package](package.md)               | Zeigt wenn vorhanden an, dass das Element ein Paket ist statt eines Ordners oder einer Datei. Pakete werden in einigen Kontexten wie Dateien, in anderen Kontexten wie Ordner behandelt. Schreibgeschützt.         |
| parentReference      | [itemReference](itemreference.md)   | Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.                                                                                                                 |
| Foto                | [photo](photo.md)                   | Fotometadaten, wenn das Element ein Foto ist. Schreibgeschützt.                                                                                                                        |
| remoteItem           | [remoteItem](remoteitem.md)         | Daten zum Remoteelement, wenn das Element von einem anderen Laufwerk freigegeben ist als dem, auf das zugegriffen wird. Schreibgeschützt.                                                                        |
| root                 | [root](root.md)                     | Wenn diese Eigenschaft nicht Null ist, bedeutet dies, dass es sich bei der driveItem-Ressource um die oberste driveItem-Ressource auf dem Laufwerk handelt.                                                                     |
| searchResult         | [searchResult](searchresult.md)     | Suchmetadaten, wenn das Element aus einem Suchergebnis stammt. Schreibgeschützt.                                                                                                          |
| shared               | [shared](shared.md)                 | Gibt an, dass das Element für andere freigegeben wurde, und enthält den „freigegeben“-Status des Elements. Schreibgeschützt.                                               |
| sharepointIds        | [sharepointIds](sharepointids.md)   | Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.                                                                                                  |
| size                 | Int64                               | Größe des Elements in Byte. Schreibgeschützt.                                                                                                                                     |
| specialFolder        | [specialFolder](specialfolder.md)   | Facet, das zurückgegeben wird, wenn das aktuelle Element auch als spezieller Ordner verfügbar ist. Schreibgeschützt.                                                                             |
| video                | [video](video.md)                   | Videometadaten, wenn das Element ein Video ist. Schreibgeschützt.                                                                                                                        |
| webDavUrl            | String                              | WebDAV-kompatible URL für das Element.                                                                                                                                       |
| webUrl               | String                              | URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.                                                                                                                 |

**Hinweis:** Die Eigenschaften „eTag“ und „cTag“ arbeiten bei Containern (Ordnern) anders. Der Wert „cTag“ wird geändert, wenn Inhalte oder Metadaten eines Nachfolgers des Ordners geändert werden. Der Wert „eTag“ wird nur geändert, wenn die Eigenschaften des Ordners geändert werden. Ausnahme: Eigenschaften, die von Nachfolgern abgeleitet werden (wie **childCount** oder **lastModifiedDateTime**).

## <a name="relationships"></a>Beziehungen

| Beziehung       | Typ                                       | Beschreibung                                                                                                                                                                       |
| :----------------- | :----------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Inhalt            | Stream                                     | Der Inhaltsdatenstrom, wenn das Element eine Datei darstellt.                                                                                                                                |
| children           | [driveitem](driveitem.md) collection       | Sammlung von Elementobjekten der direkten untergeordneten Elemente eines Elements. Nur Elemente, die Ordner repräsentieren, haben untergeordnete Elemente. Schreibgeschützt. Lässt Nullwerte zu.                                        |
| createdByUser      | [user](user.md)                            | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.                                                                                                  |
| lastModifiedByUser | [user](user.md)                            | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.                                                                                            |
| permissions        | [permission](permission.md) collection     | Der Satz von Berechtigungen für das Element. Schreibgeschützt. Lässt Nullwerte zu.                                                                                                                         |
| thumbnails         | [thumbnailSet](thumbnailset.md) collection | Sammlung der dem Element zugeordneten [ThumbnailSet](thumbnailSet.md)-Objekte. Weitere Informationen finden Sie im Artikel zum [Abrufen von Miniaturansichten](../api/thumbnailset_get.md). Schreibgeschützt. Lässt Nullwerte zu. |

## <a name="instance-attributes"></a>Instanzenattribute

Instanzenattribute sind Eigenschaften mit speziellem Verhalten. Diese Eigenschaften sind temporär. Sie definieren entweder, wie sich der Dienst verhalten soll, oder geben kurzfristige Eigenschaftswerte an, beispielsweise URLs zum Elementdownload, die ablaufen.

| Eigenschaftenname                     | Typ   | Beschreibung                                                                                                                                                         |
|:----------------------------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| @microsoft.graph.conflictBehavior | string | Das Konfliktlösungsverhalten von Aktionen, die ein neues Element erstellen. Verwenden Sie die Werte *fail*, *replace* oder *rename*. Das Standardformat für PUT ist *replace*. Ein Element wird nie mit dieser Anmerkung zurückgegeben. Schreibzugriff.                               |
| @microsoft.graph.downloadUrl      | string | Eine URL, über die die Inhalte der Datei heruntergeladen werden können. Eine Authentifizierung ist mit dieser URL nicht erforderlich. Schreibgeschützt.                                                    |
| @microsoft.graph.sourceUrl        | string | Bei Ausgabe einer PUT-Anforderung kann der Dienst mithilfe dieser Instanzanmerkung angewiesen werden, den Inhalt der URL herunterzuladen und als diese Datei zu speichern. Schreibzugriff. |

**Hinweis:** Der Wert „@microsoft.graph.downloadUrl“ ist eine kurzlebige URL und kann nicht zwischengespeichert werden. Die URL ist nur für kurze Zeit (1 Stunde) verfügbar, bevor sie ungültig wird.


## <a name="methods"></a>Methoden

| Method                                                 | REST-Pfad
|:-------------------------------------------------------|:--------------------
| [Get item](../api/item_get.md)                         | `GET /drive/items/{item-id}`
| [List children](../api/item_list_children.md)          | `GET /drive/items/{item-id}/children`
| [Create item](../api/item_post_children.md)            | `POST /drive/items/{item-id}/children`
| [Update item](../api/item_update.md)                   | `PATCH /drive/items/{item-id}`
| [Upload content](../api/item_uploadcontent.md)         | `PUT /drive/items/{item-id}/content`
| [Download content](../api/item_downloadcontent.md)     | `GET /drive/items/{item-id}/content`
| [Delete item](../api/item_delete.md)                   | `DELETE /drive/items/{item-id}`
| [Move item](../api/item_move.md)                       | `PATCH /drive/items/{item-id}`
| [Copy item](../api/item_copy.md)                       | `POST /drive/items/{item-id}/copy`
| [Search items](../api/item_search.md)                  | `GET /drive/items/{item-id}/search(q='text')`
| [List changes in a drive](../api/item_delta.md)        | `GET /drive/root/delta`
| [List thumbnails](../api/item_list_thumbnails.md)      | `GET /drive/items/{item-id}/thumbnails`  |
| [Create sharing link](../api/item_createlink.md)       | `POST /drive/items/{item-id}/createLink` |
| [Add permissions](../api/item_invite.md)               | `POST /drive/items/{item-id}/invite`     |
| [List permissions](../api/item_list_permissions.md)    | `GET /drive/items/{item-id}/permissions` |
| [Delete permission](../api/permission_delete.md)       | `DELETE /drive/items/{item-id}/permissions/{perm-id}` |

## <a name="remarks"></a>Bemerkungen

In OneDrive for Business- oder SharePoint-Dokumentbibliotheken wird die Eigenschaft **cTag** nicht zurückgegeben, wenn die **driveItem**-Ressource ein [folder](folder.md)-Facet hat.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
