---
title: deliveryOptimizationBandwidthAbsolute-Ressourcentyp
description: Bandbreitenbegrenzungen in Kilobyte pro Sekunde.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9eca95ad33ced19e437e760663a73158aacc25d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178269"
---
# <a name="deliveryoptimizationbandwidthabsolute-resource-type"></a>deliveryOptimizationBandwidthAbsolute-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Bandbreitenbegrenzungen in Kilobyte pro Sekunde.


Erbt von [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|maximumDownloadBandwidthInKilobytesPerSecond|Int64|Gibt die maximale Download Bandbreite in KiloByte/Sekunde an, die das Gerät für alle gleichzeitigen Download Aktivitäten mithilfe der Übermittlungs Optimierung verwenden kann. Gültige Werte 0 bis 4294967295
Der Wert 0 (null) bewirkt, dass die zuStellungsOptimierung dynamisch angepasst wird, um die verfügbare Bandbreite für Downloads zu verwenden. Gültige Werte 0 bis 4294967295|
|maximumUploadBandwidthInKilobytesPerSecond|Int64|Gibt die maximale Upload-Bandbreite in KiloByte/Sekunde an, die ein Gerät für alle gleichzeitigen Upload-Aktivitäten mithilfe der Übermittlungs Optimierung verwendet (0-4000000). Gültige Werte 0 bis 4 Millionen
Der Standardwert ist 0, was eine unbegrenzte Bandbreite erlaubt (optimiert für minimale Auslastung der Upload-Bandbreite). Gültige Werte 0 bis 4 Millionen|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthAbsolute",
  "maximumDownloadBandwidthInKilobytesPerSecond": 1024,
  "maximumUploadBandwidthInKilobytesPerSecond": 1024
}
```




