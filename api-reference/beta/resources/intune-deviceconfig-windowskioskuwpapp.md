---
title: windowsKioskUWPApp-Ressourcentyp
description: Die Basisklasse für eine Art von apps
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a247c3f02dc64657ec9cd297d8fff5d8591549cd
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572537"
---
# <a name="windowskioskuwpapp-resource-type"></a>windowsKioskUWPApp-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Basisklasse für eine Art von apps


Erbt von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|Die Größe der APP-Kachel für das von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)geerbte Start Layout. Mögliche Werte: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|String|Stellt den Anzeigenamen einer von [zum](../resources/intune-deviceconfig-windowskioskappbase.md) geerbten App dar.|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|Der von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)geerbte App-Typ. Mögliche Werte sind: `unknown`, `store`, `desktop` und `aumId`.|
|Autostart|Boolesch|Automatisches Starten der APP im Multi-App Kiosk-Modus, geerbt von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)|
|appUserModelId|Zeichenfolge|Dies ist die einzige Anwendungsbenutzer Modell-ID (AUMID), die im Kiosk-Modus verwendet werden kann.|
|appId|String|Dies verweist auf eine InTune-APP, die auf die gleichen Zuordnungen wie die Kiosk Konfiguration ausgerichtet sein wird.|
|containedAppId|Zeichenfolge|Dieser Verweis auf eine enthaltene App aus einer InTune-App|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```




