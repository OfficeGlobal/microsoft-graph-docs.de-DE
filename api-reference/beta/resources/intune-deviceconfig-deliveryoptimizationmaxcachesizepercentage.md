---
title: deliveryOptimizationMaxCacheSizePercentage-Ressourcentyp
description: Maximale Anzahl von Cachegrößen für die Verteilungs Optimierung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7579b95d0adefb09c9312596f4604fe9d5b05548
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177833"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a>deliveryOptimizationMaxCacheSizePercentage-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Maximale Anzahl von Cachegrößen für die Verteilungs Optimierung.


Erbt von [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|maximumCacheSizePercentage|Int32|Gibt die maximale Cachegröße, die von der BereitstellungsOptimierung verwendet werden kann, als Prozentsatz der Datenträgergröße an (1-100). Gültige Werte 1 bis 100|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizePercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizePercentage",
  "maximumCacheSizePercentage": 1024
}
```




