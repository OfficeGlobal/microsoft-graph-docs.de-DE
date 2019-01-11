---
title: messageRuleActions-Ressourcentyp
description: Stellt die Reihe von Aktionen dar, die für eine Regel verfügbar sind.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: f6a78442dc82cade6b7e6d9a793fb6e49b3a1beb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889040"
---
# <a name="messageruleactions-resource-type"></a>messageRuleActions-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Reihe von Aktionen dar, die für eine Regel verfügbar sind.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| assignCategories | Zeichenfolgenauflistung | Eine Liste von Kategorien, die einer Nachricht zugewiesen werden sollen. |
| copyToFolder | Zeichenfolge | Die ID eines Ordners, in den eine Nachricht kopiert werden soll. |
| Löschen | Boolescher Wert | Gibt an, ob eine Nachricht in den Ordner „Gelöschte Elemente“ verschoben werden soll. |
| forwardAsAttachmentTo | [recipient](recipient.md)-Sammlung | Die E-Mail-Adressen der Empfänger, an die eine Nachricht als Anlage weitergeleitet werden soll. |
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
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
