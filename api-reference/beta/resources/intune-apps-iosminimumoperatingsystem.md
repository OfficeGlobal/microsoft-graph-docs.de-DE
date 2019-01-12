---
title: iosMinimumOperatingSystem-Ressourcentyp
description: Enthält die Eigenschaften des für eine mobile iOS-App mindestens erforderlichen Betriebssystems.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: acee063da4c37627027bce2133201943a9194376
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918938"
---
# <a name="iosminimumoperatingsystem-resource-type"></a>iosMinimumOperatingSystem-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält die Eigenschaften des für eine mobile iOS-App mindestens erforderlichen Betriebssystems.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|v8_0|Boolescher Wert|Version 8.0 oder höher|
|v9_0|Boolescher Wert|Version 9.0 oder höher|
|v10_0|Boolescher Wert|Version 10.0 oder höher|
|v11_0|Boolescher Wert|Version 11.0 oder höher|
|v12_0|Boolescher Wert|Version 12.0 oder höher.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```





