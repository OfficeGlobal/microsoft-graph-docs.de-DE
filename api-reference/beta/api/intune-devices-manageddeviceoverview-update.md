---
title: Aktualisieren von „managedDeviceOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f2bdf2e213f52626ea3a45016b536c34713ad5f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984618"
---
# <a name="update-manageddeviceoverview"></a>Aktualisieren von „managedDeviceOverview“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für die Zusammenfassung|
|enrolledDeviceCount|Int32|Gesamtanzahl von registrierten Geräten. Über den Intune-PC-Agent verwaltete Geräte sind nicht enthalten.|
|mdmEnrolledCount|Int32|Anzahl von in MDM registrierten Geräten|
|dualEnrolledDeviceCount|Int32|Anzahl von Geräten, die in MDM und EAS registriert sind|
|deviceOperatingSystemSummary|[deviceOperatingSystemSummary](../resources/intune-devices-deviceoperatingsystemsummary.md)|Betriebssystem des Geräts – Zusammenfassung.|
|deviceExchangeAccessStateSummary|[deviceExchangeAccessStateSummary](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|Verteilung des Exchange-Zugriffsstatus in Intune|
|managedDeviceModelsAndManufacturers|[managedDeviceModelsAndManufacturers](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|Modelliert und fertigt meatadata für verwaltete Geräte im Konto|
|lastModifiedDateTime|DateTimeOffset|Datum der letzten Änderung der Geräteübersicht|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 943

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "Device Models value"
    ],
    "deviceManufacturers": [
      "Device Manufacturers value"
    ]
  }
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1056

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "42a91653-1653-42a9-5316-a9425316a942",
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "Device Models value"
    ],
    "deviceManufacturers": [
      "Device Manufacturers value"
    ]
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




