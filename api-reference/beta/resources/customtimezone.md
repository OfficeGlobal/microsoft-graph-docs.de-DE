---
title: customTimeZone-Ressourcentyp
description: Stellt eine Zeitzone dar, in der der Übergang von Standardzeit zu Sommerzeit oder umgekehrt nicht Standard ist.
localization_priority: Normal
ms.openlocfilehash: 0bb961e213956ef3142df1f3d55a83918a14fa78
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515251"
---
# <a name="customtimezone-resource-type"></a>customTimeZone-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Zeitzone dar, in der der Übergang von Standardzeit zu Sommerzeit oder umgekehrt nicht Standard ist.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| bias | Edm.Int32 | Der Zeitversatz der Zeitzone von der Koordinierten Weltzeit (UTC). Dieser Wert wird in Minuten angegeben.Zeitzonen, die der UTC voraus sind, haben einen positiven Versatz; Zeitzonen, die hinter der UTC liegen, haben einen negativen Versatz.|
| daylightOffset | [daylightTimeZoneOffset](daylighttimezoneoffset.md) | Gibt an, wann die Zeitzone von Standardzeit in Sommerzeit wechselt. |
| name | string | Der Name der benutzerdefinierten Zeitzone. |
| standardOffset | [standardTimeZoneOffset](standardtimezoneoffset.md) | Gibt an, wann die Zeitzone von Sommerzeit in Standardzeit wechselt. |


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/customtimezone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
