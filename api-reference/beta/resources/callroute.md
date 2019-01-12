---
title: Ressourcentyp callRoute
description: Der Typ des CallRoute.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd131afcdb5581a719107d9fd3a9a597979d6f21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933071"
---
# <a name="callroute-resource-type"></a>Ressourcentyp callRoute

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Der Typ des CallRoute.

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ                          | Beschreibung                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| endgültige               | [identitySet](identityset.md) | Die Identität, die in die Unterhaltung aufgelöst wurde.               |
| Original            | [identitySet](identityset.md) | Die Identität, die ursprünglich in den Anruf verwendet wurde.           |
| routingType         | Zeichenfolge                        | Mögliche Werte sind: `forwarded`, `lookup` und `selfFork`.  |

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
