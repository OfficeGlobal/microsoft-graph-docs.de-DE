---
title: Ressourcentyp meetingCapability
description: Enthält die Funktionen einer Besprechung
ms.openlocfilehash: 438193d08ab5542f07d4cbf61704520d81433e50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061416"
---
# <a name="meetingcapability-resource-type"></a>Ressourcentyp meetingCapability

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Enthält die Funktionen einer Besprechung

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ    | Beschreibung|
|:---------------|:--------|:----------|
| allowAnonymousUsersToDialOut | Boolesch | Gibt an, ob anonyme Benutzer als Client-Anschluss in einer Besprechung zulässig ist. |
| autoAdmittedUsers | String | Mögliche Werte: `everyoneInCompany`, `everyone`. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
