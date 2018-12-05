---
title: Ressourcentyp automaticRepliesMailTips
description: E-Mail-Infos zu automatischen Antworten, die für ein Postfach festgelegt wurden.
ms.openlocfilehash: 51657578474710d40cfc3feabdf41e50e7105942
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065890"
---
# <a name="automaticrepliesmailtips-resource-type"></a>Ressourcentyp automaticRepliesMailTips

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

[E-Mail-Infos](../resources/mailtips.md) zu automatischen Antworten, die für ein Postfach festgelegt wurden.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:-----|:-----|:-----|
| message | String | Die automatische Antwortnachricht. |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | Die Sprache, der in die automatische Antwort ist. |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | Das Datum und die Uhrzeit, die automatische Antworten für das Ende festgelegt sind. |
| scheduledStartTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | Das Datum und die Uhrzeit, die automatische Antworten beginnen festgelegt sind. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->