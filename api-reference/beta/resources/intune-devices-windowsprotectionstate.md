---
title: Windowsprotectionstate wurde-Ressourcentyp
description: Geräteschutz Status-Entität.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eebf798a41e5cbab27fab849cdead8a288a782e2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148314"
---
# <a name="windowsprotectionstate-resource-type"></a>Windowsprotectionstate wurde-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Geräteschutz Status-Entität.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Windowsprotectionstate wurde abrufen](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Lesen von Eigenschaften und Beziehungen des [windowsprotectionstate wurde](../resources/intune-devices-windowsprotectionstate.md) -Objekts.|
|[Windowsprotectionstate wurde aktualisieren](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Aktualisieren der Eigenschaften eines [windowsprotectionstate wurde](../resources/intune-devices-windowsprotectionstate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Der eindeutige Bezeichner für das Statusobjekt des Geräteschutzes. Dies ist die Geräte-ID des Geräts.|
|malwareProtectionEnabled|Boolescher Wert|Antischadsoftware ist aktiviert oder nicht|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Status des Computers (wie Clean oder ausstehender vollständiger Scan oder ausstehender Neustart usw.). Mögliche Werte sind: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending` und `critical`.|
|realTimeProtectionEnabled|Boolescher Wert|Echtzeitschutz ist aktiviert oder nicht?|
|networkInspectionSystemEnabled|Boolescher Wert|Netzwerk Inspektionssystem aktiviert oder nicht?|
|quickScanOverdue|Boolescher Wert|Schnellscan überfällig oder nicht?|
|fullScanOverdue|Boolescher Wert|Vollständiger Scan überfällig oder nicht?|
|signatureUpdateOverdue|Boolescher Wert|Signatur veraltet oder nicht?|
|rebootRequired|Boolescher Wert|Neustart erforderlich oder nicht?|
|fullScanRequired|Boolescher Wert|Vollständige Überprüfung erforderlich oder nicht?|
|engineVersion|Zeichenfolge|Version des aktuellen Endpoint Protection-Moduls|
|signatureVersion|Zeichenfolge|Aktuelle Version der Malware-Definitionen|
|antiMalwareVersion|Zeichenfolge|Aktuelle Antischadsoftware-Version|
|lastQuickScanDateTime|DateTimeOffset|Datum der letzten Schnellüberprüfung|
|lastFullScanDateTime|DateTimeOffset|Datum der letzten Schnellüberprüfung|
|lastQuickScanSignatureVersion|Zeichenfolge|Letzte Schnellscan-Signaturversion|
|lastFullScanSignatureVersion|Zeichenfolge|Letzte vollständige Scan-Signaturversion|
|lastReportedDateTime|DateTimeOffset|Zeitpunkt des letzten Geräte Integritätsstatus|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|detectedMalwareState|[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) -Sammlung|Liste der Geräte Schadsoftware|

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




