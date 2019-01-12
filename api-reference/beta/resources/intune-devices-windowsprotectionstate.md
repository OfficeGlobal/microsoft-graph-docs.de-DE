---
title: Ressourcentyp windowsProtectionState
description: Gerät Protection Status Entität.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f15044f597fb04e98571de7aec8796e9a9ddf74
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954526"
---
# <a name="windowsprotectionstate-resource-type"></a>Ressourcentyp windowsProtectionState

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Gerät Protection Status Entität.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von windowsProtectionState](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Lesen Sie Eigenschaften und Beziehungen des [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) -Objekts.|
|[WindowsProtectionState aktualisieren](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Aktualisieren Sie die Eigenschaften eines [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Der eindeutige Bezeichner für das Gerät Protection Status-Objekt. Dies ist die Geräte-Id des Geräts|
|malwareProtectionEnabled|Boolescher Wert|Anti-Malware ist oder nicht aktiviert|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Zustand des Computers (wie bereinigen oder ausstehende vollständigen Scan oder Ausstehender Neustart usw.). Mögliche Werte sind: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending` und `critical`.|
|realTimeProtectionEnabled|Boolescher Wert|Echtzeit-Schutz ist oder nicht aktiviert?|
|networkInspectionSystemEnabled|Boolescher Wert|Netzwerk-Prüfung System aktiviert ist oder nicht?|
|quickScanOverdue|Boolescher Wert|Quick scan überfällige oder nicht?|
|fullScanOverdue|Boolescher Wert|Des vollständigen Scan überfällige oder nicht?|
|signatureUpdateOverdue|Boolescher Wert|Signatur veraltet oder nicht?|
|rebootRequired|Boolescher Wert|Neustart erforderlich oder nicht?|
|fullScanRequired|Boolescher Wert|Vollständigen Scan erforderlich oder nicht?|
|%ENGINEVERSION%|Zeichenfolge|Aktuelle Endpoint Protection Datenbankmodul, version|
|signatureVersion|Zeichenfolge|Aktuelle Version der Malware-Definitionen|
|antiMalwareVersion|Zeichenfolge|Aktuelle anti-Malware-version|
|lastQuickScanDateTime|DateTimeOffset|Letzte schnell-Scan datetime|
|lastFullScanDateTime|DateTimeOffset|Letzte schnell-Scan datetime|
|lastQuickScanSignatureVersion|Zeichenfolge|Letzte schnell-Scan Signatur-version|
|lastFullScanSignatureVersion|Zeichenfolge|Letzte vollständige Überprüfung Signatur-version|
|lastReportedDateTime|DateTimeOffset|Letzte Gerät Integritätsstatus gemeldet Zeit|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|detectedMalwareState|[WindowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) -Auflistung|Liste der Geräte Schadsoftware|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```





