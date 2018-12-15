---
title: Ressourcentyp physicalOfficeAddress
description: Geschäftsadresse einer Ressource wie einen Kontakt oder eine Ereignis darstellt.
ms.openlocfilehash: 472e4dfd03670f5fd4ff6b5c5c53342fff5c391a
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2018
ms.locfileid: "27284098"
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
