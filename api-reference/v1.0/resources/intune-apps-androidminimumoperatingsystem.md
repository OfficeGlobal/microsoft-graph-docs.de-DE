---
title: androidMinimumOperatingSystem-Ressourcentyp
description: Enthält die Eigenschaften des für eine mobile Android-App mindestens erforderlichen Betriebssystems.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2402ad007b794e7d6824e52cce8ff7144c6c33b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264519"
---
# <a name="androidminimumoperatingsystem-resource-type"></a>androidMinimumOperatingSystem-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält die Eigenschaften des für eine mobile Android-App mindestens erforderlichen Betriebssystems.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|v4_0|Boolean|Version 4.0 oder höher|
|v4_0_3|Boolean|Version 4.0.3 oder höher|
|v4_1|Boolean|Version 4.1 oder höher|
|v4_2|Boolean|Version 4.2 oder höher|
|v4_3|Boolean|Version 4.3 oder höher|
|v4_4|Boolean|Version 4.4 oder höher|
|v5_0|Boolean|Version 5.0 oder höher|
|v5_1|Boolescher Wert|Version 5.1 oder höher|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMinimumOperatingSystem",
  "v4_0": true,
  "v4_0_3": true,
  "v4_1": true,
  "v4_2": true,
  "v4_3": true,
  "v4_4": true,
  "v5_0": true,
  "v5_1": true
}
```



