---
title: Ressourcentyp mediaInfo
description: Die Medieninformationen für die Aktionen für aufgefordert wird.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 65cf71f5c116fe213d0e32d560ec24704bff1172
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523981"
---
# <a name="mediainfo-resource-type"></a>Ressourcentyp mediaInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die Medieninformationen für die Aktionen für aufgefordert wird.

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    | Beschreibung                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | Zeichenfolge  | Eindeutige Identität der Ressource. |
| uri            | String  | Pfad zu der Ressource.            |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mediainfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
