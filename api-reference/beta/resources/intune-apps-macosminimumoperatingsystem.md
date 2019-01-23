---
title: Ressourcentyp macOSMinimumOperatingSystem
description: Das Betriebssystem (mindestens) für eine Mac OS-app erforderlich.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1b5bb3c31f876cb7444ff90cad5060c08d2f60b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425925"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>Ressourcentyp macOSMinimumOperatingSystem

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Das Betriebssystem (mindestens) für eine Mac OS-app erforderlich.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|v10_7|Boolean|Mac OS 10,7 oder höher.|
|v10_8|Boolean|Mac OS 10,8 oder höher.|
|v10_9|Boolean|Mac OS 10.9 oder höher.|
|v10_10|Boolean|Mac OS 10.10 oder höher.|
|v10_11|Boolean|Mac OS 10.11 oder höher.|
|v10_12|Boolean|Mac OS 10.12 oder höher.|
|v10_13|Boolean|Mac OS 10.13 oder höher.|

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




