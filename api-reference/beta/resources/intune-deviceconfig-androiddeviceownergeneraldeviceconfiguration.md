---
title: androidDeviceOwnerGeneralDeviceConfiguration-Ressourcentyp
description: Dieses Thema enthält Beschreibungen der deklarierten Methoden, Eigenschaften und Beziehungen, die von der androidDeviceOwnerGeneralDeviceConfiguration-Ressource verfügbar gemacht werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fee3354cc66bb90a51874986ed46b80b4a8c9d8c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156203"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>androidDeviceOwnerGeneralDeviceConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Dieses Thema enthält Beschreibungen der deklarierten Methoden, Eigenschaften und Beziehungen, die von der androidDeviceOwnerGeneralDeviceConfiguration-Ressource verfügbar gemacht werden.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[AndroidDeviceOwnerGeneralDeviceConfigurations aufListen](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekte.|
|[AndroidDeviceOwnerGeneralDeviceConfiguration abrufen](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts.|
|[AndroidDeviceOwnerGeneralDeviceConfiguration erstellen](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Erstellen eines neuen [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts.|
|[AndroidDeviceOwnerGeneralDeviceConfiguration löschen](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|Keine|Löscht eine [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).|
|[AndroidDeviceOwnerGeneralDeviceConfiguration aktualisieren](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Aktualisieren der Eigenschaften eines [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolescher Wert|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|accountsBlockModification|Boolescher Wert|Gibt an, ob das Hinzufügen oder Entfernen von Konten deaktiviert ist.|
|appsAllowInstallFromUnknownSources|Boolescher Wert|Gibt an, ob der Benutzer die Einstellung für unbekannte Quellen aktivieren darf.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Gibt den Wert der APP-AutoUpdate-Richtlinie an. Mögliche Werte: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Gibt die Berechtigungsrichtlinie für Anforderungen für Laufzeitberechtigungen an, wenn eine nicht speziell für die APP definiert ist. Mögliche Werte: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|appsRecommendSkippingFirstUseHints|Boolescher Wert|Ob alle apps empfohlen werden, überspringen Sie möglicherweise hinzugefügte Hinweise zum ersten Mal.|
|bluetoothBlockConfiguration|Boolescher Wert|Gibt an, ob ein Benutzer von der Konfiguration von Bluetooth blockiert werden soll.|
|bluetoothBlockContactSharing|Boolescher Wert|Gibt an, ob die Freigabe von Kontakten über Bluetooth durch einen Benutzer blockiert werden soll.|
|cameraBlocked|Boolean|Gibt an, ob die Verwendung der Kamera deaktiviert werden soll.|
|cellularBlockWifiTethering|Boolescher Wert|Gibt an, ob WLAN-Tethering blockiert werden soll.|
|dataRoamingBlocked|Boolescher Wert|Gibt an, ob ein Benutzer vom Datenroaming blockiert werden soll.|
|dateTimeConfigurationBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer das Datum oder die Uhrzeit auf dem Gerät manuell ändert.|
|factoryResetDeviceAdministratorEmails|String collection|Liste der Google-Konto-e-Mails, die für die Authentifizierung erforderlich sind, nachdem ein Gerät zurückgesetzt wurde, bevor es eingerichtet werden kann.|
|factoryResetBlocked|Boolean|Gibt an, ob die Option Factory zurücksetzen in den Einstellungen deaktiviert ist.|
|kioskModeApps|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Eine Liste der verwalteten apps, die angezeigt werden, wenn sich das Gerät im Kiosk Modus befindet. Diese Collection darf maximal 500 Elemente enthalten.|
|kioskModeWallpaperUrl|Zeichenfolge|Die URL eines öffentlich zugänglichen Bilds, das für das Hintergrundbild verwendet werden soll, wenn sich das Gerät im Kiosk Modus befindet.|
|kioskModeExitCode|Zeichenfolge|Beenden Sie Code, damit ein Benutzer aus dem Kioskmodus entkommen kann, wenn sich das Gerät im Kiosk-Modus befindet.|
|kioskModeVirtualHomeButtonEnabled|Boolescher Wert|Gibt an, ob eine virtuelle Start Schaltfläche angezeigt werden soll, wenn sich das Gerät im Kiosk Modus befindet.|
|microphoneForceMute|Boolescher Wert|Gibt an, ob die Stummschaltung des Mikrofons auf dem Gerät blockiert werden soll.|
|networkEscapeHatchAllowed|Boolescher Wert|Gibt an, ob das Gerät beim Booten das Herstellen einer Verbindung mit einer temporären Netzwerkverbindung zulässt.|
|nfcBlockOutgoingBeam|Boolescher Wert|Gibt an, ob NFC-ausgehender Balken blockiert werden soll.|
|passwordBlockKeyguard|Boolescher Wert|Gibt an, ob die Tastensperre deaktiviert ist.|
|passwordBlockKeyguardFeatures|[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) -Sammlung|Liste der zu blockierenden Geräte-Keyguard-Features. Diese Sammlung darf maximal 7 Elemente enthalten.|
|passwordExpirationDays|Int32|Gibt den Zeitraum in Sekunden an, für den ein Kennwort festgelegt werden kann, bevor es abläuft und ein neues Kennwort erforderlich ist. Gültige Werte: 1 bis 365.|
|passwordMinimumLength|Int32|Gibt die minimale Länge des auf dem Gerät erforderlichen Kennworts an. Gültige Werte: 4 bis 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Millisekunden der Inaktivität vor dem Timeout des Bildschirms.|
|passwordPreviousPasswordCountToBlock|Int32|Gibt die Länge des Kennwortverlaufs an, in der der Benutzer kein neues Kennwort eingeben kann, das mit einem Kennwort im Verlauf identisch ist. Gültige Werte: 0 bis 24.|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Gibt die auf dem Gerät erforderliche minimale Kenn Wort Qualität an. Mögliche Werte sind: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric` und `alphanumericWithSymbols`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Gibt an, wie oft ein Benutzer ein falsches Kennwort eingeben kann, bevor das Gerät gelöscht wird. Gültige Werte: 4 bis 11.|
|safeBootBlocked|Boolescher Wert|Gibt an, ob das Gerät in den sicheren Start neu gestartet wird.|
|screenCaptureBlocked|Boolescher Wert|Gibt an, ob die Funktion zum Ausführen von Screenshots deaktiviert werden soll.|
|securityAllowDebuggingFeatures|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Debuggingfunktionen auf dem Gerät aktiviert.|
|securityRequireVerifyApps|Boolescher Wert|Gibt an, ob apps überprüfen erforderlich ist.|
|statusBarBlocked|Boolescher Wert|Gibt an, ob die Statusleiste deaktiviert ist, einschließlich Benachrichtigungen, schnell Einstellungen und anderen Bildschirm-Overlays.|
|stayOnModes|[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) -Sammlung|Liste der Modi, in denen die Anzeige des Geräts eingeschaltet bleibt. Diese Auflistung kann maximal 4 Elemente enthalten.|
|storageAllowUsb|Boolescher Wert|Gibt an, ob USB-Massenspeicher zugelassen werden sollen.|
|storageBlockExternalMedia|Boolescher Wert|Gibt an, ob externe Medien blockiert werden sollen.|
|storageBlockUsbFileTransfer|Boolescher Wert|Gibt an, ob die USB-Dateiübertragung blockiert werden soll.|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|Gibt die Anzahl von Minuten nach Mitternacht an, die das System Aktualisierungsfenster startet. Gültige Werte 0 bis 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|Gibt die Anzahl von Minuten nach Mitternacht an, die das System Aktualisierungsfenster beendet. Gültige Werte 0 bis 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|Der Typ der System Update Konfiguration. Mögliche Werte: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|systemWindowsBlocked|Boolescher Wert|Gibt an, ob Android-Systemansage Fenster wie Toasts, Telefonaktivitäten und System Warnungen blockiert werden sollen.|
|usersBlockAdd|Boolescher Wert|Gibt an, ob das Hinzufügen von Benutzern und Profilen deaktiviert ist.|
|usersBlockRemove|Boolescher Wert|Gibt an, ob das Entfernen anderer Benutzer vom Gerät deaktiviert werden soll.|
|volumeBlockAdjustment|Boolescher Wert|Gibt an, ob die Master Lautstärke deaktiviert ist.|
|vpnAlwaysOnPackageIdentifier|Zeichenfolge|Android-App-Paket Name für die APP, die eine Always-on-VPN-Verbindung verarbeitet.|
|vpnAlwaysOnLockdownMode|Boolescher Wert|Wenn ein Name des Always-on-VPN-Pakets angegeben wird, unabhängig davon, ob der Netzwerkdatenverkehr beim Trennen der Verbindung mit dem VPN gesperrt werden soll.|
|wifiBlockEditConfigurations|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer die Einstellungen für die WLAN-Verbindung bearbeitet.|
|wifiBlockEditPolicyDefinedConfigurations|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer nur die von der Richtlinie definierten Netzwerke bearbeitet.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Sammlung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
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




