---
title: Ressourcentyp deviceProtectionOverview
description: Hardwareinformationen für ein bestimmtes Gerät.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 902e3a6062d2aa50c96c27eb9d542905bf9a029d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418988"
---
# <a name="deviceprotectionoverview-resource-type"></a>Ressourcentyp deviceProtectionOverview

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Hardwareinformationen für ein bestimmtes Gerät.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|totalReportedDeviceCount|Int32|Anzahl der insgesamt Geräte.|
|inactiveThreatAgentDeviceCount|Int32|Gerät mit inaktiven Threat Agent count|
|unknownStateThreatAgentDeviceCount|Int32|Gerät Threat Agent Zustand wie unbekannte Count.|
|pendingSignatureUpdateDeviceCount|Int32|Das Gerät mit alten Signatur Count.|
|cleanDeviceCount|Int32|Bereinigen Sie die Anzahl der Geräte.|
|pendingFullScanDeviceCount|Int32|Anzahl der ausstehenden vollständigen Scan Geräte.|
|pendingRestartDeviceCount|Int32|Anzahl ausstehender Neustart-Geräte.|
|pendingManualStepsDeviceCount|Int32|Anzahl der ausstehenden manuelle Schritte Geräte.|
|pendingOfflineScanDeviceCount|Int32|Anzahl der ausstehenden offline Scan Geräte.|
|criticalFailuresDeviceCount|Int32|Anzahl der Geräte kritische Fehler.|

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




