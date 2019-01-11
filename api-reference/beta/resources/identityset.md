---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: 63178fc9add3d097b7e8aaf0c5c2a697a91eaeed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807021"
---
# <a name="identityset-resource-type"></a>Ressourcentyp identitySet

Die **IdentitySet**-Ressource ist eine verschlüsselte Sammlung von [identity](identity.md)-Ressourcen. Sie wird verwendet, um eine Reihe von Identitäten darzustellen, die verschiedenen Ereignissen für ein Element zugewiesen sind, z. B. _erstellt von_ oder _zuletzt geändert von_.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
    "device",
    "encrypted",
    "guest",
    "phone",
    "user"
  ],
  "openType": true
} -->
```json
{
  "application": {"@odata.type": "#microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "#microsoft.graph.identity"},
  "device": {"@odata.type": "#microsoft.graph.identity"},
  "encrypted": {"@odata.type": "#microsoft.graph.identity"},
  "guest": {"@odata.type": "#microsoft.graph.identity"},
  "phone": {"@odata.type": "#microsoft.graph.identity"},
  "user": {"@odata.type": "#microsoft.graph.identity"}
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft    | Typ                    | Beschreibung                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| Anwendung | [Identity](identity.md) | Optional. Die mit dieser Aktion verknüpfte Anwendung.  |
| Gerät      | [Identity](identity.md) | Optional. Das mit dieser Konfiguration verknüpfte Gerät.       |
| phone       | [identity](identity.md) | Optional. Die Telefonnummer, die diese Aktion zugeordnet. |
| Benutzer        | [Identity](identity.md) | Optional. Der mit dieser Aktion verknüpfte Benutzer.         |

## <a name="remarks"></a>Bemerkungen 

Verwendung der **IdentitySet** Ressourcen finden Sie unter [aufrufen](call.md) .


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
