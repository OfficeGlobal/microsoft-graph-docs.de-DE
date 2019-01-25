---
title: Ressourcentyp educationOrganization
description: 'Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 122717952781cd8effe415fb01b07ec9bf71143d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507474"
---
# <a name="educationorganization-resource-type"></a>Ressourcentyp educationOrganization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Abstrakte Entität verwendet, um die Kompatibilität zwischen verschiedenen Organisationstypen innerhalb der Education Sektor modellieren.  

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|description|String| Beschreibung der Organisation.|
|displayName|String| Anzeigename der Organisation.|
|externalSource|string| Quelle, wo diese Organisation erstellt wurde. Mögliche Werte sind: `sis`, `manual` und `unknownFutureValue`.|

## <a name="relationships"></a>Beziehungen
Keine.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationorganization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
