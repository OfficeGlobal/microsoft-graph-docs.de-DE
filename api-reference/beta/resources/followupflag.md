---
title: followupFlag-Ressourcentyp
description: Ermöglicht das Festlegen einer Kennzeichnung für den Benutzer zur späteren Weiterverfolgung. Unterstützte Elemente umfassen message und contact.
localization_priority: Normal
ms.openlocfilehash: aa056d141bfac82b9f039ed705f6de49893783fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869378"
---
# <a name="followupflag-resource-type"></a>followupFlag-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ermöglicht das Festlegen einer Kennzeichnung für den Benutzer zur späteren Weiterverfolgung. Unterstützte Elemente umfassen [message](message.md) und [contact](contact.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet wurde.|
|dueDateTime|**dateTimeTimeZone**|Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet sein muss.|
|flagStatus|Zeichenfolge|Der Status für die Weiterverfolgung eines Elements. Mögliche Werte sind: `notFlagged`, `complete` und `flagged`.|
|startDateTime|**dateTimeTimeZone**|Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beginnen soll.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
