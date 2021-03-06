---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
ms.openlocfilehash: ceb66fdacd4a108318c84fd9297aca8b2332c3f3
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481125"
---
# <a name="remoteitem-resource-type"></a>RemoteItem-Ressourcentyp

Die **RemoteItem**-Ressource gibt an, dass ein [**driveItem**](driveitem.md)-Element auf ein Element in einem anderen Laufwerk verweist.
Diese Ressource stellt die eindeutigen IDs des Quelllaufwerks und des Zielelements bereit.

[**DriveItems**](driveitem.md) mit einem **remoteItem**-Facet ungleich Null sind Ressourcen, die freigegeben, zu OneDrive-Umgebungen von Benutzern hinzugefügt oder für Elemente von heterogenen Elementsammlungen (wie z. B. Suchergebnisse) zurückgegeben wurden.

**Hinweis:** Im Gegensatz zu Ordnern im gleichen Laufwerk wird beim Verschieben eines **driveItem**-Elements in ein Remoteelement möglicherweise der `id`-Wert geändert.

## <a name="json-representation"></a>JSON-Darstellung

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.remoteItem", 
       "optionalProperties": ["name", "fileSystemInfo", "file", "folder"] } -->

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
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "size": 1024,
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname        | Typ                                | Beschreibung                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [IdentitySet](identityset.md)       | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.                                                                                  |
| createdDateTime      | Zeitstempel                           | Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.                                                                                                                        |
| file                 | [Datei](file.md)                     | Gibt an, dass das Remote-Element eine Datei ist. Schreibgeschützt.                                                                                                              |
| fileSystemInfo       | [FileSystemInfo](filesysteminfo.md) | Informationen über das Remote-Element aus dem lokalen Dateisystem. Schreibgeschützt.                                                                                          |
| folder               | [Ordner](folder.md)                 | Gibt an, dass das Remote-Element ein Ordner ist. Schreibgeschützt.                                                                                                            |
| id                   | String                              | Eindeutige ID für das Remote-Element in dem Laufwerk. Schreibgeschützt.                                                                                                    |
| lastModifiedBy       | [IdentitySet](identityset.md)       | Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.                                                                            |
| lastModifiedDateTime | Timestamp                           | Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.                                                                                                              |
| name                 | String                              | Optional. Dateiname des Remote-Elements. Schreibgeschützt.                                                                                                                 |
| package              | [Paket](package.md)               | Zeigt wenn vorhanden an, dass das Element ein Paket ist statt eines Ordners oder einer Datei. Pakete werden in einigen Kontexten wie Dateien, in anderen Kontexten wie Ordner behandelt. Schreibgeschützt. |
| parentReference      | [ItemReference](itemreference.md)   | Eigenschaften des übergeordneten Elements des Remote-Elements. Schreibgeschützt.                                                                                                           |
| shared               | [shared](shared.md)                 | Gibt an, dass das Element für andere freigegeben wurde, und enthält den „freigegeben“-Status des Elements. Schreibgeschützt.                                       |
| sharepointIds        | [SharepointIds](sharepointids.md)   | Bietet Interoperabilität zwischen Elementen in OneDrive for Business und SharePoint mit vollständigem Satz an Element-IDs. Schreibgeschützt.                                          |
| size                 | Int64                               | Größe des Remote-Elements. Schreibgeschützt.                                                                                                                               |
| specialFolder        | [specialFolder][]                   | Facet, das zurückgegeben wird, wenn das aktuelle Element auch als spezieller Ordner verfügbar ist. Schreibgeschützt.                                                                     |
| webDavUrl            | Url                                 | DAV-kompatible URL für das Element.                                                                                                                                  |
| webUrl               | Url                                 | URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.                                                                                                         |

[specialFolder]: specialfolder.md

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets einer **driveItem**-Ressourcen finden Sie unter [driveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->
