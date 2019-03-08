---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Shared
localization_priority: Normal
ms.openlocfilehash: af426d5e51f87b9fd8894c6e956947cc75f1a38d
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481797"
---
# <a name="shared-resource-type"></a>Shared-Ressourcentyp

Die **Shared**-Ressourcenart gibt an, dass ein DriveItem für andere Personen freigegeben wurde. Die Ressource enthält Informationen darüber, wie das Element freigegeben wird.

Wenn ein [**DriveItem**](driveitem.md) ein **shared**-Facet ungleich Null aufweist, wurde das Element freigegeben.

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared",
  "optionalProperties": [ "sharedBy", "sharedDateTime" ]
}-->

```json
{
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "scope": "anonymous | organization | users",
  "sharedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "sharedDateTime": "datetime"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ                          | Beschreibung
| :------------- |:------------------------------|:----------------------------
| owner          | [IdentitySet](identityset.md) | Die Identität der der Besitzer des freigegebenen Elements. Schreibgeschützt.
| scope          | String                        | Gibt den Bereich der Freigabe des Elements an: `anonymous`, `organization` oder `users`. Schreibgeschützt.
| sharedBy       | [identitySet](identityset.md) | Die Identität des Benutzers, der das Element freigegeben hat. Schreibgeschützt.
| sharedDateTime | DateTimeOffset                | UTC-Datum und -Uhrzeit der Elementfreigabe. Schreibgeschützt.

## <a name="scope-options"></a>Bereichsoptionen

| Wert          | Beschreibung                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für jede Person mit der Link funktioniert.               |
| `organization` | Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für Organisation des Besitzers funktioniert. |
| `users`        | Das Element wird nur für bestimmte Benutzern freigegeben.                                          |

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets einer **driveItem**-Ressource finden Sie unter [**driveItem**](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/shared.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization,users) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Shared"
} -->
