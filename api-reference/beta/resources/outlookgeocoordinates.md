---
title: outlookGeoCoordinates-Ressourcentyp
description: Die geografischen Koordinaten, die Erhebung und deren Genauigkeitsgrad für einen physischen Ort.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ca63aa3df6a597aaacb81fbeacf275ac87064f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511835"
---
# <a name="outlookgeocoordinates-resource-type"></a>outlookGeoCoordinates-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die geografischen Koordinaten, die Erhebung und deren Genauigkeitsgrad für einen physischen Ort.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|accuracy|double|Die Genauigkeit des Breiten- und Längengrads. Die Genauigkeit kann beispielsweise in Metern gemessen werden, der Breiten- und Längengrad sind beispielsweise auf 50 Meter genau.|
|altitude|double|Die Höhe des Orts.|
|altitudeAccuracy|double|Die Genauigkeit der Höhe.|
|latitude|double|Der Breitengrad des Orts.|
|longitude|double|Der Längengrad des Orts.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookgeocoordinates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
