---
title: Ressourcentyp chatMessageMention
description: 'Stellt einen Vermerk in einer ChatMessage Entität dar. Benutzer, Team, Bot oder DDE-Kanal kann die Erwähnung sein. '
ms.openlocfilehash: 5f1e427b0ed2b8ffcfbc86417beb4719dc6fb2a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058431"
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
