---
title: Ressourcentyp educationOneNoteResource
description: 'Eine Unterklasse der EducationResource. Dies ist den Speicherort der OneNote-Seite.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 60b0e4647f1a601d3cbe206e264f7d288ee2110c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521418"
---
# <a name="educationonenoteresource-resource-type"></a>Ressourcentyp educationOneNoteResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Unterklasse der [EducationResource](educationresource.md). Dies ist den Speicherort der OneNote-Seite.  

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|pageUrl|String|Die Microsoft Graph-URL zu der Seite in OneNote.|
|sectionName|String|Im Abschnittsname, die Verteilung in kopiert werden sollte oder in kopiert wurden.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationonenoteresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
