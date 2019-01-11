---
title: Ressourcentyp physicalOfficeAddress
description: Geschäftsadresse einer Ressource wie einen Kontakt oder eine Ereignis darstellt.
localization_priority: Normal
ms.openlocfilehash: bd4274e29b2ef0f9e7e8318528d18103be19fabc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817787"
---
# <a name="physicalofficeaddress-resource-type"></a>Ressourcentyp physicalOfficeAddress

Geschäftsadresse einer Ressource wie eine Organisationseinheit Kontakt darstellt.

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|city|String|Der Ort.|
|countryOrRegion|String|Land oder Region Ein frei formatierbarer Zeichenfolgenwert, z. B. Vereinigte Staaten.|
|officeLocation  | String | Standort des Büros wie Gebäude und Office Anzahl für eine Organisationseinheit Kontakt.  |
|postalCode|String|Die Postleitzahl.|
|state|String|Das Land.|
|street|String|Die Straße.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
