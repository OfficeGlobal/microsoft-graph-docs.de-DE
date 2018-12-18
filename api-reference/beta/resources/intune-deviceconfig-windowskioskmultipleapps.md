---
title: Ressourcentyp windowsKioskMultipleApps
description: Die Klasse verwendet, um die Konfiguration der Multi-Mode app für die Kiosk-Konfiguration identifizieren
author: tfitzmac
ms.openlocfilehash: 30591e15d29b06ffb807c8b435d0e3c8a6a1b0fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330142"
---
# <a name="windowskioskmultipleapps-resource-type"></a>Ressourcentyp windowsKioskMultipleApps

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Klasse verwendet, um die Konfiguration der Multi-Mode app für die Kiosk-Konfiguration identifizieren

Erbt vom [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Apps|[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) -Auflistung|Dies sind die einzige Windows Store-Apps, die über das Startmenü gestartet werden.|
|showTaskBar|Boolesch|Mit dieser Einstellung kann den Administrator an, ob der Taskleiste oder nicht angezeigt wird.|
|disallowDesktopApps|Boolesch|Diese Einstellung gibt an, dass desktop-apps zulässig sind. Standardmäßig auf "true".|
|startMenuLayoutXml|Binär|Ermöglicht Administratoren das Standardlayout Start außer Kraft gesetzt, und verhindert, dass den Benutzer geändert wird.Das Layout wird durch Angabe einer XML-Datei geändert, die auf einem Layoutänderungsschema basiert. XML muss im Binärformat sein.|

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





