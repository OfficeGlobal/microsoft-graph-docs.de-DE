---
title: Filter-Ressourcentyp
description: Verwaltet das Filtern der Spalte einer Tabelle.
localization_priority: Normal
ms.openlocfilehash: cc4b1b105c2049b36fa27cb88b41102366648fa8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834664"
---
# <a name="filter-resource-type"></a>Filter-Ressourcentyp

Verwaltet das Filtern der Spalte einer Tabelle.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Apply](../api/filter-apply.md)|Keine|Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.|
|[Clear](../api/filter-clear.md)|Keine|Deaktiviert den Filter für die angegebene Spalte.|

## <a name="properties"></a>Eigenschaften

| Name | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|criteria|[WorkbookFilterCriteria](filtercriteria.md)|Der aktuell angewendete Filter in der angegebenen Spalte. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
