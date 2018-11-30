---
title: AndroidDeviceOwnerGeneralDeviceConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidDeviceOwnerGeneralDeviceConfiguration-Objekts.
ms.openlocfilehash: 463d40f24bb4240eed4fc60078b0fb576a8928b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062734"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a>AndroidDeviceOwnerGeneralDeviceConfiguration aktualisieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Aktualisieren Sie die Eigenschaften eines [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts.
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Accept|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung für das Objekt [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) eine JSON-Darstellung.

In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolesch|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|accountsBlockModification|Boolesch|Gibt an, ob das Hinzufügen oder Entfernen von Konten deaktiviert ist.|
|appsAllowInstallFromUnknownSources|Boolesch|Gibt an, ob der Benutzer berechtigt ist, um das Festlegen von unbekannten Quellen zu ermöglichen.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Gibt den Wert des app-Richtlinie für die automatische Aktualisierung. Mögliche Werte sind: `notConfigured`, `userChoice`, `never`, `wiFiOnly` und `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Gibt die Berechtigungsrichtlinie für Anforderungen für Laufzeitberechtigungen an, ob eine nicht für die app speziell definiert ist. Mögliche Werte: sind `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.|
|bluetoothBlockConfiguration|Boolesch|Gibt an, ob vom Bluetooth konfigurieren einen Benutzer blockieren.|
|bluetoothBlockContactSharing|Boolesch|Gibt an, ob einen Benutzer von der Freigabe von Kontakten über Bluetooth blockieren.|
|cameraBlocked|Boolescher Wert|Gibt an, ob die Verwendung der Kamera zu deaktivieren.|
|cellularBlockWifiTethering|Boolescher Wert|Gibt an, ob WLAN-Tethering blockiert werden soll.|
|dataRoamingBlocked|Boolesch|Gibt an, ob einen Benutzer von servergespeicherten Daten blockieren.|
|dateTimeConfigurationBlocked|Boolesch|Gibt an, ob die Benutzer manuell ändern, die Datums- oder Uhrzeitwerte auf dem Gerät blockieren|
|factoryResetDeviceAdministratorEmails|Collection von Objekten des Typs „String“|Liste der Google-Konto-e-Mails, die erforderlich sind, um zu authentifizieren, nachdem ein Gerät ist Factory zurückzusetzen, bevor eingerichtet werden kann.|
|factoryResetBlocked|Boolescher Wert|Gibt an, ob die Option zum Factory in den Einstellungen deaktiviert ist.|
|kioskModeApps|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Eine Liste der verwalteten apps, die das Gerät bei im Kioskmodus zurückgekehrt ist angezeigt werden. Diese Collection darf maximal 500 Elemente enthalten.|
|microphoneForceMute|Boolesch|Gibt an, ob blockieren Aufheben der stummschaltung für das Mikrofon auf dem Gerät.|
|networkEscapeHatchAllowed|Boolesch|Gibt an, ob das Gerät zulässig, eine Verbindung mit einer temporären-Verbindung beim Starten.|
|nfcBlockOutgoingBeam|Boolesch|Gibt an, ob ausgehende Balken NFK blockieren.|
|passwordBlockKeyguard|Boolesch|Gibt an, ob die Keyguard deaktiviert ist.|
|passwordExpirationDays|Int32|Gibt die Zeitspanne in Sekunden an, die für ein Kennwort festgelegt werden kann, bevor sie abläuft und ein neues Kennwort erforderlich. Gültige Werte: 1 bis 365.|
|passwordMinimumLength|Int32|Gibt die minimale Länge des Kennworts auf dem Gerät erforderlich. Gültige Werte: 4 bis 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeit in Millisekunden vor dem Timeout der Bildschirm Inaktivität.|
|passwordPreviousPasswordCountToBlock|Int32|Gibt die Länge des Kennwortverlauf, wobei der Benutzer nicht möglich wird ein neues Kennwort eingeben, das im Verlauf jedes beliebige Kennwort identisch ist. Gültige Werte: 0 bis 24.|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Gibt die Mindestlänge für Kennwort Qualität auf dem Gerät erforderlich. Mögliche Werte sind: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric` und `alphanumericWithSymbols`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Gibt an, wie oft ein Benutzer ein ungültiges Kennwort eingeben kann, bevor das Gerät bereinigt wird. Gültige Werte: 4 bis 11.|
|safeBootBlocked|Boolesch|Gibt an, ob neu gestartet, dass das Gerät in abgesicherten Modus deaktiviert ist.|
|screenCaptureBlocked|Boolescher Wert|Gibt an, ob die Funktion auszuführende Screenshots deaktivieren.|
|securityAllowDebuggingFeatures|Boolesch|Gibt an, ob die Benutzer aus der debugging-Funktionen auf dem Gerät aktivieren blockieren.|
|securityRequireVerifyApps|Boolescher Wert|Gibt an, ob überprüfen apps ist erforderlich.|
|statusBarBlocked|Boolesch|Gibt an, ob oder den Status Leiste deaktiviert ist, einschließlich Benachrichtigungen, schnelle Einstellungen und anderen Bildschirm überlagert.|
|stayOnModes|[AndroidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) -Auflistung|Liste der Modi, in denen der Anzeige des Geräts eingeschaltet, verbleibt. Diese Sammlung kann maximal 4 Elemente enthalten. Mögliche Werte: sind `notConfigured`, `ac`, `usb` und `wireless`.|
|storageAllowUsb|Boolesch|Gibt an, ob USB-Massenspeichergerät zulassen.|
|storageBlockExternalMedia|Boolesch|Gibt an, ob externe Medien zu blockieren.|
|storageBlockUsbFileTransfer|Boolesch|Gibt an, ob USB-Dateiübertragung zu blockieren.|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|Gibt die Anzahl der Minuten nach Mitternacht, die das System Update Fenster beginnt. Gültige Werte von 0 bis 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|Gibt die Anzahl der Minuten nach Mitternacht, die das System Update Fenster endet. Gültige Werte von 0 bis 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|Der Typ des Systemkonfiguration Update. Mögliche Werte: sind `deviceDefault`, `postpone`, `windowed` und `automatic`.|
|usersBlockAdd|Boolesch|Gibt an, ob Hinzufügen von Benutzern und Profile deaktiviert ist.|
|usersBlockRemove|Boolesch|Gibt an, ob Entfernen von anderen Benutzern vom Gerät zu deaktivieren.|
|volumeBlockAdjustment|Boolesch|Gibt an, ob anpassen, dass die Hauptlautstärke deaktiviert ist.|
|wifiBlockEditConfigurations|Boolesch|Gibt an, ob die Benutzer durch die Bearbeitung von Einstellungen für die WLAN-Verbindung zu blockieren.|
|wifiBlockEditPolicyDefinedConfigurations|Boolesch|Gibt an, ob die Benutzer bearbeiten können nur die von der Richtlinie definierten Netzwerke blockieren.|



## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts in der Antworttext.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2073

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2264

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```





