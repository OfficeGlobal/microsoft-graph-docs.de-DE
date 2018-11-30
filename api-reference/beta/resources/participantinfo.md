---
title: Ressourcentyp participantInfo
description: Enthält zusätzliche Eigenschaften über die Teilnehmerliste Identität
ms.openlocfilehash: c6f429e353d80ea53c5f5c00ca084ae7a8a4a7c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058223"
---
# <a name="participantinfo-resource-type"></a>Ressourcentyp participantInfo

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Enthält zusätzliche Eigenschaften über die Teilnehmerliste Identität

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ                          | Beschreibung  |
|:---------------|:------------------------------|:-------------|
| Identität       | [identitySet](identityset.md) | Die [IdentitySet](identityset.md) dieser Teilnehmer zugeordnet. |
| languageId     | String                        | Die Sprache-Kultur-Zeichenfolge. |
| Region         | String                        | Region des Teilnehmers. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->