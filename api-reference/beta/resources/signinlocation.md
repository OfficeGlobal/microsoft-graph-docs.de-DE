---
title: Ressourcentyp signInLocation
description: Enthält den Ort, Bundesland und Land/Region aus, in dem die Anmeldung bei der.
ms.openlocfilehash: a3d4f6ca5ec18e70960f45a3da1bb06d51ee1e65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062240"
---
# <a name="signinlocation-resource-type"></a>Ressourcentyp signInLocation
Enthält den Ort, Bundesland und Land/Region aus, in dem die Anmeldung bei der.



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|city|String|Enthält den Ort, von dem die Anmeldung stammt. Dadurch wird die anhand von Informationen aus der Aktivität Anmeldung Breitengrad/Längengrad berechnet.|
|countryOrRegion|String|Enthält das Land Code Info (2 Buchstaben Code), von dem die Anmeldung stammt.  Dadurch wird die anhand von Informationen aus der Aktivität Anmeldung Breitengrad/Längengrad berechnet.|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|Enthält die Breitengrad, Längengrad und Höhe, von dem die Anmeldung stammt.|
|state|String|Enthält den Status, in dem die Anmeldung ausgelöst hat. Dadurch wird die anhand von Informationen aus der Aktivität Anmeldung Breitengrad/Längengrad berechnet.|

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