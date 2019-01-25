---
title: Ressourcentyp filterGroup
description: Definiert eine Reihe von Klauseln, die ein Objekt erfüllen muss im Bereich gezogen werden. Ein Objekt gilt für die Gruppe im Bereich (die Gruppe ausgewertet wird, um `true`) nur dann, wenn alle Klauseln der Gruppe für ausgewertet werden `true`.
localization_priority: Normal
ms.openlocfilehash: b71bdf16d6639b5ecc8512565ccf56d592a0da58
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514187"
---
# <a name="filtergroup-resource-type"></a>Ressourcentyp filterGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Definiert eine Reihe von Klauseln, die ein Objekt erfüllen muss im Bereich gezogen werden. Ein Objekt gilt für die Gruppe im Bereich (die Gruppe ausgewertet wird, um `true`) nur dann, wenn alle Klauseln der Gruppe für ausgewertet werden `true`.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Klauseln|[FilterClause](synchronization-filterclause.md) -Auflistung|Filtert Klauseln (Conditions) dieser Gruppe an. Alle Klauseln in einer Gruppe eingehalten werden müssen, in der Reihenfolge für die Filtergruppe ergibt `true`.|
|name|String|Lesbare Namen der Filtergruppe.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterGroup"
}-->

```json
{
  "clauses": [{"@odata.type": "microsoft.graph.filterClause"}],
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filtergroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
