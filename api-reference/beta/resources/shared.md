---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Shared
localization_priority: Normal
ms.openlocfilehash: 04504b5257dfc49ad14cbee1f645120dc31a3387
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480299"
---
# <a name="shared-resource-type"></a>Shared-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

## <a name="scope-values"></a>Bereichswerte

| Wert          | Beschreibung                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für jede Person mit der Link funktioniert.               |
| `organization` | Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für Organisation des Besitzers funktioniert. |
| `users`        | Das Element wird nur für bestimmte Benutzern freigegeben.                                          |

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets einer **driveItem**-Ressource finden Sie unter [**driveItem**](driveitem.md).

<!--
{
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared",
  "suppressions": [
    "Error: /api-reference/beta/resources/shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
