---
title: Allgemeiner Fehler Ressourcentyp
description: Ein allgemeiner Fehler.
localization_priority: Normal
ms.openlocfilehash: d3c7e9cd7ff7be635adfbf329170068cd944f0b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524128"
---
# <a name="genericerror-resource-type"></a>Allgemeiner Fehler Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein allgemeiner Fehler.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------|:-----|:------------|
| message | String | Die Fehlermeldung. |
| code | String | Der Fehlercode. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/genericerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
