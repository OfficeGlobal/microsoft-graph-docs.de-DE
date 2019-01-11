---
title: Ressourcentyp commsNotification
description: Communications Benachrichtigung Basistyp, der von Änderungen benachrichtigen Communications-Server veröffentlicht wird.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 526ed88f4b1c5983a06b1830f5c0b0bb97cc874e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837149"
---
# <a name="commsnotification-resource-type"></a>Ressourcentyp commsNotification

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Communications Benachrichtigung Basistyp, der von Änderungen benachrichtigen Communications-Server veröffentlicht wird.

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    | Beschreibung                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| changeType     | String  | Mögliche Werte sind: `created`, `updated` und `deleted`.      |
| resource       | String  | Der URI der Ressource, die geändert wurde.                      |

> **Hinweis:** `resourceData` als zusätzliche Daten verfügbar ist. Es ist eine Entität oder Collection(entity) abhängig von der Anzahl der Änderungen in der Benachrichtigung gepackt.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "resourceData"
  ],
  "@odata.type": "microsoft.graph.commsNotification",
  "openType": true
}-->
```json
{
  "changeType": "created | updated | deleted",
  "resource": "String"
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E",
        "state": "incoming"
      }
    }
  ]
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "commsNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
