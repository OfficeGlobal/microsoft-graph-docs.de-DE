---
title: Ressourcentyp callRoute
description: Der Typ des CallRoute.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: e417a7e814b5a2a80da1fa9cd7a551f82e0c37db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815085"
---
# <a name="callroute-resource-type"></a>Ressourcentyp callRoute

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Der Typ des CallRoute.

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ                          | Beschreibung                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| endgültige               | [identitySet](identityset.md) | Die Identität, die in die Unterhaltung aufgelöst wurde.               |
| Original            | [identitySet](identityset.md) | Die Identität, die ursprünglich in den Anruf verwendet wurde.           |
| routingType         | String                        | Mögliche Werte sind: `forwarded`, `lookup` und `selfFork`.  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
