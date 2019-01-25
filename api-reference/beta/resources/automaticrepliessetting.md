---
title: Ressourcentyp automaticRepliesSetting
description: 'Konfigurationseinstellungen automatisch benachrichtigt den Absender einer eingehenden e-Mail mit einer Nachricht aus der '
localization_priority: Normal
ms.openlocfilehash: 5ff16aa93042e0d66063cb62de7a8dcdf870c892
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529852"
---
# <a name="automaticrepliessetting-resource-type"></a>Ressourcentyp automaticRepliesSetting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer. Beispiel: eine automatische Antwort, die darüber informiert, dass der angemeldete Benutzer zur Beantwortung von E-Mails nicht verfügbar ist. 


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|externalAudience|String| Die Zielgruppe außerhalb der Organisation des angemeldeten Benutzers, der **ExternalReplyMessage** erhält, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist. Mögliche Werte: `none`, `contactsOnly`, `all`.|
|externalReplyMessage|string|Die automatische Antwort an die angegebene externe Zielgruppe, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist.|
|internalReplyMessage|string|Die automatische Antwort an die interne Zielgruppe in der Organisation des angemeldeten Benutzers, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist. |
|scheduledEndDateTime|[dateTimeTimeZone](datetimetimezone.md)|Datum und Uhrzeit, die zum Beenden der automatischen Antworten festgelegt werden, wenn Status auf  gesetzt ist. |
|scheduledStartDateTime|[dateTimeTimeZone](datetimetimezone.md)|Datum und Uhrzeit, die für den Beginn der automatischen Antworten festgelegt werden, wenn Status auf  gesetzt ist.|
|status|String|Konfigurationensstatus für automatische Antworten. Mögliche Werte: `disabled`, `alwaysEnabled`, `scheduled`.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/automaticrepliessetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
