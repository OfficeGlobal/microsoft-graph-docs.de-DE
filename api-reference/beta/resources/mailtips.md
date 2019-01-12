---
title: e-Mail-Infos Ressourcentyp
description: 'Informative Nachrichten über einen Empfänger, die beim Verfassen einer Nachricht angezeigt werden. Beispielsweise eine Out-of-Office-Nachricht '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ed6d43e033b020b884a6cd1b6220b1ff566a507b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985956"
---
# <a name="mailtips-resource-type"></a>e-Mail-Infos Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Informative Nachrichten über einen Empfänger, die beim Verfassen einer Nachricht angezeigt werden. Beispielsweise eine Abwesenheits Nachricht als automatische Antwort für einen Nachrichtenempfänger.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | Mail-Tipps für die automatische Antwort, wenn es vom Empfänger eingerichtet wurde. |
| customMailTip | Zeichenfolge | Eine benutzerdefinierte e-Mail-Info, die für das Postfach des Empfängers festgelegt werden kann. |
| deliveryRestricted| Boolescher Wert | Gibt an, ob das Postfach des Empfängers beschränkt, beispielsweise ist akzeptieren von Nachrichten aus einer vordefinierten Liste Absender, ablehnen von Nachrichten aus einer vordefinierten Liste der Absender oder Nachrichten von nur von authentifizierten Absendern akzeptieren. |
| emailAddress | [emailAddress](../resources/emailaddress.md) | Die e-Mail-Adresse des Empfängers zum Abrufen von e-Mail-Infos für. |
| error | [mailTipsError](../resources/mailtipserror.md) | Fehler, die während der Aktion [GetMailTips](../api/user-getmailtips.md) auftreten. |
| externalMemberCount | Int32 | Die Anzahl der externen Elemente, wenn beim Empfänger um eine Verteilerliste handelt. |
| isModerated |Boolescher Wert  | Gibt an, ob das Senden von Nachrichten an den Empfänger genehmigt werden muss. Angenommen, wurde Wenn der Empfänger eine große Verteilerliste ist und eine Moderator festgelegt bis zu an diese Verteilerliste gesendete Nachrichten genehmigen oder wenn Senden von Nachrichten an ein Empfänger Genehmigung des Managers des Empfängers erforderlich. |
| mailboxFull | Boolescher Wert | Der vollständige Postfachstatus des Empfängers. |
| maxMessageSize | Int32 | Die maximale Nachrichtengröße für die Organisation oder das Postfach des Empfängers konfiguriert wurde. |
| recipientScope | Zeichenfolge | Der Bereich des Empfängers. Mögliche Werte sind: `none`, `internal`, `external`, `externalPartner` und `externalNonParther`. Beispielsweise kann ein Administrator einer anderen Organisation zu seinem "Partner" festgelegt. Der Bereich ist nützlich, wenn ein Administrator möchte, dass bestimmte e-Mail-Infos für bestimmte Bereiche zugänglich sein. Es ist außerdem hilfreich, Absender zu informieren, dass ihre Nachricht die Organisation, deren Unterstützung bei der richtigen Entscheidungen zu Wortlaut, Ton und Inhalte lassen kann.|
| recipientSuggestions | [recipient](../resources/recipient.md)-Sammlung | Empfänger vorgeschlagene basierend auf vorherigen Kontext, in dem sie in der gleichen Nachricht angezeigt werden. |
| totalMemberCount | Int32 | Die Anzahl der Elemente, wenn der Empfänger eine Verteilerliste handelt. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
