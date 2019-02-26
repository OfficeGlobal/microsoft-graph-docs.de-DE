---
title: windowsKioskUWPApp-Ressourcentyp
description: Die Basisklasse für eine Art von apps
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1dbaf8dfd7f2cd488de37378f934ca3f31daedd6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147327"
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
|name|Zeichenfolge|Stellt den Anzeigenamen einer von [zum](../resources/intune-deviceconfig-windowskioskappbase.md) geerbten App dar.|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|Der von [zum](../resources/intune-deviceconfig-windowskioskappbase.md)geerbte App-Typ. Mögliche Werte: `unknown`, `store`, `desktop`, `aumId`.|
|appUserModelId|Zeichenfolge|Dies ist die einzige Anwendungsbenutzer Modell-ID (AUMID), die im Kiosk-Modus verwendet werden kann.|
|appId|Zeichenfolge|Dies verweist auf eine InTune-APP, die auf die gleichen Zuordnungen wie die Kiosk Konfiguration ausgerichtet sein wird.|
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
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```




