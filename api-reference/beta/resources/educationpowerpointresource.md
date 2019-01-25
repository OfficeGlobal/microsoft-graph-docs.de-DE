---
title: Ressourcentyp educationPowerPointResource
description: 'Eine Unterklasse der EducationResource. Hierbei handelt es sich um eine PowerPoint-Ressource. PowerPoint-Datei muss im Zusammenhang mit **FileResource** Verzeichnis hochgeladen werden die '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: b61f210ce0efde36b83632268e12d18d3b96b661
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512199"
---
# <a name="educationpowerpointresource-resource-type"></a>Ressourcentyp educationPowerPointResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Unterklasse der [EducationResource](educationresource.md). Hierbei handelt es sich um eine PowerPoint-Ressource. PowerPoint-Datei muss im Verzeichnis **FileResource** zugeordnet, die Zuordnung oder die Übermittlung hochgeladen werden.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fileUrl|String|Speicherort der Datei auf dem Datenträger.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerpointresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
