---
title: licenseUnitsDetail-Ressourcentyp
description: Die prepaidUnits-Eigenschaft der subscribedSku-Entität ist vom Typ licenseUnitsDetail.
localization_priority: Normal
ms.openlocfilehash: a5eacb79dfca97b992e2f8584761aaa45beccd76
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511317"
---
# <a name="licenseunitsdetail-resource-type"></a>licenseUnitsDetail-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **prepaidUnits**-Eigenschaft der [subscribedSku](subscribedsku.md)-Entität ist vom Typ **licenseUnitsDetail**.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:-------------|:-----|:----------|
|aktiviert|Int32| Die Anzahl der Einheiten, die aktiviert werden. |
|suspended|Int32| Die Anzahl der Einheiten, die angehalten werden. |
|warning|Int32| Die Anzahl der Einheiten, für die eine Warnung vorliegt. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseunitsdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
