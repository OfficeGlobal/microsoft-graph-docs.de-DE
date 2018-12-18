---
title: Ressourcentyp windowsProtectionState
description: Gerät Protection Status Entität.
author: tfitzmac
ms.openlocfilehash: 636b969ddafde5976939df764ae1180e19a181c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328077"
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
|id|String|Der eindeutige Bezeichner für das Gerät Protection Status-Objekt. Dies ist die Geräte-Id des Geräts|
|malwareProtectionEnabled|Boolesch|Anti-Malware ist oder nicht aktiviert|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Zustand des Computers (wie bereinigen oder ausstehende vollständigen Scan oder Ausstehender Neustart usw.). Mögliche Werte sind: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending` und `critical`.|
|realTimeProtectionEnabled|Boolesch|Echtzeit-Schutz ist oder nicht aktiviert?|
|networkInspectionSystemEnabled|Boolesch|Netzwerk-Prüfung System aktiviert ist oder nicht?|
|quickScanOverdue|Boolesch|Quick scan überfällige oder nicht?|
|fullScanOverdue|Boolesch|Des vollständigen Scan überfällige oder nicht?|
|signatureUpdateOverdue|Boolesch|Signatur veraltet oder nicht?|
|rebootRequired|Boolesch|Neustart erforderlich oder nicht?|
|fullScanRequired|Boolesch|Vollständigen Scan erforderlich oder nicht?|
|%ENGINEVERSION%|String|Aktuelle Endpoint Protection Datenbankmodul, version|
|signatureVersion|String|Aktuelle Version der Malware-Definitionen|
|antiMalwareVersion|String|Aktuelle anti-Malware-version|
|lastQuickScanDateTime|DateTimeOffset|Letzte schnell-Scan datetime|
|lastFullScanDateTime|DateTimeOffset|Letzte schnell-Scan datetime|
|lastQuickScanSignatureVersion|String|Letzte schnell-Scan Signatur-version|
|lastFullScanSignatureVersion|String|Letzte vollständige Überprüfung Signatur-version|
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





