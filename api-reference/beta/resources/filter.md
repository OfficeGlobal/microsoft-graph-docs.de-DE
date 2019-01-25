---
title: Filter-Ressourcentyp
description: Verwaltet das Filtern der Spalte einer Tabelle.
localization_priority: Normal
ms.openlocfilehash: 6adc4e378b47bcb134a640e77bf54c32a35b3be2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518891"
---
# <a name="filter-resource-type"></a>Filter-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/filter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
