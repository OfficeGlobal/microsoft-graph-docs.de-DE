---
title: deliveryOptimizationBandwidthBusinessHoursLimit-Ressourcentyp
description: Bandbreiten-und prozentuale Geschäftszeiten
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba15df46075e5cbea1a2eab8a798c333f4a60ae6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178115"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a>deliveryOptimizationBandwidthBusinessHoursLimit-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Bandbreiten-und prozentuale Geschäftszeiten

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|bandwidthBeginBusinessHours|Int32|Gibt den Beginn der Geschäftszeiten mit einer 24-Stunden-Uhr an (0-23). Gültige Werte 0 bis 23|
|bandwidthEndBusinessHours|Int32|Gibt das Ende der Geschäftszeiten in einem 24-Stunden-Format an (0-23). Gültige Werte 0 bis 23|
|bandwidthPercentageDuringBusinessHours|Int32|Gibt den Prozentsatz der Bandbreite an, der während der Geschäftszeiten begrenzt werden soll (0-100). Gültige Werte: 0 bis 100.|
|bandwidthPercentageOutsideBusinessHours|Int32|Gibt den Prozentsatz der Bandbreite an, um die Geschäftszeiten für SIDs zu begrenzen (0-100). Gültige Werte: 0 bis 100.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
  "bandwidthBeginBusinessHours": 1024,
  "bandwidthEndBusinessHours": 1024,
  "bandwidthPercentageDuringBusinessHours": 1024,
  "bandwidthPercentageOutsideBusinessHours": 1024
}
```




