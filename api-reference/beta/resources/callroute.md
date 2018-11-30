---
title: Ressourcentyp callRoute
description: Der Typ des CallRoute.
ms.openlocfilehash: d2a85d34fe755c6e725abc9a1308a3837f0acf3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060373"
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
