# <a name="androidworkprofilegeneraldeviceconfiguration-resource-type"></a>androidWorkProfileGeneralDeviceConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Allgemeine Gerätekonfiguration für das Android-Arbeitsprofil.

Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[androidWorkProfileGeneralDeviceConfigurations-Liste](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_list.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)-Sammlung|Listeneigenschaften und Beziehungen der [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)-Objekte.|
|[Abrufen von androidWorkProfileGeneralDeviceConfiguration](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_get.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)-Objekts.|
|[androidWorkProfileGeneralDeviceConfiguration erstellen](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_create.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)|Erstellt ein neues [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)-Objekt.|
|[androidWorkProfileGeneralDeviceConfiguration löschen](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_delete.md)|Keine|Löscht [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md).|
|[androidWorkProfileGeneralDeviceConfiguration aktualisieren](../api/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration_update.md)|[androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)|Aktualisiert die Eigenschaften eines [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Beschreibung|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|passwordBlockFingerprintUnlock|boolesch|Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.|
|passwordBlockTrustAgents|boolesch|Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts. Gültige Werte: 1 bis 365.|
|passwordMinimumLength|Int32|Mindestlänge von Kennwörtern. Gültige Werte: 4 bis 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt|
|passwordPreviousPasswordBlockCount|Int32|Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen. Gültige Werte: 0 bis 24.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird. Gültige Werte: 4 bis 11.|
|passwordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.|
|workProfileDataSharingType|[androidWorkProfileCrossProfileDataSharingType](../resources/intune_deviceconfig_androidworkprofilecrossprofiledatasharingtype.md)|Typ der zulässigen Datenfreigabe. Mögliche Werte: `deviceDefault`, `preventAny`, `allowPersonalToWork` und `noRestrictions`.|
|workProfileBlockNotificationsWhileDeviceLocked|Boolesch|Gibt an, ob Benachrichtigungen blockiert werden, während ein Gerät gesperrt ist.|
|workProfileBlockAddingAccounts|Boolesch|Blockiert Benutzer vom Hinzufügen/Entfernen von Konten im Arbeitsprofil.|
|workProfileBluetoothEnableContactSharing|Boolesch|Lässt zu, dass Bluetooth-Geräte auf Unternehmenskontakte zugreifen.|
|workProfileBlockScreenCapture|Boolesch|Blockiert die Bildschirmaufnahme im Arbeitsprofil.|
|workProfileBlockCrossProfileCallerId|Boolesch|Blockiert die Anzeige der Arbeitprofil-Rufnummernanzeige im persönlichen Profil.|
|workProfileBlockCamera|Boolesch|Blockiert die Kamera des Arbeitsprofils.|
|workProfileBlockCrossProfileContactsSearch|Boolesch|Blockiert die Verfügbarkeit der Kontakte des Arbeitprofils im persönlichen Profil.|
|workProfileBlockCrossProfileCopyPaste|Boolesch|Boolesch, gibt an, ob die Einstellung für ein Verbot von übergreifendem Kopieren und Einfügen des Profils aktiviert ist.|
|workProfileDefaultAppPermissionPolicy|[androidWorkProfileDefaultAppPermissionPolicyType](../resources/intune_deviceconfig_androidworkprofiledefaultapppermissionpolicytype.md)|Geforderter Kennworttyp. Mögliche Werte: `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.|
|workProfilePasswordBlockFingerprintUnlock|Boolesch|Gibt an, ob die Entsperrung durch Fingerabdruck für das Arbeitsprofil blockiert werden soll.|
|workProfilePasswordBlockTrustAgents|Boolesch|Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agenten für das Arbeitsprofil blockiert werden sollen.|
|workProfilePasswordExpirationDays|Int32|Anzahl der Tage bis zum Ablaufen des Kennworts des Arbeitsprofils. Gültige Werte: 1 bis 365|
|workProfilePasswordMinimumLength|Int32|Mindestlänge des Kennwort des Arbeitsprofils. Gültige Werte: 4 bis 16|
|workProfilePasswordMinNumericCharacters|Int32|Mindestanzahl der numerische Zeichen im Kennwort des Arbeitsprofils. Gültige Werte: 1 bis 10|
|workProfilePasswordMinNonLetterCharacters|Int32|Mindestanzahl der Nicht-Buchstaben-Zeichen im Kennwort des Arbeitsprofils. Gültige Werte: 1 bis 10|
|workProfilePasswordMinLetterCharacters|Int32|Mindestanzahl der Buchstaben im Kennwort des Arbeitsprofils. Gültige Werte: 1 bis 10|
|workProfilePasswordMinLowerCaseCharacters|Int32|Mindestanzahl der Kleinbuchstaben im Kennwort des Arbeitsprofils. Gültige Werte: 1 bis 10|
|workProfilePasswordMinUpperCaseCharacters|Int32|Mindestanzahl der Großbuchstaben im Kennwort des Arbeitsprofils. Gültige Werte: 1 bis 10|
|workProfilePasswordMinSymbolCharacters|Int32|Mindestanzahl der Symbole im Kennwort des Arbeitsprofils. Gültige Werte: 1 bis 10|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.|
|workProfilePasswordPreviousPasswordBlockCount|Int32|Anzahl der zuletzt verwendeten Kennwörter des Arbeitsprofils, die nicht erneut verwendet werden dürfen. Gültige Werte: 0 bis 24|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Anzahl der fehlgeschlagenen Anmeldeversuchen, bevor ein Arbeitsprofil entfernt und alle Firmendaten gelöscht werden. Gültige Werte: 4 bis 11|
|workProfilePasswordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|Geforderter Kennworttyp des Arbeitsprofils. Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.|
|workProfileRequirePassword|Boolesch|Entscheidet, ob ein Kennwort für ein Arbeitsprofil erforderlich ist oder nicht|
|securityRequireVerifyApps|Boolesch|Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|Aufgaben|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileGeneralDeviceConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
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
  "securityRequireVerifyApps": true
}
```








