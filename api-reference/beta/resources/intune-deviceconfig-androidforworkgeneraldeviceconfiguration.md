---
title: Ressourcentyp androidForWorkGeneralDeviceConfiguration
description: Allgemeine Gerätekonfiguration Android für Arbeit.
ms.openlocfilehash: 9979fa108970acbe4cf9c39f3f10f22a818b77d3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060815"
---
# <a name="androidforworkgeneraldeviceconfiguration-resource-type"></a>Ressourcentyp androidForWorkGeneralDeviceConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Allgemeine Gerätekonfiguration Android für Arbeit.

Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste androidForWorkGeneralDeviceConfigurations](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-list.md)|[AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) -Objekte.|
|[Abrufen von androidForWorkGeneralDeviceConfiguration](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-get.md)|[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) -Objekts.|
|[Erstellen von androidForWorkGeneralDeviceConfiguration](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-create.md)|[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)|Erstellen eines neuen [AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) -Objekts.|
|[AndroidForWorkGeneralDeviceConfiguration löschen](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-delete.md)|Keines|Löscht eine [AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).|
|[AndroidForWorkGeneralDeviceConfiguration aktualisieren](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-update.md)|[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)|Aktualisieren Sie die Eigenschaften eines [AndroidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
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
|passwordBlockFingerprintUnlock|Boolescher Wert|Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.|
|passwordBlockTrustAgents|Boolescher Wert|Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts. Gültige Werte: 1 bis 365.|
|passwordMinimumLength|Int32|Mindestlänge von Kennwörtern. Gültige Werte: 4 bis 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt|
|passwordPreviousPasswordBlockCount|Int32|Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen. Gültige Werte: 0 bis 24.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird. Gültige Werte: 4 bis 11.|
|passwordRequiredType|[androidForWorkRequiredPasswordType](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.|
|workProfileDataSharingType|[androidForWorkCrossProfileDataSharingType](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|Typ der Daten, die Freigabe ist zulässig. Mögliche Werte: sind `deviceDefault`, `preventAny`, `allowPersonalToWork` und `noRestrictions`.|
|workProfileBlockNotificationsWhileDeviceLocked|Boolesch|Gibt an, ob beim Gerät gesperrt Benachrichtigungen zu blockieren.|
|workProfileBlockAddingAccounts|Boolesch|Blockieren Sie den Benutzer hinzufügen/entfernen von Konten im Profil Arbeit.|
|workProfileBluetoothEnableContactSharing|Boolesch|Können Sie Bluetooth-Geräte können Kontakte im Unternehmen zugreifen.|
|workProfileBlockScreenCapture|Boolesch|Blockiert die Bildschirmaufnahme im Profil Arbeit.|
|workProfileBlockCrossProfileCallerId|Boolesch|Block Anzeige Arbeit Profil Anrufer-ID im persönlichen Profil.|
|workProfileBlockCamera|Boolesch|Blockieren der Profil Kamera.|
|workProfileBlockCrossProfileContactsSearch|Boolesch|Verfügbarkeit der Block Arbeit Profil Kontakte im persönlichen Profil.|
|workProfileBlockCrossProfileCopyPaste|Boolesch|Boolescher Wert, der angibt, wenn die Einstellung firewallübergreifenden disallow Profil kopieren und einfügen aktiviert ist.|
|workProfileDefaultAppPermissionPolicy|[androidForWorkDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|Geforderter Kennworttyp. Mögliche Werte: sind `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.|
|workProfilePasswordBlockFingerprintUnlock|Boolesch|Gibt an, ob blockieren Fingerabdruck Entsperren für Arbeit Profil.|
|workProfilePasswordBlockTrustAgents|Boolesch|Gibt an, ob intelligente sperren und andere Trust-Agenten für Arbeit Profil zu blockieren.|
|workProfilePasswordExpirationDays|Int32|Anzahl von Tagen vor der Arbeit Profilkennwort läuft ab. Gültige Werte: 1 bis 365.|
|workProfilePasswordMinimumLength|Int32|Minimale Länge der Arbeit Profilkennwort. Gültige Werte: 4 bis 16.|
|workProfilePasswordMinNumericCharacters|Int32|Minimale Anzahl der numerische Zeichen in Arbeit Profilkennwort erforderlich. Gültige Werte 1 bis 10|
|workProfilePasswordMinNonLetterCharacters|Int32|Minimale Anzahl der nicht-Buchstaben in Arbeit Profilkennwort erforderlich. Gültige Werte 1 bis 10|
|workProfilePasswordMinLetterCharacters|Int32|Minimale Anzahl der Buchstaben in Arbeit Profilkennwort erforderlich. Gültige Werte 1 bis 10|
|workProfilePasswordMinLowerCaseCharacters|Int32|Minimale Anzahl der Kleinbuchstaben in Arbeit Profilkennwort erforderlich. Gültige Werte 1 bis 10|
|workProfilePasswordMinUpperCaseCharacters|Int32|Minimale Anzahl der Großbuchstaben in Arbeit Profilkennwort erforderlich. Gültige Werte 1 bis 10|
|workProfilePasswordMinSymbolCharacters|Int32|Minimale Anzahl der Symbole in Arbeit Profilkennwort erforderlich. Gültige Werte 1 bis 10|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt|
|workProfilePasswordPreviousPasswordBlockCount|Int32|Anzahl der vorherigen Arbeit Profil Kennwörter zu blockieren. Gültige Werte: 0 bis 24.|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Anzahl der Anmeldung Fehler zulässig sind, bevor Arbeit Profil entfernt wird und alle Daten gelöscht. Gültige Werte: 4 bis 11.|
|workProfilePasswordRequiredType|[androidForWorkRequiredPasswordType](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|Typ der Arbeit Profilkennwort, das erforderlich ist. Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.|
|workProfileRequirePassword|Boolesch|Kennwort erforderlich ist oder nicht für Arbeit Profil|
|securityRequireVerifyApps|Boolescher Wert|Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.|
|vpnAlwaysOnPackageIdentifier|String|Aktivieren Sie Sperrmodus für immer auf VPN.|
|vpnEnableAlwaysOnLockdownMode|Boolesch|Aktivieren Sie Sperrmodus für immer auf VPN.|

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
  "@odata.type": "microsoft.graph.androidForWorkGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
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
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "workProfileDataSharingType": "String",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "String",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1024,
  "workProfilePasswordMinimumLength": 1024,
  "workProfilePasswordMinNumericCharacters": 1024,
  "workProfilePasswordMinNonLetterCharacters": 1024,
  "workProfilePasswordMinLetterCharacters": 1024,
  "workProfilePasswordMinLowerCaseCharacters": 1024,
  "workProfilePasswordMinUpperCaseCharacters": 1024,
  "workProfilePasswordMinSymbolCharacters": 1024,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "workProfilePasswordPreviousPasswordBlockCount": 1024,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 1024,
  "workProfilePasswordRequiredType": "String",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "String",
  "vpnEnableAlwaysOnLockdownMode": true
}
```




