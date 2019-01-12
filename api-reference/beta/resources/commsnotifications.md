---
title: Ressourcentyp commsNotifications
description: Liste der Benachrichtigungen für mehrere Benachrichtigungen gesendet werden in einem einzelnen Batch von den Communications-Servern verwendet.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 83a89e848d0992d253efb532ed078031b6f965d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946301"
---
# <a name="commsnotifications-resource-type"></a>Ressourcentyp commsNotifications

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Liste der Benachrichtigungen für mehrere Benachrichtigungen gesendet werden in einem einzelnen Batch von den Communications-Servern verwendet.

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ                                                 | Beschreibung                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| Wert          | [CommsNotification](commsnotification.md) -Auflistung | Die Benachrichtigung über eine Änderung in der Ressource. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
