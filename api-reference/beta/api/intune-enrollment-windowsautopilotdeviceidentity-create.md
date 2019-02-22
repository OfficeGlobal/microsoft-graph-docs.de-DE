---
title: WindowsAutopilotDeviceIdentity erstellen
description: Erstellen eines neuen windowsAutopilotDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d87a27c120f4866725e2f91828e8c267f655e69c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175304"
---
# <a name="create-windowsautopilotdeviceidentity"></a>WindowsAutopilotDeviceIdentity erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsAutopilotDeviceIdentity-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsAutopilotDeviceIdentity erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|GUID des Objekts|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Profil Zuordnungsstatus des Windows Autopilot-Geräts. Mögliche Werte sind: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending` und `failed`.|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|Profilzuweisung detaillierter Status des Windows Autopilot-Geräts. Mögliche Werte sind: `none` und `hardwareRequirementsNotMet`.|
|deploymentProfileAssignedDateTime|DateTimeOffset|Festgelegte Zeit des Windows Autopilot-Geräts.|
|orderIdentifier|String|Auftragsbezeichner des Windows Autopilot-Geräts.|
|purchaseOrderIdentifier|Zeichenfolge|Bestellkennung des Windows Autopilot-Geräts.|
|serialNumber|String|Seriennummer des Windows AutoPilot-Geräts|
|productKey|Zeichenfolge|Product Key des Windows AutoPilot-Geräts|
|manufacturer|Zeichenfolge|OEM-Hersteller des Windows Autopilot-Geräts.|
|model|Zeichenfolge|Modellname des Windows Autopilot-Geräts.|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|InTune-Registrierungsstatus des Windows Autopilot-Geräts. Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.|
|lastContactedDateTime|DateTimeOffset|InTune zuletzt kontaktierte Datum Uhrzeit des Windows Autopilot-Geräts.|
|addressableUserName|Zeichenfolge|Adressierbarer Benutzername.|
|userPrincipalName|Zeichenfolge|Benutzerprinzipal Name.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 755

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 804

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




