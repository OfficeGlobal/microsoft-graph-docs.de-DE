---
title: customTimeZone-Ressourcentyp
description: Stellt eine Zeitzone dar, in der der Übergang von Standardzeit zu Sommerzeit oder umgekehrt nicht Standard ist.
ms.openlocfilehash: 83375c96e4247cb0ddf2d17b1bede2c295f0b27f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058250"
---
# <a name="customtimezone-resource-type"></a>customTimeZone-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->