---
title: Ressourcentyp deviceProtectionOverview
description: Hardwareinformationen für ein bestimmtes Gerät.
author: tfitzmac
ms.openlocfilehash: e705324bfc611117657ec629f8770e76c69be28d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317052"
---
# <a name="deviceprotectionoverview-resource-type"></a>Ressourcentyp deviceProtectionOverview

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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





