---
title: Ressourcentyp tokenMeetingInfo
description: Der Typ des TokenMeetingInfo.
author: VinodRavichandran
ms.openlocfilehash: 6fa66fef6f401db848a9ed3e92c5a1003a5294b6
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380548"
---
# <a name="tokenmeetinginfo-resource-type"></a>Ressourcentyp tokenMeetingInfo

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Der Typ des TokenMeetingInfo.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                     | Typ    | Beschreibung                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| allowConversationWithoutHost | Boolescher Wert | Gibt an, ob eine Unterhaltung fortgesetzt werden kann, sobald der Host der Unterhaltung verlässt. |
| token                        | String  | Das Token an der Besprechung teilnehmen/aktivieren.                                        |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a>Beispiel

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "ABCD123"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
