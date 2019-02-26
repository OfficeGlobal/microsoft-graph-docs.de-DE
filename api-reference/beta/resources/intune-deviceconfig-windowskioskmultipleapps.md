---
title: windowsKioskMultipleApps-Ressourcentyp
description: Die Klasse, die zum Identifizieren der multiMode-App-Konfiguration für die Kiosk Konfiguration verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2d2ff38e3b07920f474d9e3894bbd1f8855e277
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162020"
---
# <a name="windowskioskmultipleapps-resource-type"></a>windowsKioskMultipleApps-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Klasse, die zum Identifizieren der multiMode-App-Konfiguration für die Kiosk Konfiguration verwendet wird.


Erbt von [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|apps|[zum](../resources/intune-deviceconfig-windowskioskappbase.md) -Sammlung|Dies sind die einzigen Windows Store-Apps, die über das Startmenü zur Verfügung stehen. Diese Auflistung kann maximal 128 Elemente enthalten.|
|showTaskBar|Boolean|Mit dieser Einstellung kann der Administrator angeben, ob die Vorgangsleiste angezeigt wird.|
|disallowDesktopApps|Boolean|Diese Einstellung gibt an, dass Desktop-Apps zulässig sind. Standardwert true.|
|startMenuLayoutXml|Binär|Ermöglicht Administratoren das außer Kraft setzen des Standard Start Layouts und hindert den Benutzer daran, es zu ändern.Das Layout wird durch Angabe einer XML-Datei geändert, die auf einem Layoutänderungsschema basiert. XML muss im Binärformat vorliegen.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskMultipleApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskMultipleApps",
  "apps": [
    {
      "@odata.type": "microsoft.graph.windowsKioskUWPApp",
      "startLayoutTileSize": "String",
      "name": "String",
      "appType": "String",
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```




