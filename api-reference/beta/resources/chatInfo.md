---
title: Ressourcentyp chatInfo
description: Informationen zu einer Nachricht in Microsoft-Teams.
author: VinodRavichandran
ms.openlocfilehash: 45af1a7e178286c77ed4bf90528eb602fd48a6bb
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380415"
---
# <a name="chatinfo-resource-type"></a>Ressourcentyp chatInfo

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Informationen zu einer Nachricht in Microsoft-Teams.

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ    | Beschreibung|
|:--------------------|:--------|:-----------|
| messageId           | Zeichenfolge  | Der eindeutige Bezeichner für eine Nachricht in einem Microsoft-Teams Kanal. |
| replyChainMessageId | Zeichenfolge  | Die ID der Antwort-Nachricht. |
| threadId            | Zeichenfolge  | Der eindeutige Bezeichner für ein Thread im Microsoft-Teams. |

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
