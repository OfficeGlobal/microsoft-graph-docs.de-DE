---
title: Ressourcentyp chatMessageMention
description: 'Stellt einen Vermerk in einer ChatMessage Entität dar. Benutzer, Team, Bot oder DDE-Kanal kann die Erwähnung sein. '
localization_priority: Normal
ms.openlocfilehash: 7b24d2af6f61f3da69480557e1c5b5f32c009c25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876138"
---
# <a name="chatmessagemention-resource-type"></a>Ressourcentyp chatMessageMention

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt einen Vermerk in einer [ChatMessage](chatmessage.md) Entität dar. Benutzer, Team, Bot oder DDE-Kanal kann die Erwähnung sein. 

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|string|ID der Entität erwähnt wird|
|mentionText|string|Zeichenfolge, mit der Erwähnung Ex dargestellt: Anzeigename des Benutzers, Teamname usw.|
|erwähnten|[identitySet](identityset.md)|Der Benutzer, der erwähnt wurde|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
