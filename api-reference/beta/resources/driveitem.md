---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7ac95379d8e5eeae07e520f40ae9403c47e98f58
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789641"
---
# <a name="driveitem-resource-type"></a>driveItem-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "children": [{ "@odata.type": "microsoft.graph.driveItem" }],
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "subscriptions": [ {"@odata.type": "microsoft.graph.subscription"} ],
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
| audio                | [audio][]          | Audiometadaten, wenn das Element eine Audiodatei ist. Schreibgeschützt.
| content              | Stream             | Der Inhaltsdatenstrom, wenn das Element eine Datei ist
| createdBy            | [identitySet][]    | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.
| createdDateTime      | DateTimeOffset     | Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.
| cTag                 | String             | Ein ETag für den Inhalt des Elements. Dieses ETag wird nicht geändert, wenn nur die Metadaten geändert werden. **Hinweis:** Diese Eigenschaft wird nicht zurückgegeben, wenn das Element ein Ordner ist. Schreibgeschützt.
| gelöscht              | [deleted][]        | Informationen zum „gelöscht“-Zustand des Elements. Schreibgeschützt.
| description          | Zeichenfolge             | Stellt eine für den Benutzer sichtbare Beschreibung des Elements bereit. Lese-/Schreibzugriff. Nur auf OneDrive Personal
| eTag                 | String             | ETag des gesamten Elements (Metadaten + Inhalt). Schreibgeschützt.
| file                 | [file][]           | Dateimetadaten, wenn das Element eine Datei ist. Schreibgeschützt.
| fileSystemInfo       | [fileSystemInfo][] | Informationen zum Dateisystem des Clients. Lese-/Schreibzugriff.
| folder               | [Ordner][]         | Ordnermetadaten, wenn das Element ein Ordner ist. Schreibgeschützt.
| id                   | String             | Der eindeutige Bezeichner des Elements im Laufwerk. Schreibgeschützt.
| Abbildung                | [image][]          | Bildmetadaten, wenn das Element ein Bild ist. Schreibgeschützt.
| lastModifiedBy       | [identitySet][]    | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.
| lastModifiedDateTime | DateTimeOffset     | Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.
| location             | [geoCoordinates][] | Standortmetadaten, sofern das Element Standortdaten aufweist. Schreibgeschützt.
| name                 | String             | Der Name des Elements (Dateiname und Erweiterung). Lese-/Schreibzugriff.
| package              | [package][]        | Zeigt wenn vorhanden an, dass das Element ein Paket ist statt eines Ordners oder einer Datei. Pakete werden in einigen Kontexten wie Dateien, in anderen Kontexten wie Ordner behandelt. Schreibgeschützt.
| parentReference      | [itemReference][]  | Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.
| Foto                | [photo][]          | Fotometadaten, wenn das Element ein Foto ist. Schreibgeschützt.
| Veröffentlichung          | [publicationFacet][] | Stellt Informationen über den veröffentlichten oder ausgecheckten Status eines Elements an Stellen bereit, die solche Aktionen unterstützen. Diese Eigenschaft wird standardmäßig nicht zurückgegeben. Schreibgeschützt. |
| remoteItem           | [remoteItem][]     | Daten zum Remoteelement, wenn das Element von einem anderen Laufwerk freigegeben ist als dem, auf das zugegriffen wird. Schreibgeschützt.
| root                 | [root][]           | Wenn diese Eigenschaft nicht Null ist, bedeutet dies, dass es sich bei der driveItem-Ressource um die oberste driveItem-Ressource auf dem Laufwerk handelt.
| searchResult         | [searchResult][]   | Suchmetadaten, wenn das Element aus einem Suchergebnis stammt. Schreibgeschützt.
| freigegeben               | [shared][]         | Gibt an, dass das Element für andere freigegeben wurde, und enthält den „freigegeben“-Status des Elements. Schreibgeschützt.
| sharepointIds        | [sharepointIds][]  | Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.
| size                 | Int64              | Größe des Elements in Byte. Schreibgeschützt.
| specialFolder        | [specialFolder][]  | Facet, das zurückgegeben wird, wenn das aktuelle Element auch als spezieller Ordner verfügbar ist. Schreibgeschützt.
| video                | [video][]          | Videometadaten, wenn das Element ein Video ist. Schreibgeschützt.
| webDavUrl            | String             | WebDAV-kompatible URL für das Element.
| webUrl               | String             | URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.

**Hinweis:** Die Eigenschaften „eTag“ und „cTag“ arbeiten bei Containern (Ordnern) anders. Der Wert „cTag“ wird geändert, wenn Inhalte oder Metadaten eines Nachfolgers des Ordners geändert werden. Der Wert „eTag“ wird nur geändert, wenn die Eigenschaften des Ordners geändert werden. Ausnahme: Eigenschaften, die von Nachfolgern abgeleitet werden (wie **childCount** oder **lastModifiedDateTime**).

## <a name="relationships"></a>Beziehungen

| Beziehung       | Typ                        | Beschreibung
|:-------------------|:----------------------------|:--------------------------
| Aktivitäten         | [itemActivity][]-Sammlung | Die Liste der letzten Aktivitäten, die für dieses Element durchgeführt wurden.
| analytics          | [itemAnalytics][]-Ressource  | Analysen zu den Ansichts Aktivitäten, die für dieses Element durchgeführt wurden.
| children           | driveitem-Sammlung        | Sammlung von Elementobjekten der direkten untergeordneten Elemente eines Elements. Nur Elemente, die Ordner repräsentieren, haben untergeordnete Elemente. Schreibgeschützt. Nullwerte zulassend.
| createdByUser      | [user][]                    | Der Name des Benutzers, der das Element erstellt hat. Schreibgeschützt.
| lastModifiedByUser | [user][]                    | Der Name des Benutzers, der das Element zuletzt geändert hat. Schreibgeschützt.
| listItem           | [listItem][]                | Für Laufwerke in SharePoint das zugehörige Dokumentbibliothek-Listenelement. Schreibgeschützt. Lässt Nullwerte zu.
| Berechtigungen        | [permission][] collection   | Der Satz von Berechtigungen für das Element. Schreibgeschützt. Lässt Nullwerte zu.
| Abonnements      | [Abonnement][] Sammlung | Die Gruppe von Abonnements für das Element. Wird nur im Stammverzeichnis eines Laufwerks unterstützt.
| thumbnails         | [thumbnailSet][] collection | Sammlung der dem Element zugeordneten [ThumbnailSet][]-Objekte. Weitere Informationen finden Sie im Artikel zum [Abrufen von Miniaturansichten][]. Schreibgeschützt. Nullwerte zulassend.
| versions           | [driveItemVersion][]-Sammlung | Die Liste der früheren Versionen des Elements. Weitere Informationen finden Sie unter [Abrufen früherer Versionen][]. Schreibgeschützt. Lässt Nullwerte zu.
| workbook           | [workbook][]                | Greift für Dateien, die Excel-Tabellen sind, auf die Workbook-API zu, um mit dem Inhalt der Tabelle zu arbeiten. Nullwerte zulassend.

## <a name="instance-attributes"></a>Instanzenattribute

Instanzenattribute sind Eigenschaften mit speziellem Verhalten. Diese Eigenschaften sind temporär. Sie definieren entweder, wie sich der Dienst verhalten soll, oder geben kurzfristige Eigenschaftswerte an, beispielsweise URLs zum Elementdownload, die ablaufen.

| Eigenschaftenname                     | Typ   | Beschreibung
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.conflictBehavior | Zeichenfolge | Das Konfliktlösungsverhalten von Aktionen, die ein neues Element erstellen. Verwenden Sie die Werte *fail*, *replace* oder *rename*. Das Standardformat für PUT ist *replace*. Ein Element wird nie mit dieser Anmerkung zurückgegeben. Schreibzugriff.
| @microsoft.graph.downloadUrl      | string | Eine URL, über die die Inhalte der Datei heruntergeladen werden können. Eine Authentifizierung ist mit dieser URL nicht erforderlich. Schreibgeschützt.
| @microsoft.graph.sourceUrl        | string | Bei Ausgabe einer PUT-Anforderung kann der Dienst mithilfe dieser Instanzanmerkung angewiesen werden, den Inhalt der URL herunterzuladen und als diese Datei zu speichern. Schreibzugriff.

**Hinweis:** Der Wert „@microsoft.graph.downloadUrl“ ist eine kurzlebige URL und kann nicht zwischengespeichert werden.
Die URL ist nur für kurze Zeit (1 Stunde) verfügbar, bevor sie ungültig wird.
Durch das Entfernen von Dateiberechtigungen für einen Benutzer wird die URL möglicherweise nicht sofort ungültig.

## <a name="methods"></a>Methoden

| Method                                                   | REST-Pfad
|:---------------------------------------------------------|:------------------
| [Get item](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [Aktivitäten auflisten](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| [Analysen abrufen][]                                        | `GET /drive/items/{item-id}/analytics`
| [Aktivitäten nach Intervall abrufen][]                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [Untergeordnete Elemente auflisten](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [Versionen auflisten](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [Element erstellen](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [Update item](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [Upload content](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [Inhalte herunterladen](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| [Bestimmtes Dateiformat herunterladen][download-format]         | `GET /drive/items/{item-id}/content?format={format}`
| [Element löschen](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [Move item](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [Copy item](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [Search items](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [List changes in a drive](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [List thumbnails](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [Create sharing link](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [Add permissions](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [List permissions](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [Berechtigung löschen](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| [WebSocket-Kanal abrufen][getWebSocket]                    | `GET /drive/root/subscriptions/socketIo`
| [Element in Vorschau anzeigen][item-preview]                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[Analysen abrufen]: ../api/itemanalytics-get.md
[Aktivitäten nach Intervall abrufen]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a>Hinweise

In OneDrive for Business- oder SharePoint-Dokumentbibliotheken wird die Eigenschaft **cTag** nicht zurückgegeben, wenn die **driveItem**-Ressource ein [Ordner][]-Facet hat.

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[Abrufen früherer Versionen]: ../api/driveitem-list-versions.md
[Abrufen von Miniaturansichten]: ../api/driveitem-list-thumbnails.md
[getWebSocket]: ../api/driveitem-subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[List activities]: ../api/activities-list.md
[listItem]: listitem.md
[package]: package.md
[permission]: permission.md
[photo]: photo.md
[remoteItem]: remoteitem.md
[root]: root.md
[searchResult]: searchresult.md
[shared]: shared.md
[sharepointIds]: sharepointids.md
[specialFolder]: specialfolder.md
[Abonnement]: subscription.md
[thumbnailSet]: thumbnailset.md
[video]: video.md
[workbook]: workbook.md
[user]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": {
    "Resources/Item": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/driveitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
