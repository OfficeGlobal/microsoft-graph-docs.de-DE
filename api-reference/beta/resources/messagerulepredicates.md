---
title: messageRulePredicates-Ressourcentyp
description: Steht für die Gruppe von Bedingungen und Ausnahmen, die für eine Regel zur Verfügung stehen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 324c46728b33e70bae66426c6fbfd46ba830246b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571835"
---
# <a name="messagerulepredicates-resource-type"></a>messageRulePredicates-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Steht für die Gruppe von Bedingungen und Ausnahmen, die für eine Regel zur Verfügung stehen.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| bodyContains |  Zeichenfolgenauflistung | Steht für die Zeichenfolgen, die im Textkörper einer eingehenden Nachricht angezeigt werden sollten, damit die Bedingung oder Ausnahme zutrifft. |
| bodyOrSubjectContains |  Zeichenfolgenauflistung | Steht für die Zeichenfolgen, die im Textkörper oder Betreff einer eingehenden Nachricht angezeigt werden sollten, damit die Bedingung oder Ausnahme zutrifft. |
| categories | Zeichenfolgenauflistung | Steht für die Kategorien, mit denen eine eingehende Nachricht gekennzeichnet werden sollte, damit die Bedingung oder Ausnahme zutrifft. |
| fromAddresses |  [recipient](recipient.md) collection | Steht für die speziellen Absender-E-Mail-Adressen einer eingehenden Nachricht, damit die Bedingung oder Ausnahme zutrifft. |
| hasAttachments | Boolescher Wert | Gibt an, ob eine eingehende Nachricht Anlagen aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft. |
| HeaderContains | Zeichenfolgenauflistung  | Steht für die Zeichenfolgen, die in den Kopfzeilen einer eingehenden Nachricht angezeigt werden sollten, damit die Bedingung oder Ausnahme zutrifft. |
| Wichtigkeit | Zeichenfolge | Die Wichtigkeit einer eingehenden Nachricht, damit die Bedingung oder Ausnahme zutrifft: `low`, `normal`, `high`. |
| isApprovalRequest | Boolescher Wert | Gibt an, ob eine eingehende Nachricht eine Genehmigungsanforderung sein muss, damit die Bedingung oder Ausnahme zutrifft. |
| isAutomaticForward | Boolescher Wert | Gibt an, ob eine eingehende Nachricht automatisch weitergeleitet werden muss, damit die Bedingung oder Ausnahme zutrifft. |
| isAutomaticReply | Boolescher Wert | Gibt an, ob eine eingehende Nachricht eine automatische Antwort sein muss, damit die Bedingung oder Ausnahme zutrifft. |
| isEncrypted | Boolescher Wert | Gibt an, ob eine eingehende Nachricht verschlüsselt sein muss, damit die Bedingung oder Ausnahme zutrifft. |
| isMeetingRequest | Boolescher Wert | Gibt an, ob eine eingehende Nachricht eine Besprechungsanfrage sein muss, damit die Bedingung oder Ausnahme zutrifft. |
| isMeetingResponse | Boolescher Wert | Gibt an, ob eine eingehende Nachricht eine Besprechungsantwort sein muss, damit die Bedingung oder Ausnahme zutrifft. |
| isNonDeliveryReport | Boolescher Wert | Gibt an, ob eine eingehende Nachricht ein Unzustellbarkeitsbericht sein muss, damit die Bedingung oder Ausnahme zutrifft. |
| isPermissionControlled | Boolescher Wert | Gibt an, ob eine eingehende Nachricht berechtigungsgesteuert (RMS-geschützt) sein muss, damit die Bedingung oder Ausnahme zutrifft. |
| isReadReceipt | Boolescher Wert | Gibt an, ob eine eingehende Nachricht eine Lesebestätigung sein muss, damit die Bedingung oder Ausnahme zutrifft. |
| isSigned | Boolescher Wert | Gibt an, ob eine eingehende Nachricht S/MIME-signiert sein muss, damit die Bedingung oder Ausnahme zutrifft. |
| isVoicemail | Boolescher Wert | Gibt an, ob eine eingehende Nachricht eine Voicemail sein muss, damit die Bedingung oder Ausnahme zutrifft. |
| messageActionFlag | Zeichenfolge  | Steht für den flag-for-action-Wert, der in einer eingehenden Nachricht angezeigt wird, damit die Bedingung oder Ausnahme zutrifft. Mögliche Werte sind: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`. |
| notSentToMe | Boolescher Wert | Gibt an, ob der Besitzer des Postfachs kein Empfänger einer eingehenden Nachrichten sein darf, damit die Bedingung oder Ausnahme zutrifft. |
| recipientContains | Zeichenfolgenauflistung | Steht für die Zeichenfolgen, die in den Eigenschaften **toRecipients** oder **ccRecipients** einer eingehenden Nachricht angezeigt werden sollten, damit die Bedingung oder Ausnahme zutrifft. |
| senderContains |  Zeichenfolgenauflistung | Steht für die Zeichenfolgen, die in der **from**-Eigenschaft Kopfzeilen einer eingehenden Nachricht angezeigt werden sollten, damit die Bedingung oder Ausnahme zutrifft. |
| sensitivity | Zeichenfolge | Steht für die Vertraulichkeitsstufe, mit der eine eingehende Nachricht gekennzeichnet werden sollte, damit die Bedingung oder Ausnahme zutrifft. Mögliche Werte: `normal`, `personal`, `private`, `confidential` |
| sentCcMe | Boolescher Wert | Gibt an, ob sich der Besitzer des Postfachs in der **ccRecipients**-Eigenschaft einer eingehenden Nachrichten befinden muss, damit die Bedingung oder Ausnahme zutrifft. |
| sentOnlyToMe | Boolescher Wert | Gibt an, ob der Besitzer des Postfachs der einzige Empfänger in einer eingehenden Nachrichten sein muss, damit die Bedingung oder Ausnahme zutrifft. |
| sentToAddresses |  [recipient](recipient.md) collection | Steht für die E-Mail-Adressen, an die eine eingehenden Nachricht gesendet werden muss, damit die Bedingung oder Ausnahme zutrifft. |
| sentToMe | Boolescher Wert | Gibt an, ob sich der Besitzer des Postfachs in der **toRecipients**-Eigenscahft einer eingehenden Nachrichten befinden muss, damit die Bedingung oder Ausnahme zutrifft. |
| sentToOrCcMe | Boolescher Wert | Gibt an, ob sich der Besitzer des Postfachs in der **toRecipients**-Eigenschaft oder in der **ccRecipients**-Eigenschaft einer eingehenden Nachrichten befinden muss, damit die Bedingung oder Ausnahme zutrifft. |
| SubjectContains | Zeichenfolgenauflistung | Steht für die Zeichenfolgen, die im Betreiff einer eingehenden Nachricht angezeigt werden sollten, damit die Bedingung oder Ausnahme zutrifft. |
| withinSizeRange | [sizeRange](sizerange.md) | Gibt die maximale und minimale Größe (in Kilobyte) an, zwischen der eine eingehende Nachricht liegen muss, damit eine Bedingung oder Ausnahme zutrifft. |



## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRulePredicates"
}-->

```json
{
  "bodyContains": ["String"],
  "bodyOrSubjectContains": ["String"],
  "categories": ["String"],
  "fromAddresses": [{"@odata.type": "#microsoft.graph.recipient"}],
  "hasAttachments": "Boolean",
  "headerContains": ["String"],
  "importance": "String",
  "isApprovalRequest": "Boolean",
  "isAutomaticForward": "Boolean",
  "isAutomaticReply": "Boolean",
  "isEncrypted": "Boolean",
  "isMeetingRequest": "Boolean",
  "isMeetingResponse": "Boolean",
  "isNonDeliveryReport": "Boolean",
  "isPermissionControlled": "Boolean",
  "isReadReceipt": "Boolean",
  "isSigned": "Boolean",
  "isVoicemail": "Boolean",
  "messageActionFlag": "String",
  "notSentToMe": "Boolean",
  "recipientContains": ["String"],
  "senderContains": ["String"],
  "sensitivity": "String",
  "sentCcMe": "Boolean",
  "sentOnlyToMe": "Boolean",
  "sentToAddresses": [{"@odata.type": "#microsoft.graph.recipient"}],
  "sentToMe": "Boolean",
  "sentToOrCcMe": "Boolean",
  "subjectContains": ["String"],
  "withinSizeRange": {"@odata.type": "#microsoft.graph.sizeRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRulePredicates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/messagerulepredicates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
