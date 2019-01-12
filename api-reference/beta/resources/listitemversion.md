---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: abc6187f4e0ef415ec8a01088fd02aa406b1bc50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933414"
---
# <a name="listitemversion-resource-type"></a>ListItemVersion-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **ListItemVersion**-Ressource stellt eine frühere Version der [ListItem](listitem.md)-Ressource dar.

## <a name="tasks-on-listitemversion-resources"></a>Aufgaben für ListItemVersion-Ressourcen

Die folgenden Aufgaben sind für listItemVersion-Ressourcen verfügbar.

|            Häufige Aufgaben             |         HTTP-Methode         |
| :--------------------------------- | :-------------------------- |
| [Versionen auflisten][version-list]      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| [Version abrufen][version-get]         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| [Version wiederherstellen][version-restore] | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a>JSON-Darstellung

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.listItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a>Eigenschaften

|      Eigenschaftenname       |                         Typ                         |                               Beschreibung                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | Die ID der Version. Schreibgeschützt.                                       |
| **lastModifiedBy**       | [IdentitySet](../resources/identityset.md)           | Die Identität des Benutzers, der die Version zuletzt geändert hat. Schreibgeschützt.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Datum und Uhrzeit der letzten Änderung der Version. Schreibgeschützt.                 |
| **published**            | [PublicationFacet](../resources/publicationfacet.md) | Zeigt den Veröffentlichungsstatus dieser bestimmten Version an. Schreibgeschützt. |


## <a name="relationships"></a>Beziehungen

In der folgenden Tabelle werden die Beziehungen der **driveItemVersion**-Ressource zu anderen Ressourcen angegeben.

| Beziehungsname |                      Typ                      |                               Beschreibung                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| **fields**        | [fieldValueSet](../resources/fieldvalueset.md) | Eine Auflistung der Felder und Werte für diese Version des Listenelements. |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
