---
title: Ressourcentyp windowsKioskDesktopApp
description: Die Basisklasse für einen Typ von apps
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a9b808bfd67e1b14e0b11fe84da48b77b4d965ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947330"
---
# <a name="windowskioskdesktopapp-resource-type"></a>Ressourcentyp windowsKioskDesktopApp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Basisklasse für einen Typ von apps

Erbt vom [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|Die app-Kachelgröße für die Start-Layout Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Mögliche Werte sind: `hidden`, `small`, `medium`, `wide` und `large`.|
|name|Zeichenfolge|Stellt den Anzeigenamen einer App Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) dar.|
|Pfad|Zeichenfolge|Definieren Sie den Pfad einer desktop-App|
|desktopApplicationId|Zeichenfolge|Definieren der DesktopApplicationID der app|
|desktopApplicationLinkPath|Zeichenfolge|Definieren der DesktopApplicationLinkPath der app|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```





