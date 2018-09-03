---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
ms.openlocfilehash: 60f2d58331f349f9990f78f36f04df055ce90b9e
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23269838"
---
# <a name="driveitem-resource-type"></a>DriveItem-Ressourcentyp

Die **driveItem**-Ressource stellt eine Datei, einen Ordner oder ein anderes auf einem Laufwerk gespeichertes Element dar. Alle Dateisystemobjekte in OneDrive und SharePoint werden als **driveItem**-Ressourcen zurückgegeben.

Es gibt zwei Hauptmethoden zum Adressieren einer **driveItem**-Ressource:

* Durch den eindeutigen **driveItem**-Bezeichner unter Verwendung von `drive/items/{item-id}`
* Durch den Dateisystempfad unter Verwendung von `/drive/root:/path/to/file`

**DriveItem**-Ressourcen verfügen über als Eigenschaften modellierte Facets, die Daten zu den driveItem-Identitäten und -Funktionen bereitstellen. Beispiel:

* Ordner haben ein [**„folder“-Facet**][-Ordner]
* Dateien haben eine [**„file“-Facet**][-Datei].
* Bilder haben zusätzlich zu ihrem „file“-Facet ein [**„image“Facet**][-Bild].
* Mit einer Kamera aufgenommene Bilder (Fotos) haben ein [**„photo“-Facet**][-Foto], das die Elemente als Foto identifiziert und als Eigenschaften das Aufnahmedatum sowie das zur Aufnahme verwendete Gerät aufführt.

Elemente mit dem **folder**-Facet fungieren als Elementcontainer und besitzen daher einen `children`-Verweis auf eine Sammlung von **driveItems** im jeweiligen Ordner.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **driveItem**-Ressource.

Die **driveItem**-Ressource wird von [**baseItem**][baseItem] abgeleitet und erbt Eigenschaften von dieser Ressource.

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
       "baseType": "microsoft.graph.baseItem",
       "optionalProperties": ["cTag", "children", "folder", "file", "image", "audio", "video",
       "location", "deleted", "specialFolder", "photo", "thumbnails", "searchResult", "remoteItem",
       "shared", "content", "@microsoft.graph.conflictBehavior", "@microsoft.graph.downloadUrl", "@content.sourceUrl",
       "sharepointIds"],
       "keyProperty": "id", "openType": true } -->

```json
{
  "audio": { "@odata.type": "microsoft.graph.audio" },
  "content": { "@odata.type": "Edm.Stream" },
  "cTag": "string (etag)",
  "deleted": { "@odata.type": "microsoft.graph.deleted"},
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "photo": { "@odata.type": "microsoft.graph.photo" },
  "publication": {"@odata.type": "microsoft.graph.publicationFacet"},
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
  "children": [{ "@odata.type": "microsoft.graph.driveItem" }],
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "microsoft.graph.driveItemVersion"}],

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

| Eigenschaft             | Typ               | Beschreibung
|:---------------------|:-------------------|:---------------------------------
| Audio                | [Audio][]          | Audiometadaten, wenn das Element eine Audiodatei ist. Schreibgeschützt.
| Inhalt              | Datenstrom             | Der Inhaltsdatenstrom, wenn das Element eine Datei ist
| createdBy            | [identitySet][]    | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.
| createdDateTime      | DateTimeOffset     | Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.
| cTag                 | Zeichenfolge             | Ein ETag für den Inhalt des Elements. Dieses ETag wird nicht geändert, wenn nur die Metadaten geändert werden. **Hinweis:** Diese Eigenschaft wird nicht zurückgegeben, wenn das Element ein Ordner ist. Schreibgeschützt.
| gelöscht              | [gelöscht][]        | Informationen zum „gelöscht“-Zustand des Elements. Schreibgeschützt.
| Beschreibung          | Zeichenfolge             | Stellt eine für den Benutzer sichtbare Beschreibung des Elements bereit. Lese-/Schreibzugriff. Nur auf OneDrive Personal
| eTag                 | Zeichenfolge             | ETag des gesamten Elements (Metadaten + Inhalt). Schreibgeschützt.
| Datei                 | [Datei][]           | Dateimetadaten, wenn das Element eine Datei ist. Schreibgeschützt.
| fileSystemInfo       | [fileSystemInfo][] | Informationen zum Dateisystem des Clients. Lese-/Schreibzugriff.
| Ordner               | [Ordner][]         | Ordnermetadaten, wenn das Element ein Ordner ist. Schreibgeschützt.
| id                   | Zeichenfolge             | Der eindeutige Bezeichner des Elements im Laufwerk. Schreibgeschützt.
| Abbildung                | [Bild][]          | Bildmetadaten, wenn das Element ein Bild ist. Schreibgeschützt.
| lastModifiedBy       | [identitySet][]    | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.
| lastModifiedDateTime | DateTimeOffset     | Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.
| Standort             | [geoCoordinates][] | Standortmetadaten, sofern das Element Standortdaten aufweist. Schreibgeschützt.
| Name                 | Zeichenfolge             | Der Name des Elements (Dateiname und Erweiterung). Lese-/Schreibzugriff.
| Paket              | [Paket][]        | Zeigt wenn vorhanden an, dass das Element ein Paket ist statt eines Ordners oder einer Datei. Pakete werden in einigen Kontexten wie Dateien, in anderen Kontexten wie Ordner behandelt. Schreibgeschützt.
| parentReference      | [itemReference][]  | Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.
| Foto                | [Foto][]          | Fotometadaten, wenn das Element ein Foto ist. Schreibgeschützt.
| Veröffentlichung          | [publicationFacet][] | Stellt Informationen über den veröffentlichten oder ausgecheckten Status eines Elements an Stellen bereit, die solche Aktionen unterstützen. Diese Eigenschaft wird standardmäßig nicht zurückgegeben. Schreibgeschützt. |
| remoteItem           | [remoteItem][]     | Daten zum Remoteelement, wenn das Element von einem anderen Laufwerk freigegeben ist als dem, auf das zugegriffen wird. Schreibgeschützt.
| Stamm                 | [Stamm][]           | Wenn diese Eigenschaft nicht Null ist, bedeutet dies, dass es sich bei der driveItem-Ressource um die oberste driveItem-Ressource auf dem Laufwerk handelt.
| searchResult         | [searchResult][]   | Suchmetadaten, wenn das Element aus einem Suchergebnis stammt. Schreibgeschützt.
| freigegeben               | [freigegeben][]         | Gibt an, dass das Element für andere freigegeben wurde, und enthält den „freigegeben“-Status des Elements. Schreibgeschützt.
| sharepointIds        | [sharepointIds][]  | Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.
| Größe                 | Int64              | Größe des Elements in Byte. Schreibgeschützt.
| specialFolder        | [specialFolder][]  | Facet, das zurückgegeben wird, wenn das aktuelle Element auch als spezieller Ordner verfügbar ist. Schreibgeschützt.
| Video                | [Video][]          | Videometadaten, wenn das Element ein Video ist. Schreibgeschützt.
| webDavUrl            | Zeichenfolge             | WebDAV-kompatible URL für das Element.
| webUrl               | Zeichenfolge             | URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.

**Hinweis:** Die Eigenschaften „eTag“ und „cTag“ arbeiten bei Containern (Ordnern) anders. Der Wert „cTag“ wird geändert, wenn Inhalte oder Metadaten eines Nachfolgers des Ordners geändert werden. Der Wert „eTag“ wird nur geändert, wenn die Eigenschaften des Ordners geändert werden. Ausnahme: Eigenschaften, die von Nachfolgern abgeleitet werden (wie **childCount** oder **lastModifiedDateTime**).

## <a name="relationships"></a>Beziehungen

| Beziehung       | Typ                        | Beschreibung
|:-------------------|:----------------------------|:--------------------------
| Untergeordnetes Element           | driveItem-Sammmlung        | Sammlung von Elementobjekten für die direkt untergeordneten Elemente eines Elements. Nur Elemente, die Ordner repräsentieren, haben untergeordnete Elemente. Schreibgeschützt. Lässt Nullwerte zu.
| createdByUser      | [Benutzer][]                    | Der Name des Benutzers, der das Element erstellt hat. Schreibgeschützt.
| lastModifiedByUser | [Benutzer][]                    | Der Name des Benutzers, der das Element zuletzt geändert hat. Schreibgeschützt.
| listItem           | [listItem][]                | Für Laufwerke in SharePoint, die zugeordneten Dokumentbibliothek-Listenelement. Schreibgeschützt. Lässt Nullwerte zu.
| Berechtigungen        | [Berechtigungen][] -Sammlung   | Der Satz von Berechtigungen für das Element. Schreibgeschützt. Lässt Nullwerte zu.
| Miniaturansichten         | [thumbnailSet][] -Sammlung | Sammlung der dem Element zugeordneten [ThumbnailSet][]-Objekte. Weitere Informationen finden Sie im Artikel zum [Abrufen von Miniaturansichten][]. Schreibgeschützt. Lässt Nullwerte zu.
| Versionen           | [DriveItemVersion][] -Auflistung | Die Liste der vorherigen Versionen des Listenelements. Weitere Informationen finden Sie unter [Abrufen von früheren Versionen][]. Schreibgeschützt. Lässt Nullwerte zu.
| Arbeitsmappe           | [Arbeitsmappe][]                | Für Dateien, die Excel-Kalkulationstabellen sind, greift auf die Arbeitsmappen-API zu, um mit dem Inhalt der Kalkulationstabelle zu arbeiten. Lässt Nullwerte zu.

## <a name="instance-attributes"></a>Instanzenattribute

Instanzenattribute sind Eigenschaften mit speziellem Verhalten. Diese Eigenschaften sind temporär. Sie definieren entweder, wie sich der Dienst verhalten soll, oder geben kurzfristige Eigenschaftswerte an, beispielsweise URLs zum Elementdownload, die ablaufen.

| Eigenschaftenname                     | Typ   | Beschreibung
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.conflictBehavior | Zeichenfolge | Das Konfliktlösungsverhalten von Aktionen, die ein neues Element erstellen. Verwenden Sie die Werte *fail*, *replace* oder *rename*. Das Standardformat für PUT ist *replace*. Ein Element wird nie mit dieser Anmerkung zurückgegeben. Schreibzugriff.
| @microsoft.graph.downloadUrl      | Zeichenfolge | Eine URL, über die die Inhalte der Datei heruntergeladen werden können. Eine Authentifizierung ist mit dieser URL nicht erforderlich. Schreibgeschützt.
| @microsoft.graph.sourceUrl        | Zeichenfolge | Bei Ausgabe einer PUT-Anforderung kann der Dienst mithilfe dieser Instanzanmerkung angewiesen werden, den Inhalt der URL herunterzuladen und als diese Datei zu speichern. Schreibzugriff.

**Hinweis:** Der Wert „@microsoft.graph.downloadUrl“ ist eine kurzlebige URL und kann nicht zwischengespeichert werden. Die URL ist nur für kurze Zeit (1 Stunde) verfügbar, bevor sie ungültig wird.

## <a name="methods"></a>Methoden

| Methode                                                   | REST-Pfad
|:---------------------------------------------------------|:------------------
| [Element abrufen](../api/driveitem_get.md)                      | `GET /drive/items/{item-id}`
| [Untergeordnete Objekte auflisten](../api/driveitem_list_children.md)       | `GET /drive/items/{item-id}/children`
| [Versionen auflisten](../api/driveitem_list_versions.md)       | `GET /drive/items/{item-id}/versions`
| [Element erstellen](../api/driveitem_post_children.md)         | `POST /drive/items/{item-id}/children`
| [Element aktualisieren](../api/driveitem_update.md)                | `PATCH /drive/items/{item-id}`
| [Inhalt aktualisieren](../api/driveitem_put_content.md)        | `PUT /drive/items/{item-id}/content`
| [Inhalte herunterladen](../api/driveitem_get_content.md)      | `GET /drive/items/{item-id}/content`
| [Bestimmtes Dateiformat herunterladen][download-format]         | `GET /drive/items/{item-id}/content?format={format}`
| [Element löschen](../api/driveitem_delete.md)                | `DELETE /drive/items/{item-id}`
| [Element verschieben](../api/driveitem_move.md)                    | `PATCH /drive/items/{item-id}`
| [Element kopieren](../api/driveitem_copy.md)                    | `POST /drive/items/{item-id}/copy`
| [Elemente durchsuchen](../api/driveitem_search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [Liste der Änderungen auf einem Laufwerk](../api/driveitem_delta.md)     | `GET /drive/root/delta`
| [Liste Miniaturansichten](../api/driveitem_list_thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [Freigabelink erstellen](../api/driveitem_createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [Berechtigungen hinzufügen](../api/driveitem_invite.md)            | `POST /drive/items/{item-id}/invite`
| [Berechtigungen auflisten](../api/driveitem_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [Berechtigung löschen](../api/permission_delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`


## <a name="remarks"></a>Bemerkungen

In OneDrive for Business- oder SharePoint-Dokumentbibliotheken wird die Eigenschaft **cTag** nicht zurückgegeben, wenn die **driveItem**-Ressource ein [Ordner][]-Facet hat.

[Audio]: audio.md
[baseItem]: baseItem.md
[gelöscht]: deleted.md
[download-format]: ../api/driveitem_get_content_format.md
[driveItemVersion]: driveItemVersion.md
[Datei]: file.md
[fileSystemInfo]: fileSystemInfo.md
[Ordner]: folder.md
[Abrufen von früheren Versionen]: ../api/driveitem_list_versions.md
[Abrufen von Miniaturansichten]: ../api/driveitem_list_thumbnails.md
[identitySet]: identitySet.md
[Bild]: image.md
[itemReference]: itemReference.md
[geoCoordinates]: geoCoordinates.md
[listItem]: listItem.md
[Paket]: package.md
[Paket]: permission.md
[Foto]: photo.md
[remoteItem]: remoteItem.md
[Stamm]: root.md
[searchResult]: searchResult.md
[shared]: shared.md
[sharepointIds]: sharepointIds.md
[specialFolder]: specialFolder.md
[thumbnailSet]: thumbnailSet.md
[Video]: video.md
[Arbeitsmappe]: workbook.md
[Benutzer]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
