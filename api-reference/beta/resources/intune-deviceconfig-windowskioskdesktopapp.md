---
title: windowsKioskDesktopApp-Ressourcentyp
description: Die Basisklasse für eine Art von apps
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4cccd1b5e7ec7ca16aeb76b87fc31d90e92e7dcd
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30572082"
---
# <a name="windowskioskdesktopapp-resource-type"></a>windowsKioskDesktopApp-Ressourcentyp

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
|Pfad|String|Definieren des Pfads einer Desktop-App|
|desktopApplicationId|String|Definieren der DesktopApplicationID der APP|
|desktopApplicationLinkPath|String|Definieren der DesktopApplicationLinkPath der APP|

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
  "appType": "String",
  "autoLaunch": true,
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




