---
title: managedDeviceOverview-Ressourcentyp
description: Zusammenfassungsdaten für verwaltete Geräte
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e6c7187bc5cb984e4ca7e607068e6010f747f868
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175003"
---
# <a name="manageddeviceoverview-resource-type"></a>managedDeviceOverview-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Zusammenfassungsdaten für verwaltete Geräte

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedDeviceOverview abrufen](../api/intune-devices-manageddeviceoverview-get.md)|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Lesen von Eigenschaften und Beziehungen des [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.|
|[managedDeviceOverview aktualisieren](../api/intune-devices-manageddeviceoverview-update.md)|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für die Zusammenfassung|
|enrolledDeviceCount|Int32|Gesamtanzahl von registrierten Geräten. Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.|
|mdmEnrolledCount|Int32|Anzahl von in MDM registrierten Geräten|
|dualEnrolledDeviceCount|Int32|Anzahl von Geräten, die in MDM und EAS registriert sind|
|deviceOperatingSystemSummary|[deviceOperatingSystemSummary](../resources/intune-devices-deviceoperatingsystemsummary.md)|Betriebssystemzusammenfassung für das Gerät|
|deviceExchangeAccessStateSummary|[deviceExchangeAccessStateSummary](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|Verteilung des Exchange-Zugriffsstatus in Intune|
|managedDeviceModelsAndManufacturers|[managedDeviceModelsAndManufacturers](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|Modelliert und fertigt meatadata für verwaltete Geräte im Konto|
|lastModifiedDateTime|DateTimeOffset|Datum der letzten Änderung der Geräteübersicht|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "String"
    ],
    "deviceManufacturers": [
      "String"
    ]
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```




