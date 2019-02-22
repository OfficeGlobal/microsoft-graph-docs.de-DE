---
title: deviceGeoLocation-Ressourcentyp
description: Standort des Geräts
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1eaa46929ae627dbf6cdee8d300b7910b4817ffc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149602"
---
# <a name="devicegeolocation-resource-type"></a>deviceGeoLocation-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Standort des Geräts

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|lastCollectedDateTimeUtc|DateTimeOffset|Zeit der Aufzeichnung des Standorts, relativ zu UTC|
|lastCollectedDateTime|DateTimeOffset|Zeit der Aufzeichnung des Standorts, relativ zu UTC|
|longitude|Gleitkommawert mit doppelter Genauigkeit|Längengrad-Koordinate des Gerätestandorts|
|latitude|Gleitkommawert mit doppelter Genauigkeit|Breitengrad-Koordinate des Gerätestandorts|
|altitude|Gleitkommawert mit doppelter Genauigkeit|Höhe in Metern über dem Meeresspiegel|
|horizontalAccuracy|Gleitkommawert mit doppelter Genauigkeit|Genauigkeit von Länge und Breite in Metern|
|verticalAccuracy|Gleitkommawert mit doppelter Genauigkeit|Genauigkeit der Höhe in Metern|
|heading|Gleitkommawert mit doppelter Genauigkeit|Kurs in Grad vom geografischen Norden|
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
  "lastCollectedDateTimeUtc": "String (timestamp)",
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




