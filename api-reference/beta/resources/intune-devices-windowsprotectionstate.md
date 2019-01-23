---
title: Ressourcentyp windowsProtectionState
description: Gerät Protection Status Entität.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1ef6c86983475abc687055ac2322ba02fae27ecd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423587"
---
# <a name="windowsprotectionstate-resource-type"></a>Ressourcentyp windowsProtectionState

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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
|malwareProtectionEnabled|Boolean|Anti-Malware ist oder nicht aktiviert|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Zustand des Computers (wie bereinigen oder ausstehende vollständigen Scan oder Ausstehender Neustart usw.). Mögliche Werte sind: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending` und `critical`.|
|realTimeProtectionEnabled|Boolean|Echtzeit-Schutz ist oder nicht aktiviert?|
|networkInspectionSystemEnabled|Boolean|Netzwerk-Prüfung System aktiviert ist oder nicht?|
|quickScanOverdue|Boolean|Quick scan überfällige oder nicht?|
|fullScanOverdue|Boolean|Des vollständigen Scan überfällige oder nicht?|
|signatureUpdateOverdue|Boolean|Signatur veraltet oder nicht?|
|rebootRequired|Boolean|Neustart erforderlich oder nicht?|
|fullScanRequired|Boolean|Vollständigen Scan erforderlich oder nicht?|
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




