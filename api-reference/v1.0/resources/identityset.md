---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: 369068dd48b9173032542303e3fd9831d25e6e9e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480292"
---
# <a name="identityset-resource-type"></a>IdentitySet-Ressourcentyp

Die **IdentitySet**-Ressource ist eine verschlüsselte Sammlung von [identity](identity.md)-Ressourcen. Sie wird verwendet, um eine Reihe von Identitäten darzustellen, die verschiedenen Ereignissen für ein Element zugewiesen sind, z. B. _erstellt von_ oder _zuletzt geändert von_.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identitySet",
       "optionalProperties": ["user", "application", "device"],
       "openType": true } -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft    | Typ                    | Beschreibung                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| Anwendung | [Identity](identity.md) | Optional. Die mit dieser Aktion verknüpfte Anwendung. |
| Gerät      | [Identity](identity.md) | Optional. Das mit dieser Konfiguration verknüpfte Gerät.      |
| Benutzer        | [Identity](identity.md) | Optional. Der mit dieser Aktion verknüpfte Benutzer.        |

## <a name="remarks"></a>Bemerkungen 

Informationen zur Verwendung von [IdentitySet](driveitem.md)-Ressourcen finden Sie unter **DriveItem**.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
