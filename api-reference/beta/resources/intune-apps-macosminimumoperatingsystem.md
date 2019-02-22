---
title: macOSMinimumOperatingSystem-Ressourcentyp
description: Das minimale Betriebssystem, das für eine MacOS-App erforderlich ist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f6975690361c981d6b5aaf1d9dae959ad6f8be5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169937"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>macOSMinimumOperatingSystem-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Das minimale Betriebssystem, das für eine MacOS-App erforderlich ist.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|v10_7|Boolescher Wert|Mac OS 10,7 oder höher.|
|v10_8|Boolescher Wert|Mac OS 10,8 oder höher.|
|v10_9|Boolescher Wert|Mac OS 10,9 oder höher.|
|v10_10|Boolescher Wert|Mac OS 10,10 oder höher.|
|v10_11|Boolescher Wert|Mac OS 10,11 oder höher.|
|v10_12|Boolescher Wert|Mac OS 10,12 oder höher.|
|v10_13|Boolescher Wert|Mac OS 10,13 oder höher.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSMinimumOperatingSystem",
  "v10_7": true,
  "v10_8": true,
  "v10_9": true,
  "v10_10": true,
  "v10_11": true,
  "v10_12": true,
  "v10_13": true
}
```




