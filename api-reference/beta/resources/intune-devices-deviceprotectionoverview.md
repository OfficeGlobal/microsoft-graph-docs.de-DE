---
title: deviceProtectionOverview-Ressourcentyp
description: Hardware Informationen eines bestimmten Geräts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d6cd5cc1eef939476a6fa3b5c46a7cfa315607b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154089"
---
# <a name="deviceprotectionoverview-resource-type"></a>deviceProtectionOverview-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Hardware Informationen eines bestimmten Geräts.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|totalReportedDeviceCount|Int32|Gesamtanzahl der Geräte.|
|inactiveThreatAgentDeviceCount|Int32|Geräte mit Anzahl der inaktiven Bedrohungen|
|unknownStateThreatAgentDeviceCount|Int32|Gerät mit dem Status des Bedrohungs-Agents als unbekannte Anzahl.|
|pendingSignatureUpdateDeviceCount|Int32|Gerät mit Alter Signatur Anzahl.|
|cleanDeviceCount|Int32|Geräteanzahl wird bereinigt.|
|pendingFullScanDeviceCount|Int32|Anzahl der ausStehenden vollständigen Scans.|
|pendingRestartDeviceCount|Int32|Anzahl der ausStehenden Neustart Geräte.|
|pendingManualStepsDeviceCount|Int32|AusStehende manuelle Schritte Geräteanzahl.|
|pendingOfflineScanDeviceCount|Int32|Anzahl der ausStehenden Offline Scangeräte.|
|criticalFailuresDeviceCount|Int32|Geräteanzahl für kritische Fehler.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "totalReportedDeviceCount": 1024,
  "inactiveThreatAgentDeviceCount": 1024,
  "unknownStateThreatAgentDeviceCount": 1024,
  "pendingSignatureUpdateDeviceCount": 1024,
  "cleanDeviceCount": 1024,
  "pendingFullScanDeviceCount": 1024,
  "pendingRestartDeviceCount": 1024,
  "pendingManualStepsDeviceCount": 1024,
  "pendingOfflineScanDeviceCount": 1024,
  "criticalFailuresDeviceCount": 1024
}
```




