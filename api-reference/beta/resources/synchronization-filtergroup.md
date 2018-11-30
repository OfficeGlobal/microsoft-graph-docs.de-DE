---
title: Ressourcentyp filterGroup
description: Definiert eine Reihe von Klauseln, die ein Objekt erfüllen muss im Bereich gezogen werden. Ein Objekt gilt für die Gruppe im Bereich (die Gruppe ausgewertet wird, um `true`) nur dann, wenn alle Klauseln der Gruppe für ausgewertet werden `true`.
ms.openlocfilehash: d49f7a4364f1d8ce3e1c4daba3bb331cf9a9c001
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064279"
---
# <a name="filtergroup-resource-type"></a>Ressourcentyp filterGroup

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
<!-- {
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->