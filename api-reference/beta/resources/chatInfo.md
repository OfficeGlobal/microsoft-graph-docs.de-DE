---
title: Ressourcentyp chatInfo
description: Informationen zu einer Nachricht in Microsoft-Teams.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: c2cc0dd288abdab7852017600c4c55b9a40b0aa7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852941"
---
# <a name="chatinfo-resource-type"></a>Ressourcentyp chatInfo

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Informationen zu einer Nachricht in Microsoft-Teams.

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ    | Beschreibung|
|:--------------------|:--------|:-----------|
| messageId           | String  | Der eindeutige Bezeichner für eine Nachricht in einem Microsoft-Teams Kanal. |
| replyChainMessageId | String  | Die ID der Antwort-Nachricht. |
| threadId            | String  | Der eindeutige Bezeichner für ein Thread im Microsoft-Teams. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
