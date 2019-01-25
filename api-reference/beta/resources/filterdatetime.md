---
title: FilterDatetime-Ressourcentyp
description: Stellt dar, wie ein Datum beim Filtern nach Werten gefiltert wird.
localization_priority: Normal
ms.openlocfilehash: ad4341e13eadc911377ec7b9859d6a31305fadf8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507551"
---
# <a name="filterdatetime-resource-type"></a>FilterDatetime-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt dar, wie ein Datum beim Filtern nach Werten gefiltert wird.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|date|string|Das Datum im ISO8601-Format zum Filtern von Daten.|
|specificity|string|Genauigkeit des Datums zum Beibehalten von Daten. Wenn z. B. das Datum 2005-04-02 ist und die Spezifität auf „Monat“ festgelegt ist, werden beim Filtervorgang alle Zeilen mit einem Datum im Monat April 2009 beibehalten. Mögliche Werte:`Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/filterdatetime.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
