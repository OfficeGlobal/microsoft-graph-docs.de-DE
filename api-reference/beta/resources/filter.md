---
title: Filter-Ressourcentyp
description: Verwaltet das Filtern der Spalte einer Tabelle.
localization_priority: Normal
ms.openlocfilehash: 5bbc4eff85f40e116ea513c27fa2966dd28a5493
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852787"
---
# <a name="filter-resource-type"></a>Filter-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Verwaltet das Filtern der Spalte einer Tabelle.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Apply](../api/filter-apply.md)|Keine|Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.|
|[Clear](../api/filter-clear.md)|Keine|Deaktiviert den Filter für die angegebene Spalte.|

## <a name="properties"></a>Eigenschaften
Keine

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|criteria|[FilterCriteria](filtercriteria.md)|Der aktuell angewendete Filter in der angegebenen Spalte. Schreibgeschützt.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
