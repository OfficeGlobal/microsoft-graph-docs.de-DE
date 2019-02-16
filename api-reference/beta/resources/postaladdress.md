---
title: postalAddress-Ressourcentyp
description: Stellt die Adresse einer Ressource, z. B. eines Kontakts oder Ereignisses, dar.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7d168e4f53dbd182e4dbd93d0a5b6342daf3339d
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057377"
---
# <a name="postaladdress-resource-type"></a>postalAddress-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt die Straßenadresse eines Standorts dar.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|city|String|Der Ort.|
|countryOrRegion|String|Land oder Region Ein frei formatierbarer Zeichenfolgenwert, z. B. Vereinigte Staaten.|
|isInferred|Boolescher Wert|Nur für internen Gebrauch.|
|postalCode|String|Die Postleitzahl.|
|state|String|Das Land.|
|street|String|Die Straße.|
|type|addressType|Der Adresstyp. Die möglichen Werte sind: `unknown`, `home`, `business`, `other`.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.postalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "isInferred": "boolean",
  "postalCode": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "postaladdress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/postaladdress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
