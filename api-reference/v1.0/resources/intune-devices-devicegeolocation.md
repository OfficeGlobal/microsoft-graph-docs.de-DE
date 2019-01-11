---
title: deviceGeoLocation-Ressourcentyp
description: Standort des Geräts
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 68e89b2e63b99324332874a3ad6a2f2e3c335832
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816128"
---
# <a name="devicegeolocation-resource-type"></a>deviceGeoLocation-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Standort des Geräts
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|lastCollectedDateTime|DateTimeOffset|Zeit der Aufzeichnung des Standorts, relativ zu UTC|
|longitude|Double|Längengrad-Koordinate des Gerätestandorts|
|latitude|Double|Breitengrad-Koordinate des Gerätestandorts|
|altitude|Double|Höhe in Metern über dem Meeresspiegel|
|horizontalAccuracy|Double|Genauigkeit von Länge und Breite in Metern|
|verticalAccuracy|Double|Genauigkeit der Höhe in Metern|
|heading|Double|Kurs in Grad vom geografischen Norden|
|speed|Double|Geschwindigkeit der Bewegung des Geräts in Metern pro Sekunde|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```



