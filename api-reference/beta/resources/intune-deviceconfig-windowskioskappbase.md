---
title: Zum-Ressourcentyp
description: Die Basisklasse für eine Art von apps
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b86921fcdaa11b37b985184dfbc645c2a193bfdb
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572306"
---
# <a name="windowskioskappbase-resource-type"></a>Zum-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Basisklasse für eine Art von apps

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|Die Größe der APP-Kachel für das Start Layout. Mögliche Werte: `hidden`, `small`, `medium`, `wide`, `large`.|
|name|String|Stellt den Anzeigenamen einer APP dar.|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|Der APP-Typ. Mögliche Werte sind: `unknown`, `store`, `desktop` und `aumId`.|
|Autostart|Boolesch|Automatisches Starten der APP im Multi-App Kiosk-Modus|

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
  "name": "String",
  "appType": "String",
  "autoLaunch": true
}
```




