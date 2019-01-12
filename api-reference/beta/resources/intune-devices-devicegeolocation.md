---
title: deviceGeoLocation-Ressourcentyp
description: Standort des Geräts
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ef73925c31b58327f0e0b89d5682035d14d38afc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943099"
---
# <a name="devicegeolocation-resource-type"></a>deviceGeoLocation-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Standort des Geräts
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|lastCollectedDateTimeUtc|DateTimeOffset|Zeit der Aufzeichnung des Standorts, relativ zu UTC|
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





