---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5b3618610a803f86852a95ed1cb662f98cfb6e3f
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482133"
---
# <a name="listinfo-resource"></a>ListInfo-Ressource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Der Komplexe Typ **listInfo** enthält zusätzliche Informationen zu einer [Liste][].

[Liste]: list.md

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.listInfo"
}-->

```json
{
  "contentTypesEnabled": false,
  "hidden": false,
  "template": "documentLibrary | genericList | tasks | survey | links | announcements | contacts | ..."
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname           | Typ    | Beschreibung
|:------------------------|:--------|:------------------------------------------------
| **contentTypesEnabled** | Boolesch | `true` gibt an, dass die Inhaltstypen für diese Liste aktiviert sind.
| **hidden**              | Boolean | `true` gibt an, dass die Liste normalerweise nicht in die SharePoint-Benutzeroberfläche angezeigt wird.
| **template**            | string  | Ein Aufzählungswert, der die bei der Erstellung der Liste verwendete Basislistenvorlage verwendet. Beispielwerte: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` etc.

### <a name="remarks"></a>Hinweise

Obgleich die meisten von Benutzern erstellen Listen einen der oben aufgeführten Werte enthalten, sind andere Werte ebenfalls möglich.
Ihre App sollte darauf vorbereitet werden, auch alle hier nicht aufgelisteten Werte zu verarbeiten.
Hinweis für Entwickler, die mit CSOM-APIs von SharePoint vertraut sind: Der `template`-Wert entspricht der `SPListTemplateType`-Enumeration.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/listinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
