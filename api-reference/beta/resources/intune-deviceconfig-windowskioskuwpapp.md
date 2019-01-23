---
title: Ressourcentyp windowsKioskUWPApp
description: Die Basisklasse für einen Typ von apps
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ba5367721890f02af3b348ad469b15024de4800
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392682"
---
# <a name="windowskioskuwpapp-resource-type"></a>Ressourcentyp windowsKioskUWPApp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Die Basisklasse für einen Typ von apps


Erbt vom [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|Die app-Kachelgröße für die Start-Layout Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Mögliche Werte sind: `hidden`, `small`, `medium`, `wide` und `large`.|
|name|Zeichenfolge|Stellt den Anzeigenamen einer App Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) dar.|
|der appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|Der app-Typ Inherited aus [WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md). Mögliche Werte: sind `unknown`, `store`, `desktop` und `aumId`.|
|appUserModelId|Zeichenfolge|Dies ist die einzige Anwendung Benutzer Modell ID (AUMID), die Verwendung im Kioskmodus gestartet werden|
|appId|Zeichenfolge|Dies verweist auf eine Intune-App, die Ziel ein, um dieselben Zuweisungen als Kiosk-Konfiguration werden|
|containedAppId|Zeichenfolge|Dies wird auf einer enthaltenen App aus einer Intune App|

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




