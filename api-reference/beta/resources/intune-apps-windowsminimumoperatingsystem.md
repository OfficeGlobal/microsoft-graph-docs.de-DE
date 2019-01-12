---
title: windowsMinimumOperatingSystem-Ressourcentyp
description: Das mindestens für eine mobile Windows-App erforderliche Betriebssystem.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cbee999b213d6c4b76a1203ac48b84c8dbeda3c5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914647"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>windowsMinimumOperatingSystem-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Das mindestens für eine mobile Windows-App erforderliche Betriebssystem.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|v8_0|Boolescher Wert|Windows-Version 8.0 oder höher|
|v8_1|Boolescher Wert|Windows-Version 8.1 oder höher|
|v10_0|Boolescher Wert|Windows-Version 10.0 oder höher|
|v10_1607|Boolescher Wert|Windows 1607 10 oder höher.|
|v10_1703|Boolescher Wert|Windows 1703 10 oder höher.|
|v10_1709|Boolescher Wert|Windows 1709 10 oder höher.|
|v10_1803|Boolescher Wert|Windows 1803 10 oder höher.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true,
  "v10_1607": true,
  "v10_1703": true,
  "v10_1709": true,
  "v10_1803": true
}
```





