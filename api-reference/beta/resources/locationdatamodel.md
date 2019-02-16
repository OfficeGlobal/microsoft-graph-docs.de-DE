---
title: locationDataModel-Ressourcentyp
description: Stellt locationDataModel-Informationen eines Ereignisses dar.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 2b1fd0c25cdd41e6a8d9c87f8a1c0c80d70b78e5
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057379"
---
# <a name="locationdatamodel-resource-type"></a>locationDataModel-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt Standortinformationen für eine Besprechung dar.


## <a name="properties"></a>Eigenschaften
| Eigenschaft  | Typ   | Beschreibung                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| address | [postalAddress](postaladdress.md) |Die Adresse des Orts. |
| Koordinaten | [outlookGeoCoordinates](outlookgeocoordinates.md) | Die geografischen Koordinaten und die Erhebung des Orts. |
| displayName  | String | Der Name, der mit dem Ort verknüpft ist                       |
| locationEmailAddress | String | Optionale E-Mail-Adresse des Orts. |
| locationUri | String | Optionaler URI, der den Ort darstellt. |


## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationDataModel"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string"
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationdatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
