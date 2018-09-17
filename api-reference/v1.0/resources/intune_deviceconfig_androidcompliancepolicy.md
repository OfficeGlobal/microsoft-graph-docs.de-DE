# <a name="androidcompliancepolicy-resource-type"></a>Ressourcentyp „androidCompliancePolicy“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Klasse enthält Konformitätseinstellungen für Android.

Sie erbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „androidCompliancePolicy“](../api/intune_deviceconfig_androidcompliancepolicy_list.md)|Sammlung von Objekten des Typs [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) auf.|
|[Abrufen von „androidCompliancePolicy“](../api/intune_deviceconfig_androidcompliancepolicy_get.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).|
|[Erstellen von „androidCompliancePolicy“](../api/intune_deviceconfig_androidcompliancepolicy_create.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|Erstellt neue Objekte des Typs [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).|
|[Löschen von „androidCompliancePolicy“](../api/intune_deviceconfig_androidcompliancepolicy_delete.md)|Keiner|Löscht Objekte des Typs [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).|
|[Aktualisieren von „androidCompliancePolicy“](../api/intune_deviceconfig_androidcompliancepolicy_update.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|Aktualisiert die Eigenschaften von Objekten des Typs [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|Beschreibung|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|passwordRequired|Boolesch|Legt fest, dass zum Entsperren des Geräts ein Kennwort erforderlich ist.|
|passwordMinimumLength|Int32|Mindestlänge des Kennworts. Gültige Werte: 4 bis 16.|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|Typ der Zeichen im Kennwort. Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.|
|passwordMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts Gültige Werte: 1 bis 65535|
|passwordPreviousPasswordBlockCount|Int32|Legt fest, wie viele der zuletzt verwendeten Kennwörter nicht erneut verwendet werden dürfen.|
|securityPreventInstallAppsFromUnknownSources|Boolesch|Legt fest, dass Geräte die Installation von Apps aus unbekannten Quellen nicht zulassen dürfen.|
|securityDisableUsbDebugging|Boolesch|Deaktiviert das USB-Debuggen auf Android-Geräten.|
|securityRequireVerifyApps|Boolesch|Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.|
|deviceThreatProtectionEnabled|Boolesch|Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll. Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.|
|securityBlockJailbrokenDevices|Boolesch|Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.|
|osMinimumVersion|Zeichenfolge|Mindestversion von Android|
|osMaximumVersion|Zeichenfolge|Maximalversion von Android|
|minAndroidSecurityPatchLevel|Zeichenfolge|Mindestens geforderter Sicherheitspatchlevel von Android|
|storageRequireEncryption|Boolesch|Legt fest, dass auf Android-Geräten Verschlüsselung aktiviert sein muss.|
|securityRequireSafetyNetAttestationBasicIntegrity|Boolesch|Legt fest, dass das Gerät die SafetyNet-Basisintegritätsprüfung bestanden haben muss.|
|securityRequireSafetyNetAttestationCertifiedDevice|Boolesch|Legt fest, dass das Gerät die Prüfung zum SafetyNet-zertifizierten Gerät bestanden haben muss.|
|securityRequireGooglePlayServices|Boolesch|Legt fest, dass Google Play Services auf dem Gerät installiert und aktiviert sein muss.|
|securityRequireUpToDateSecurityProviders|Boolesch|Legt fest, dass die Sicherheitsanbieter des Geräts aktuell sein müssen. Die aktuelle Version von Google Play Services muss auf dem Gerät installiert und aktiviert sein.|
|securityRequireCompanyPortalAppIntegrity|Boolesch|Legt fest, dass das Gerät die Laufzeitintegritätsprüfung für Unternehmensportal-Client-Apps bestanden haben muss.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|scheduledActionsForRule|Sammlung von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Liste der geplanten Aktionen für die Regel. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceStatuses|Sammlung von Objekten des Typs [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|Liste von Objekten des Typs „deviceComplianceDeviceStatus“. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|userStatuses|Sammlung von Objekten des Typs [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Liste von Objekten des Typs „deviceComplianceUserStatus“. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|Übersicht über den Status der Gerätekonformität nach Gerät. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|Übersicht über den Status der Gerätekonformität nach Benutzer. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus der Konformitätsrichtlinie nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|Aufgaben|Sammlung von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|Sammlung von Zuweisungen für die Konformitätsrichtlinie. Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceCompliancePolicy",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidCompliancePolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordMinimumLength": 1024,
  "passwordRequiredType": "String",
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "minAndroidSecurityPatchLevel": "String",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```








