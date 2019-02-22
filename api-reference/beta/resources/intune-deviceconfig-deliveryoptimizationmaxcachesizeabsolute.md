---
title: deliveryOptimizationMaxCacheSizeAbsolute-Ressourcentyp
description: Verteilungs Optimierung maximale Cachegröße.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e1ff180136804d6a98e2ebbb292acc358d908d6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178129"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a>deliveryOptimizationMaxCacheSizeAbsolute-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Verteilungs Optimierung maximale Cachegröße.


Erbt von [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|maximumCacheSizeInGigabytes|Int64|Gibt die maximale Größe des Caches für die Verteilungs Optimierung in GB an. Gültige Werte 0 bis 4294967295
Der Wert 0 (null) steht für "unbegrenzten" Cache. Durch die BereitstellungsOptimierung wird der Cache gelöscht, wenn auf dem Gerät wenig Speicherplatz zur Verfügung steht. Gültige Werte 0 bis 4294967295|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute",
  "maximumCacheSizeInGigabytes": 1024
}
```




