---
title: physicalAddress-Ressourcentyp
description: Stellt die Adresse einer Ressource, z. B. eines Kontakts oder Ereignisses, dar.
localization_priority: Normal
ms.openlocfilehash: 3a656046cc23394fc8cff9100eb5ad2289050b25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823583"
---
# <a name="physicaladdress-resource-type"></a>physicalAddress-Ressourcentyp

Stellt die Adresse einer Ressource, z. B. eines Kontakts oder Ereignisses, dar.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|type|Zeichenfolge|Die Art der Adresse. Mögliche Werte: sind `unknown`, `home`, `business` und `other`.|
|postOfficeBox|Zeichenfolge|Die Postfachnummer.|
|Ort|Zeichenfolge|Der Ort.|
|countryOrRegion|Zeichenfolge|Land oder Region Ein frei formatierbarer Zeichenfolgenwert, z. B. Vereinigte Staaten.|
|postalCode|Zeichenfolge|Die Postleitzahl.|
|state|Zeichenfolge|Das Land.|
|street|Zeichenfolge|Die Straße.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "type": "string",
  "postOfficeBox": "string",
  "city": "string",
  "countryOrRegion": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
