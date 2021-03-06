---
title: followupFlag-Ressourcentyp
description: Ermöglicht das Festlegen einer Kennzeichnung für den Benutzer zur späteren Weiterverfolgung. Unterstützte Elemente umfassen message und contact.
localization_priority: Normal
ms.openlocfilehash: f8ae4cdc04b48fe0b6dede437684215cefb75969
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509546"
---
# <a name="followupflag-resource-type"></a>followupFlag-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/followupflag.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
