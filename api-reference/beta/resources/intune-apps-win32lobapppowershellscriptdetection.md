---
title: win32LobAppPowerShellScriptDetection-Ressourcentyp
description: Enthält PowerShell-Skripteigenschaften zum Auffinden einer Win32-App
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa5452fd9e73aef846d0b6de86a2b84e2c42ba26
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168523"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a>win32LobAppPowerShellScriptDetection-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält PowerShell-Skripteigenschaften zum Auffinden einer Win32-App


Erbt von [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|enforceSignatureCheck|Boolescher Wert|Ein Wert, der angibt, ob die Signaturüberprüfung erzwungen wird.|
|runAs32Bit|Boolescher Wert|Ein Wert, der angibt, ob dieses Skript als 32-Bit ausgeführt werden soll|
|scriptContent|Zeichenfolge|Der Base64-codierte Skriptinhalt zum Aufspüren der Win32-Branchen-App|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptDetection",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String"
}
```




