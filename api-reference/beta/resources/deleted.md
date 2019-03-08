---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Gelöscht
localization_priority: Normal
ms.openlocfilehash: 06fe9835ef4b31d7a48bad955b17872142a94b2d
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480782"
---
# <a name="deleted-facet"></a>Facet „Deleted“

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **Deleted**-Ressource gibt an, dass das Element gelöscht wurde. In dieser Version der API gibt das Vorhandensein (nicht Null) des Ressourcenwerts an, dass die Datei gelöscht wurde. Ein NULL-Werte (oder ein fehlender Wert) gibt an, dass die Datei nicht gelöscht wurde.

Unter [Änderungen für ein Element anzeigen](../api/driveitem-delta.md) finden Sie weitere Informationen zum Nachverfolgen von Änderungen und zum Suchen gelöschter Elemente.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "state"
  ],
  "@odata.type": "microsoft.graph.deleted"
}-->
```json
{
  "state": "string"
}
```
## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ   | Beschreibung                               |
|:---------|:-------|:------------------------------------------|
| state    | String | Stellt den Status des gelöschten Elements dar. |

## <a name="remarks"></a>Bemerkungen 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted",
  "suppressions": [
    "Error: /api-reference/beta/resources/deleted.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
