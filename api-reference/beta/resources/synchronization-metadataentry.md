---
title: Ressourcentyp metadataEntry
description: Metadaten für das angegebene Objekt.
localization_priority: Normal
ms.openlocfilehash: a6b9170144917e4c7b66bb52c1efb17d93167ef0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511779"
---
# <a name="metadataentry-resource-type"></a>Ressourcentyp metadataEntry

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Metadaten für das angegebene Objekt.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Key|String|Name der Metadateneigenschaft.|
|Wert|Zeichenfolge|Der Wert der Metadateneigenschaft.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-metadataentry.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
