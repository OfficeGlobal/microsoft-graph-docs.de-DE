---
title: DriveItemVersion-Ressourcentyp
description: Die Ressource **DriveItemVersion** stellt eine bestimmte Version von einer DriveItem dar.
ms.openlocfilehash: e257e800b0ac8ad4d94027f9c8040ffb3b20ea90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017655"
---
# <a name="driveitemversion-resource-type"></a>DriveItemVersion-Ressourcentyp

Die **DriveItemVersion**-Ressource stellt eine bestimmte Version eines [DriveItem](driveitem.md) dar.


## <a name="tasks-on-driveitemversion-resources"></a>Aufgaben für DriveItemVersion-Ressourcen

Die folgenden Aufgaben sind für driveItemVersion-Ressourcen verfügbar.

|            Häufige Aufgaben             |         HTTP-Methode         |
| :--------------------------------- | :-------------------------- |
| [Versionen auflisten][version-list]      | `GET /drive/items/{item-id}/versions`  |
| [Version abrufen][version-get]         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| [Inhalte abrufen][content-get]        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| [Version wiederherstellen][version-restore] | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

Im Beispiel der vorstehenden Tabelle wird `/drive` verwendet, aber es gibt viele gültige Abfragen.

## <a name="json-representation"></a>JSON-Darstellung

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka": "oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356
}
```

## <a name="properties"></a>Eigenschaften

|      Eigenschaftenname       |                         Typ                         |                               Beschreibung                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | Die ID der Version. Schreibgeschützt.                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | Die Identität des Benutzers, der die Version zuletzt geändert hat. Schreibgeschützt.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Datum und Uhrzeit der letzten Änderung der Version. Schreibgeschützt.                 |
| **Veröffentlichung**          | [PublicationFacet](../resources/publicationfacet.md) | Zeigt den Veröffentlichungsstatus dieser bestimmten Version an. Schreibgeschützt. |
| **size**                 | Int64                                                | Gibt die Größe des Inhalt-Streams für diese Version des Elements an.  |
| **content**              | Stream                                               | Der Inhaltsstream für diese Version des Elements.                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
