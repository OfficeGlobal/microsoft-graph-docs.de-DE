---
title: messageRuleActions-Ressourcentyp
description: Stellt die Reihe von Aktionen dar, die für eine Regel verfügbar sind.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a786a225bb9d439d60a29d2395b2d438975fc16c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523232"
---
# <a name="messageruleactions-resource-type"></a>messageRuleActions-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt die Reihe von Aktionen dar, die für eine Regel verfügbar sind.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| assignCategories | Zeichenfolgenauflistung | Eine Liste von Kategorien, die einer Nachricht zugewiesen werden sollen. |
| copyToFolder | String | Die ID eines Ordners, in den eine Nachricht kopiert werden soll. |
| Löschen | Boolescher Wert | Gibt an, ob eine Nachricht in den Ordner „Gelöschte Elemente“ verschoben werden soll. |
| forwardAsAttachmentTo | [recipient](recipient.md) collection | Die E-Mail-Adressen der Empfänger, an die eine Nachricht als Anlage weitergeleitet werden soll. |
| forwardTo | [recipient](recipient.md)-Sammlung | Die E-Mail-Adressen der Empfänger, an die eine Nachricht weitergeleitet werden soll. |
| markAsRead | Boolescher Wert | Gibt an, ob eine Nachricht als gelesen markiert werden soll. |
| markImportance | Zeichenfolge | Legt die Wichtigkeit der Nachricht fest. Die folgenden Einstellungen sind möglich: `low`, `normal`, `high`. |
| moveToFolder |  Zeichenfolge| Die ID des Ordners, in den eine Nachricht verschoben wird. |
| permanentDelete | Boolescher Wert | Gibt an, ob eine Nachricht dauerhaft gelöscht und nicht im Ordner „Gelöschte Elemente“ gespeichert werden soll. |
| redirectTo | [recipient](recipient.md) | Die E-Mail-Adresse, an die eine Nachricht umgeleitet werden soll. |
| stopProcessingRules | Boolescher Wert | Gibt an, ob nachfolgende Regeln ausgewertet werden sollen. |


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": {"@odata.type": "microsoft.graph.recipient"},
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/messageruleactions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
