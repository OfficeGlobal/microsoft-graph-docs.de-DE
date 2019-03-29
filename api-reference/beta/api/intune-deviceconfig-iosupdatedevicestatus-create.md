---
title: Erstellen von „iosUpdateDeviceStatus“
description: Diese Methode erstellt ein neues Objekt des Typs iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 493c689e11f02d1b57c64796e40346e424b4efb0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984184"
---
# <a name="create-iosupdatedevicestatus"></a>Erstellen von „iosUpdateDeviceStatus“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Diese Methode erstellt ein neues Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementConfiguration.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosUpdateDeviceStatus“ an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosUpdateDeviceStatus“ erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|installStatus|[iosUpdatesInstallStatus](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|Installationsstatus des Richtlinienberichts. Mögliche Werte sind: `success`, `available`, `idle` `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientNetwork` `installing` `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed`,,,, `notSupportedOperation`,,,,,,,,,, `sharedDeviceUserLoggedInError` `downloadInsufficientSpace` `downloadInsufficientPower`|
|osVersion|String|Gemeldete Geräteversion|
|deviceId|String|Gemeldete Geräte-ID|
|userId|String|Gemeldete Benutzer-ID|
|deviceDisplayName|String|Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist|
|userName|String|Gemeldeter Benutzername|
|deviceModel|Zeichenfolge|Gemeldetes Gerätemodell|
|Plattform|Int32|Plattform des gemeldeten Geräts|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität|
|status|[Wurde](../resources/intune-shared-compliancestatus.md)|Konformitätsstatus des Richtlinienberichts. Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Richtlinienberichts|
|userPrincipalName|String|Benutzerprinzipalname|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses
Content-type: application/json
Content-length: 570

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 619

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "63a79499-9499-63a7-9994-a7639994a763",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




