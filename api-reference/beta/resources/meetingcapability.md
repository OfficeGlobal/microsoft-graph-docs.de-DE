---
title: Ressourcentyp meetingCapability
description: Enthält die Funktionen einer Besprechung
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 342d264c1f4c670d159c15558c78cc896d4a9487
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931363"
---
# <a name="meetingcapability-resource-type"></a>Ressourcentyp meetingCapability

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Enthält die Funktionen einer Besprechung

## <a name="properties"></a>Eigenschaften

| Eigenschaft                          | Typ    | Beschreibung                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| allowAnonymousUsersToDialOut      | Boolescher Wert | Gibt an, ob anonyme Benutzer als Client-Anschluss in einer Besprechung zulässig ist. |
| allowAnonymousUsersToStartMeeting | Boolescher Wert | Gibt an, ob anonyme Benutzer zugelassen sind, um eine Besprechung zu starten.  |
| autoAdmittedUsers                 | String  | Mögliche Werte: `everyoneInCompany`, `everyone`.              |

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
  "allowAnonymousUsersToStartMeeting": true,
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
