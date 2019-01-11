---
title: Ressourcentyp automaticRepliesSetting
description: 'Konfigurationseinstellungen automatisch benachrichtigt den Absender einer eingehenden e-Mail mit einer Nachricht aus der '
localization_priority: Normal
ms.openlocfilehash: 0160197a4fafe10b7f78be9124da3b6260bfcee6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820657"
---
# <a name="automaticrepliessetting-resource-type"></a>Ressourcentyp automaticRepliesSetting

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer. Beispiel: eine automatische Antwort, die darüber informiert, dass der angemeldete Benutzer zur Beantwortung von E-Mails nicht verfügbar ist. 


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|externalAudience|String| Die Zielgruppe außerhalb der Organisation des angemeldeten Benutzers, der **ExternalReplyMessage** erhält, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist. Mögliche Werte: `none`, `contactsOnly`, `all`.|
|externalReplyMessage|string|Die automatische Antwort an die angegebene externe Zielgruppe, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist.|
|internalReplyMessage|string|Die automatische Antwort an die interne Zielgruppe in der Organisation des angemeldeten Benutzers, wenn **Status** `AlwaysEnabled` oder `Scheduled` ist. |
|scheduledEndDateTime|[dateTimeTimeZone](datetimetimezone.md)|Datum und Uhrzeit, die zum Beenden der automatischen Antworten festgelegt werden, wenn **Status** auf `Scheduled` gesetzt ist. |
|scheduledStartDateTime|[dateTimeTimeZone](datetimetimezone.md)|Datum und Uhrzeit, die für den Beginn der automatischen Antworten festgelegt werden, wenn **Status** auf `Scheduled` gesetzt ist.|
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
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
