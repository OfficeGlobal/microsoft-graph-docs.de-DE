---
title: Ressourcentyp androidDeviceOwnerGeneralDeviceConfiguration
description: Dieses Thema enthält eine Beschreibung der deklarierten Methoden, Eigenschaften und Beziehungen, die durch die AndroidDeviceOwnerGeneralDeviceConfiguration Ressource verfügbar gemacht werden.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ac403bd13091a9db61b7f27462caecf6934b452
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403749"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>Ressourcentyp androidDeviceOwnerGeneralDeviceConfiguration

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Dieses Thema enthält eine Beschreibung der deklarierten Methoden, Eigenschaften und Beziehungen, die durch die AndroidDeviceOwnerGeneralDeviceConfiguration Ressource verfügbar gemacht werden.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste androidDeviceOwnerGeneralDeviceConfigurations](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|[AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekte.|
|[Abrufen von androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts.|
|[Erstellen von androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Erstellen eines neuen [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts.|
|[AndroidDeviceOwnerGeneralDeviceConfiguration löschen](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|Keine|Löscht eine [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).|
|[AndroidDeviceOwnerGeneralDeviceConfiguration aktualisieren](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Aktualisieren Sie die Eigenschaften eines [AndroidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Zeichenfolgenauflistung|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|accountsBlockModification|Boolean|Gibt an, ob das Hinzufügen oder Entfernen von Konten deaktiviert ist.|
|appsAllowInstallFromUnknownSources|Boolean|Gibt an, ob der Benutzer berechtigt ist, um das Festlegen von unbekannten Quellen zu ermöglichen.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Gibt den Wert des app-Richtlinie für die automatische Aktualisierung. Mögliche Werte sind: `notConfigured`, `userChoice`, `never`, `wiFiOnly` und `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Gibt die Berechtigungsrichtlinie für Anforderungen für Laufzeitberechtigungen an, ob eine nicht für die app speziell definiert ist. Mögliche Werte: sind `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.|
|appsRecommendSkippingFirstUseHints|Boolean|Ob alle apps empfehlen überspringen Hinweise ersten Mal verwenden, die sie möglicherweise hinzugefügt haben.|
|bluetoothBlockConfiguration|Boolean|Gibt an, ob vom Bluetooth konfigurieren einen Benutzer blockieren.|
|bluetoothBlockContactSharing|Boolean|Gibt an, ob einen Benutzer von der Freigabe von Kontakten über Bluetooth blockieren.|
|cameraBlocked|Boolean|Gibt an, ob die Verwendung der Kamera zu deaktivieren.|
|cellularBlockWifiTethering|Boolean|Gibt an, ob WLAN-Tethering blockiert werden soll.|
|dataRoamingBlocked|Boolean|Gibt an, ob einen Benutzer von servergespeicherten Daten blockieren.|
|dateTimeConfigurationBlocked|Boolean|Gibt an, ob die Benutzer manuell ändern, die Datums- oder Uhrzeitwerte auf dem Gerät blockieren|
|factoryResetDeviceAdministratorEmails|Zeichenfolgenauflistung|Liste der Google-Konto-e-Mails, die erforderlich sind, um zu authentifizieren, nachdem ein Gerät ist Factory zurückzusetzen, bevor eingerichtet werden kann.|
|factoryResetBlocked|Boolean|Gibt an, ob die Option zum Factory in den Einstellungen deaktiviert ist.|
|kioskModeApps|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Eine Liste der verwalteten apps, die das Gerät bei im Kioskmodus zurückgekehrt ist angezeigt werden. Diese Collection darf maximal 500 Elemente enthalten.|
|kioskModeWallpaperUrl|Zeichenfolge|URL zu einem öffentlich zugänglichen Bild für den Hintergrund verwenden, wenn das Gerät im Kioskmodus zurückgekehrt ist.|
|kioskModeExitCode|Zeichenfolge|Beenden Sie Code, damit der Benutzer von Kioskmodus Escapezeichen, wenn das Gerät im Kioskmodus zurückgekehrt ist.|
|kioskModeVirtualHomeButtonEnabled|Boolean|Ob Sie eine virtuelle private Schaltfläche angezeigt wird, wenn das Gerät im Kioskmodus zurückgekehrt ist.|
|microphoneForceMute|Boolean|Gibt an, ob blockieren Aufheben der stummschaltung für das Mikrofon auf dem Gerät.|
|networkEscapeHatchAllowed|Boolean|Gibt an, ob das Gerät zulässig, eine Verbindung mit einer temporären-Verbindung beim Starten.|
|nfcBlockOutgoingBeam|Boolean|Gibt an, ob ausgehende Balken NFK blockieren.|
|passwordBlockKeyguard|Boolean|Gibt an, ob die Keyguard deaktiviert ist.|
|passwordBlockKeyguardFeatures|[AndroidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) -Auflistung|Liste der Features des Geräts Keyguard blockiert. Diese Sammlung darf maximal 7 Elemente enthalten.|
|passwordExpirationDays|Int32|Gibt die Zeitspanne in Sekunden an, die für ein Kennwort festgelegt werden kann, bevor sie abläuft und ein neues Kennwort erforderlich. Gültige Werte: 1 bis 365.|
|passwordMinimumLength|Int32|Gibt die minimale Länge des Kennworts auf dem Gerät erforderlich. Gültige Werte: 4 bis 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeit in Millisekunden vor dem Timeout der Bildschirm Inaktivität.|
|passwordPreviousPasswordCountToBlock|Int32|Gibt die Länge des Kennwortverlauf, wobei der Benutzer nicht möglich wird ein neues Kennwort eingeben, das im Verlauf jedes beliebige Kennwort identisch ist. Gültige Werte: 0 bis 24.|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Gibt die Mindestlänge für Kennwort Qualität auf dem Gerät erforderlich. Mögliche Werte sind: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric` und `alphanumericWithSymbols`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Gibt an, wie oft ein Benutzer ein ungültiges Kennwort eingeben kann, bevor das Gerät bereinigt wird. Gültige Werte: 4 bis 11.|
|safeBootBlocked|Boolean|Gibt an, ob neu gestartet, dass das Gerät in abgesicherten Modus deaktiviert ist.|
|screenCaptureBlocked|Boolean|Gibt an, ob die Funktion auszuführende Screenshots deaktivieren.|
|securityAllowDebuggingFeatures|Boolean|Gibt an, ob die Benutzer aus der debugging-Funktionen auf dem Gerät aktivieren blockieren.|
|securityRequireVerifyApps|Boolean|Gibt an, ob überprüfen apps ist erforderlich.|
|statusBarBlocked|Boolean|Gibt an, ob oder den Status Leiste deaktiviert ist, einschließlich Benachrichtigungen, schnelle Einstellungen und anderen Bildschirm überlagert.|
|stayOnModes|[AndroidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) -Auflistung|Liste der Modi, in denen der Anzeige des Geräts eingeschaltet, verbleibt. Diese Sammlung kann maximal 4 Elemente enthalten.|
|storageAllowUsb|Boolean|Gibt an, ob USB-Massenspeichergerät zulassen.|
|storageBlockExternalMedia|Boolean|Gibt an, ob externe Medien zu blockieren.|
|storageBlockUsbFileTransfer|Boolean|Gibt an, ob USB-Dateiübertragung zu blockieren.|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|Gibt die Anzahl der Minuten nach Mitternacht, die das System Update Fenster beginnt. Gültige Werte von 0 bis 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|Gibt die Anzahl der Minuten nach Mitternacht, die das System Update Fenster endet. Gültige Werte von 0 bis 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|Der Typ des Systemkonfiguration Update. Mögliche Werte: sind `deviceDefault`, `postpone`, `windowed` und `automatic`.|
|systemWindowsBlocked|Boolean|Ob Android System blockieren auffordern, Windows, wie Popups, Telefon Aktivitäten und System-Benachrichtigungen.|
|usersBlockAdd|Boolean|Gibt an, ob Hinzufügen von Benutzern und Profile deaktiviert ist.|
|usersBlockRemove|Boolean|Gibt an, ob Entfernen von anderen Benutzern vom Gerät zu deaktivieren.|
|volumeBlockAdjustment|Boolean|Gibt an, ob anpassen, dass die Hauptlautstärke deaktiviert ist.|
|vpnAlwaysOnPackageIdentifier|Zeichenfolge|Android-app-Paket-Name für die app, die eine VPN-Verbindung immer auf behandelt.|
|vpnAlwaysOnLockdownMode|Boolean|Wenn ein immer auf VPN Packen Sie Name werden, unabhängig davon, ob angegeben Netzwerkverkehr sperren, wenn diese VPN getrennt wird.|
|wifiBlockEditConfigurations|Boolean|Gibt an, ob die Benutzer durch die Bearbeitung von Einstellungen für die WLAN-Verbindung zu blockieren.|
|wifiBlockEditPolicyDefinedConfigurations|Boolean|Gibt an, ob die Benutzer bearbeiten können nur die von der Richtlinie definierten Netzwerke blockieren.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Auflistung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Gerät Konfiguration Installationsstatus durch Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "String",
  "appsDefaultPermissionPolicy": "String",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "String"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "kioskModeWallpaperUrl": "String",
  "kioskModeExitCode": "String",
  "kioskModeVirtualHomeButtonEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "String"
  ],
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordCountToBlock": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "String"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 1024,
  "systemUpdateWindowEndMinutesAfterMidnight": 1024,
  "systemUpdateInstallType": "String",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "String",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```




