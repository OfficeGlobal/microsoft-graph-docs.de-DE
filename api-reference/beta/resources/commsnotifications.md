---
title: Ressourcentyp commsNotifications
description: Liste der Benachrichtigungen für mehrere Benachrichtigungen gesendet werden in einem einzelnen Batch von den Communications-Servern verwendet.
author: VinodRavichandran
ms.openlocfilehash: 052520a99081e5c09cd6e3ec3b74f74e9527d38d
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380450"
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