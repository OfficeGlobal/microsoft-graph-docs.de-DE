---
title: Ressourcentyp macOSMinimumOperatingSystem
description: Das Betriebssystem (mindestens) für eine Mac OS-app erforderlich.
author: tfitzmac
ms.openlocfilehash: ff9d4e3fc375f17d7b3c3efdd4af16cd7e87ceb6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354775"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>Ressourcentyp macOSMinimumOperatingSystem

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Das Betriebssystem (mindestens) für eine Mac OS-app erforderlich.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|v10_7|Boolesch|Mac OS 10,7 oder höher.|
|v10_8|Boolesch|Mac OS 10,8 oder höher.|
|v10_9|Boolesch|Mac OS 10.9 oder höher.|
|v10_10|Boolesch|Mac OS 10.10 oder höher.|
|v10_11|Boolesch|Mac OS 10.11 oder höher.|
|v10_12|Boolesch|Mac OS 10.12 oder höher.|
|v10_13|Boolesch|Mac OS 10.13 oder höher.|

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





