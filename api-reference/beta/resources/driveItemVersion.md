---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: DriveItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3f33c59da4a748c176c6044e4db3bac70eac71cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923614"
---
# <a name="driveitemversion-resource-type"></a>DriveItemVersion-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemVersion", "@type.aka": "oneDrive.driveItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
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

## <a name="relationships"></a>Beziehungen

In der folgenden Tabelle werden die Beziehungen der **driveItemVersion**-Ressource zu anderen Ressourcen angegeben.

| Beziehungsname |  Typ  |            Beschreibung             |
| :---------------- | :----- | :--------------------------------- |
| **content**       | Stream | Der Inhalt-Stream der Version. |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
