# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a>androidWorkProfileGeneralDeviceConfiguration aktualisieren

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Aktualisiert die Eigenschaften eines [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)-Objekts.
## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

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
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Autorisierung|Bearer&lt;token&gt; erforderlich|
|Akzeptieren|Anwendung/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung des [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)-Objekts an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen von [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)zurück.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Beschreibung|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|passwordBlockFingerprintUnlock|boolesch|Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.|
|passwordBlockTrustAgents|boolesch|Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts. Gültige Werte: 1 bis 365.|
|passwordMinimumLength|Int32|Mindestlänge von Kennwörtern. Gültige Werte: 4 bis 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt|
|passwordPreviousPasswordBlockCount|Int32|Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen. Gültige Werte: 0 bis 24.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird. Gültige Werte: 4 bis 11.|
|passwordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.|
|workProfileDataSharingType|[androidWorkProfileCrossProfileDataSharingType](../resources/intune_deviceconfig_androidworkprofilecrossprofiledatasharingtype.md)|Typ der zulässigen Datenfreigabe. Mögliche Werte: sind `deviceDefault`, `preventAny`, `allowPersonalToWork` und `noRestrictions`.|
|workProfileBlockNotificationsWhileDeviceLocked|Boolesch|Gibt an, ob Benachrichtigungen blockiert werden, während ein Gerät gesperrt ist.|
|workProfileBlockAddingAccounts|Boolesch|Blockiert Benutzer vom Hinzufügen/Entfernen von Konten im Arbeitsprofil.|
|workProfileBluetoothEnableContactSharing|Boolesch|Lässt zu, dass Bluetooth-Geräte auf Unternehmenskontakte zugreifen.|
|workProfileBlockScreenCapture|Boolesch|Blockiert die Bildschirmaufnahme im Arbeitsprofil.|
|workProfileBlockCrossProfileCallerId|Boolesch|Blockiert die Anzeige der Arbeitsprofil-Rufnummernanzeige im persönlichen Profil.|
|workProfileBlockCamera|Boolesch|Blockiert die Kamera des Arbeitsprofils.|
|workProfileBlockCrossProfileContactsSearch|Boolesch|Blockiert die Verfügbarkeit der Kontakte des Arbeitsprofils im persönlichen Profil.|
|workProfileBlockCrossProfileCopyPaste|Boolesch|Boolescher Wert, der angibt, ob die Einstellung für ein Verbot von übergreifendem Kopieren und Einfügen des Profils aktiviert ist.|
|workProfileDefaultAppPermissionPolicy|[androidWorkProfileDefaultAppPermissionPolicyType](../resources/intune_deviceconfig_androidworkprofiledefaultapppermissionpolicytype.md)|Geforderter Kennworttyp. Mögliche Werte: sind `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.|
|workProfilePasswordBlockFingerprintUnlock|Boolesch|Gibt an, ob die Entsperrung durch Fingerabdruck für das Arbeitsprofil blockiert werden soll oder nicht.|
|workProfilePasswordBlockTrustAgents|Boolesch|Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agenten für das Arbeitsprofil blockiert werden sollen.|
|workProfilePasswordExpirationDays|Int32|Anzahl der Tage bis zum Ablaufen des Kennworts des Arbeitsprofils. Gültige Werte: 1 bis 365.|
|workProfilePasswordMinimumLength|Int32|Mindestlänge des Kennwort des Arbeitsprofils. Gültige Werte: 4 bis 16.|
|workProfilePasswordMinNumericCharacters|Int32|Mindestanzahl der numerische Zeichen im Kennwort des Arbeitsprofils. Gültige Werte: 1 bis 10|
|workProfilePasswordMinNonLetterCharacters|Int32|Mindestanzahl der Nicht-Buchstaben-Zeichen im Kennwort des Arbeitsprofils. Gültige Werte: 1 bis 10|
|workProfilePasswordMinLetterCharacters|Int32|Mindestanzahl der Buchstaben im Kennwort des Arbeitsprofils. Gültige Werte: 1 bis 10|
|workProfilePasswordMinLowerCaseCharacters|Int32|Mindestanzahl der Kleinbuchstaben im Kennwort des Arbeitsprofils. Gültige Werte: 1 bis 10|
|workProfilePasswordMinUpperCaseCharacters|Int32|Mindestanzahl der Großbuchstaben im Kennwort des Arbeitsprofils. Gültige Werte: 1 bis 10|
|workProfilePasswordMinSymbolCharacters|Int32|Mindestanzahl der Symbole im Kennwort des Arbeitsprofils. Gültige Werte: 1 bis 10|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt|
|workProfilePasswordPreviousPasswordBlockCount|Int32|Anzahl der zuletzt verwendeten Kennwörter des Arbeitsprofils, die nicht erneut verwendet werden dürfen. Gültige Werte: 0 bis 24.|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Anzahl der fehlgeschlagenen Anmeldeversuche, bevor ein Arbeitsprofil entfernt und alle Firmendaten gelöscht werden. Gültige Werte: 4 bis 11.|
|workProfilePasswordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|Geforderter Kennworttyp des Arbeitsprofils. Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.|
|workProfileRequirePassword|Boolesch|Entscheidet, ob ein Kennwort für ein Arbeitsprofil erforderlich ist oder nicht|
|securityRequireVerifyApps|Boolesch|Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.|



## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein aktualisiertes [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1812

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```








