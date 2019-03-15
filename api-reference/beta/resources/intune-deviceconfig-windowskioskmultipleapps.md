---
title: windowsKioskMultipleApps-Ressourcentyp
description: Die Klasse, die zum Identifizieren der multiMode-App-Konfiguration für die Kiosk Konfiguration verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c657300cf3ca00482b85b7983f28b4df3135c97d
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570843"
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
|showTaskBar|Boolesch|Mit dieser Einstellung kann der Administrator angeben, ob die Vorgangsleiste angezeigt wird.|
|allowAccessToDownloadsFolder|Boolesch|Diese Einstellung ermöglicht den Zugriff auf den Ordner Downloads im Datei-Explorer.|
|disallowDesktopApps|Boolesch|Diese Einstellung gibt an, dass Desktop-Apps zulässig sind. Standardwert true.|
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
      "autoLaunch": true,
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "allowAccessToDownloadsFolder": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```




