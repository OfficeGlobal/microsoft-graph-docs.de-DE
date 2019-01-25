---
title: e-Mail-Infos Ressourcentyp
description: 'Informative Nachrichten über einen Empfänger, die beim Verfassen einer Nachricht angezeigt werden. Beispielsweise eine Out-of-Office-Nachricht '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 11e64c09a90d130b7656d4e87770e6df3fb67408
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508412"
---
# <a name="mailtips-resource-type"></a>e-Mail-Infos Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informative Nachrichten über einen Empfänger, die beim Verfassen einer Nachricht angezeigt werden. Beispielsweise eine Abwesenheits Nachricht als automatische Antwort für einen Nachrichtenempfänger.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | Mail-Tipps für die automatische Antwort, wenn es vom Empfänger eingerichtet wurde. |
| CustomMailTip | String | Eine benutzerdefinierte e-Mail-Info, die für das Postfach des Empfängers festgelegt werden kann. |
| DeliveryRestricted| Boolescher Wert | Gibt an, ob das Postfach des Empfängers beschränkt, beispielsweise ist akzeptieren von Nachrichten aus einer vordefinierten Liste Absender, ablehnen von Nachrichten aus einer vordefinierten Liste der Absender oder Nachrichten von nur von authentifizierten Absendern akzeptieren. |
| emailAddress | [emailAddress](../resources/emailaddress.md) | Die e-Mail-Adresse des Empfängers zum Abrufen von e-Mail-Infos für. |
| error | [mailTipsError](../resources/mailtipserror.md) | Fehler, die während der Aktion [GetMailTips](../api/user-getmailtips.md) auftreten. |
| ExternalMemberCount | Int32 | Die Anzahl der externen Elemente, wenn beim Empfänger um eine Verteilerliste handelt. |
| IsModerated |Boolescher Wert  | Gibt an, ob das Senden von Nachrichten an den Empfänger genehmigt werden muss. Angenommen, wurde Wenn der Empfänger eine große Verteilerliste ist und eine Moderator festgelegt bis zu an diese Verteilerliste gesendete Nachrichten genehmigen oder wenn Senden von Nachrichten an ein Empfänger Genehmigung des Managers des Empfängers erforderlich. |
| MailboxFull | Boolescher Wert | Der vollständige Postfachstatus des Empfängers. |
| MaxMessageSize | Int32 | Die maximale Nachrichtengröße für die Organisation oder das Postfach des Empfängers konfiguriert wurde. |
| recipientScope | String | Der Bereich des Empfängers. Mögliche Werte sind: `none`, `internal`, `external`, `externalPartner` und `externalNonParther`. Beispielsweise kann ein Administrator einer anderen Organisation zu seinem "Partner" festgelegt. Der Bereich ist nützlich, wenn ein Administrator möchte, dass bestimmte e-Mail-Infos für bestimmte Bereiche zugänglich sein. Es ist außerdem hilfreich, Absender zu informieren, dass ihre Nachricht die Organisation, deren Unterstützung bei der richtigen Entscheidungen zu Wortlaut, Ton und Inhalte lassen kann.|
| recipientSuggestions | [recipient](../resources/recipient.md) collection | Empfänger vorgeschlagene basierend auf vorherigen Kontext, in dem sie in der gleichen Nachricht angezeigt werden. |
| TotalMemberCount | Int32 | Die Anzahl der Elemente, wenn der Empfänger eine Verteilerliste handelt. |

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
<!--
{
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailtips.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
