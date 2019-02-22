---
title: ImportedAppleDeviceIdentityResult aktualisieren
description: Aktualisieren der Eigenschaften eines importedAppleDeviceIdentityResult-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85f2446058aa899f8b624b843ee25df148cec416
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154383"
---
# <a name="update-importedappledeviceidentityresult"></a>ImportedAppleDeviceIdentityResult aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekts.

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
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)|
|serialNumber|Zeichenfolge|Von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbte Geräteseriennummer|
|requestedEnrollmentProfileId|Zeichenfolge|Registrierungsprofil-ID, die vom Administrator für das Gerät während der nächsten von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Registrierung angewendet werden soll|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|Das Zeit Registrierungsprofil wurde dem Gerät zugewiesen, das von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbt wurde.|
|isSupervised|Boolescher Wert|Gibt an, ob das Apple-Gerät überwacht wird. Weitere Informationen finden Sie unter https://support.apple.com/en-us/HT202837 : Inherited from [importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple-Geräte Ermittlungs Quelle. Von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)geerbt. Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.|
|createdDateTime|DateTimeOffset|ErstellungsDatum des von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Geräts|
|lastContactedDateTime|DateTimeOffset|Datum der letzten Kontaktaufnahme des von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Geräts|
|description|Zeichenfolge|Die Beschreibung des von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md) geerbten Geräts|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Der Status des Geräts in InTune, das von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)geerbt wurde. Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.|
|Plattform|[Plattform](../resources/intune-enrollment-platform.md)|Die Plattform des Geräts. Von [Importappledeviceidentitylist](../resources/intune-enrollment-importedappledeviceidentity.md)geerbt. Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.|
|status|Boolescher Wert|Status der importierten Geräte Identität|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 522

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 630

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```




