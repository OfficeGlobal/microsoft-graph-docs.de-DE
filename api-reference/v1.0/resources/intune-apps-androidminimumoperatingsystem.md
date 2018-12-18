---
title: androidMinimumOperatingSystem-Ressourcentyp
description: Enthält die Eigenschaften des für eine mobile Android-App mindestens erforderlichen Betriebssystems.
author: tfitzmac
ms.openlocfilehash: 3c477a624377febe6001b92f6694fe27b0666cf5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350470"
---
# <a name="androidminimumoperatingsystem-resource-type"></a>androidMinimumOperatingSystem-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält die Eigenschaften des für eine mobile Android-App mindestens erforderlichen Betriebssystems.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|v4_0|Boolescher Wert|Version 4.0 oder höher|
|v4_0_3|Boolescher Wert|Version 4.0.3 oder höher|
|v4_1|Boolescher Wert|Version 4.1 oder höher|
|v4_2|Boolescher Wert|Version 4.2 oder höher|
|v4_3|Boolescher Wert|Version 4.3 oder höher|
|v4_4|Boolescher Wert|Version 4.4 oder höher|
|v5_0|Boolescher Wert|Version 5.0 oder höher|
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



