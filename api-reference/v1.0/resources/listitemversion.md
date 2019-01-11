---
title: ListItemVersion-Ressourcentyp
description: Die **ListItemVersion**-Ressource stellt eine frühere Version der ListItem-Ressource dar.
localization_priority: Normal
ms.openlocfilehash: 41dcbeee3f098b6c156a7ddfe484ef42cca8b6d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810682"
---
# <a name="listitemversion-resource-type"></a>ListItemVersion-Ressourcentyp

Die **ListItemVersion**-Ressource stellt eine frühere Version der [ListItem](listitem.md)-Ressource dar.

## <a name="tasks-on-listitemversion-resources"></a>Aufgaben für ListItemVersion-Ressourcen

Die folgenden Aufgaben sind für listItemVersion-Ressourcen verfügbar.

|            Häufige Aufgaben             |         HTTP-Methode         |
| :--------------------------------- | :-------------------------- |
| [Versionen auflisten][version-list]      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| [Version abrufen][version-get]         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| [Version wiederherstellen][version-restore] | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a>JSON-Darstellung

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.listItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
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
