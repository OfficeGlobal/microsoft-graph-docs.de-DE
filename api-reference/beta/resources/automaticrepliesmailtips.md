---
title: Ressourcentyp automaticRepliesMailTips
description: E-Mail-Infos zu automatischen Antworten, die für ein Postfach festgelegt wurden.
localization_priority: Normal
ms.openlocfilehash: 7eb9d57da427090c554e111ae6ba1eeb369437ca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513676"
---
# <a name="automaticrepliesmailtips-resource-type"></a>Ressourcentyp automaticRepliesMailTips

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/automaticrepliesmailtips.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
