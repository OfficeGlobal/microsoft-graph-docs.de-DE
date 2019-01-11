---
title: Ressourcentyp windowsKioskAppBase
description: Die Basisklasse für einen Typ von apps
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fa83243959105b09707fa28a53271d8f95c5fd1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845157"
---
# <a name="windowskioskappbase-resource-type"></a>Ressourcentyp windowsKioskAppBase

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Basisklasse für einen Typ von apps
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|Die app-Kachelgröße für das Layout Start. Mögliche Werte sind: `hidden`, `small`, `medium`, `wide` und `large`.|
|name|String|Stellt den Anzeigenamen einer App|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String"
}
```





