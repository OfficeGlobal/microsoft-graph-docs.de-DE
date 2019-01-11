---
title: Ressourcentyp signInLocation
description: Enthält den Ort, Bundesland und Land/Region aus, in dem die Anmeldung bei der.
localization_priority: Normal
ms.openlocfilehash: 49d6dfb07c635ac3754b3e873d75911a43593a73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839137"
---
# <a name="signinlocation-resource-type"></a>Ressourcentyp signInLocation
Enthält den Ort, Bundesland und Land/Region aus, in dem die Anmeldung bei der.



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|city|Zeichenfolge|Enthält den Ort, von dem die Anmeldung stammt. Dadurch wird die anhand von Informationen aus der Aktivität Anmeldung Breitengrad/Längengrad berechnet.|
|countryOrRegion|Zeichenfolge|Enthält das Land Code Info (2 Buchstaben Code), von dem die Anmeldung stammt.  Dadurch wird die anhand von Informationen aus der Aktivität Anmeldung Breitengrad/Längengrad berechnet.|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|Enthält die Breitengrad, Längengrad und Höhe, von dem die Anmeldung stammt.|
|state|Zeichenfolge|Enthält den Status, in dem die Anmeldung ausgelöst hat. Dadurch wird die anhand von Informationen aus der Aktivität Anmeldung Breitengrad/Längengrad berechnet.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInLocation"
}-->

```json
{
  "city": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.geoCoordinates"},
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
