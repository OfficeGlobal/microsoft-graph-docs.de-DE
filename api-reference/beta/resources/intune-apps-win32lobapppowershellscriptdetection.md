---
title: Ressourcentyp win32LobAppPowerShellScriptDetection
description: Enthält Eigenschaften, die PowerShell-Skript zum Erkennen von einer Win32-App
author: tfitzmac
ms.openlocfilehash: 7f69b2c066ae90cfcd805b3d3cfe57193046d440
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327573"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a>Ressourcentyp win32LobAppPowerShellScriptDetection

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften, die PowerShell-Skript zum Erkennen von einer Win32-App

Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|enforceSignatureCheck|Boolesch|Ein Wert, der angibt, ob die Signatur Kontrollkästchen erzwungen wird|
|runAs32Bit|Boolesch|Ein Wert, der angibt, ob dieses Skript als 32-Bit ausgeführt werden soll|
|scriptContent|String|Die base64-codierten Skriptinhalt zum Erkennen von Win32 Line of Business (LoB)-app|

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





