---
title: Ressourcentyp automaticRepliesMailTips
description: E-Mail-Infos zu automatischen Antworten, die für ein Postfach festgelegt wurden.
localization_priority: Normal
ms.openlocfilehash: bb477979b975996f70e4b8ac624befab7f254f46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816275"
---
# <a name="automaticrepliesmailtips-resource-type"></a>Ressourcentyp automaticRepliesMailTips


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
