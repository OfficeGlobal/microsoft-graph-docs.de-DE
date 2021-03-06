---
title: Ressourcentyp referencedObject
description: Beschreibt einen Verweis auf ein anderes Objekt in der gleichen Verzeichnis Definition definiert.
localization_priority: Normal
ms.openlocfilehash: dcec232335fdf3d447097ea1ae87fbc9ea676cfe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529320"
---
# <a name="referencedobject-resource-type"></a>Ressourcentyp referencedObject

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Beschreibt einen Verweis auf ein anderes Objekt in der gleichen [Verzeichnis Definition](synchronization-directorydefinition.md)definiert.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                   | Typ                      | Beschreibung    |
|:---------------------------|:--------------------------|:---------------|
|referencedObjectName        |String                     |Name des Objekts verwiesen wird. Muss eines der Objekte in der [Definition des Verzeichnisses](synchronization-directorydefinition.md)übereinstimmen.|
|referencedProperty          |String                     |**Derzeit nicht unterstützt**. Der Name der Eigenschaft in das Objekt verwiesen wird, der, das Wert für die als Referenz verwendet wird.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referencedObject"
}-->

```json
{
  "referencedObjectName": "String",
  "referencedProperty": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-referencedobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
            
