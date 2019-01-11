---
title: messageRulePredicates-Ressourcentyp
description: Steht für die Gruppe von Bedingungen und Ausnahmen, die für eine Regel zur Verfügung stehen.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 13978b4ee09f863ee3f57ac109ee8f3f5adf39c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804739"
---
# <a name="messagerulepredicates-resource-type"></a>messageRulePredicates-Ressourcentyp


Steht für die Gruppe von Bedingungen und Ausnahmen, die für eine Regel zur Verfügung stehen.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| bodyContains | Collection(String) | Steht für die Zeichenfolgen, die im Textkörper einer eingehenden Nachricht angezeigt werden sollten, damit die Bedingung oder Ausnahme zutrifft. |
| bodyOrSubjectContains | Collection(String) | Steht für die Zeichenfolgen, die im Textkörper oder Betreff einer eingehenden Nachricht angezeigt werden sollten, damit die Bedingung oder Ausnahme zutrifft. |
| categories | Collection(String) | Steht für die Kategorien, mit denen eine eingehende Nachricht gekennzeichnet werden sollte, damit die Bedingung oder Ausnahme zutrifft. |
| fromAddresses | Auflistung ([Empfänger](recipient.md)) | Steht für die speziellen Absender-E-Mail-Adressen einer eingehenden Nachricht, damit die Bedingung oder Ausnahme zutrifft. |
| hasAttachments | Boolescher Wert | Gibt an, ob eine eingehende Nachricht Anlagen aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft. |
| HeaderContains | Collection(String) | Steht für die Zeichenfolgen, die in den Kopfzeilen einer eingehenden Nachricht angezeigt werden sollten, damit die Bedingung oder Ausnahme zutrifft. |
| Wichtigkeit | Wichtigkeit | Die Wichtigkeit einer eingehenden Nachricht, damit die Bedingung oder Ausnahme zutrifft: `low`, `normal`, `high`. |
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
| messageActionFlag | messageActionFlag  | Steht für den flag-for-action-Wert, der in einer eingehenden Nachricht angezeigt wird, damit die Bedingung oder Ausnahme zutrifft. Die möglichen Werte sind: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`. |
| notSentToMe | Boolescher Wert | Gibt an, ob der Besitzer des Postfachs kein Empfänger einer eingehenden Nachrichten sein darf, damit die Bedingung oder Ausnahme zutrifft. |
| recipientContains | Collection(String) | Steht für die Zeichenfolgen, die in den Eigenschaften **toRecipients** oder **ccRecipients** einer eingehenden Nachricht angezeigt werden sollten, damit die Bedingung oder Ausnahme zutrifft. |
| senderContains | Collection(String) | Steht für die Zeichenfolgen, die in der **from**-Eigenschaft Kopfzeilen einer eingehenden Nachricht angezeigt werden sollten, damit die Bedingung oder Ausnahme zutrifft. |
| sensitivity | sensitivity | Steht für die Vertraulichkeitsstufe, mit der eine eingehende Nachricht gekennzeichnet werden sollte, damit die Bedingung oder Ausnahme zutrifft. Die möglichen Werte sind: `normal`, `personal`, `private`, `confidential`. |
| sentCcMe | Boolescher Wert | Gibt an, ob sich der Besitzer des Postfachs in der **ccRecipients**-Eigenschaft einer eingehenden Nachrichten befinden muss, damit die Bedingung oder Ausnahme zutrifft. |
| sentOnlyToMe | Boolescher Wert | Gibt an, ob der Besitzer des Postfachs der einzige Empfänger in einer eingehenden Nachrichten sein muss, damit die Bedingung oder Ausnahme zutrifft. |
| sentToAddresses | Auflistung ([Empfänger](recipient.md)) | Steht für die E-Mail-Adressen, an die eine eingehenden Nachricht gesendet werden muss, damit die Bedingung oder Ausnahme zutrifft. |
| sentToMe | Boolescher Wert | Gibt an, ob sich der Besitzer des Postfachs in der **toRecipients**-Eigenscahft einer eingehenden Nachrichten befinden muss, damit die Bedingung oder Ausnahme zutrifft. |
| sentToOrCcMe | Boolescher Wert | Gibt an, ob sich der Besitzer des Postfachs in der **toRecipients**-Eigenschaft oder in der **ccRecipients**-Eigenschaft einer eingehenden Nachrichten befinden muss, damit die Bedingung oder Ausnahme zutrifft. |
| SubjectContains | Collection(String) | Steht für die Zeichenfolgen, die im Betreiff einer eingehenden Nachricht angezeigt werden sollten, damit die Bedingung oder Ausnahme zutrifft. |
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
  "fromAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
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
  "sentToAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "sentToMe": "Boolean",
  "sentToOrCcMe": "Boolean",
  "subjectContains": ["String"],
  "withinSizeRange": {"@odata.type": "microsoft.graph.sizeRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRulePredicates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
