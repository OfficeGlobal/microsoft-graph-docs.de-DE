---
title: windowsKioskDesktopApp-Ressourcentyp
description: Die Basisklasse für eine Art von apps
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0487fa24ecd2d27817349b68063cf606a2401944
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170476"
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
|name|Zeichenfolge|Stellt den Anzeigenamen einer von [zum](../resources/intune-deviceconfig-windowskioskappbase.md) geerbten App dar.|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|Der von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)geerbte App-Typ. Mögliche Werte: `unknown`, `store`, `desktop`, `aumId`.|
|Pfad|Zeichenfolge|Definieren des Pfads einer Desktop-App|
|desktopApplicationId|Zeichenfolge|Definieren der DesktopApplicationID der APP|
|desktopApplicationLinkPath|Zeichenfolge|Definieren der DesktopApplicationLinkPath der APP|

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
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




