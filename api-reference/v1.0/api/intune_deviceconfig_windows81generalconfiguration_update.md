# <a name="update-windows81generalconfiguration"></a>Aktualisieren von „windows81GeneralConfiguration“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).
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
|Authorization|Bearer&lt;token&gt; erforderlich|
|Accept|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer E-Mail-Konten zu Geräten hinzufügt, die keinem Microsoft-Konto zugeordnet sind.|
|applyOnlyToWindows81|Boolean|Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt. Diese Eigenschaft ist schreibgeschützt.|
|browserBlockAutofill|Boolean|Gibt an, ob AutoAusfüllen blockiert werden soll.|
|browserBlockAutomaticDetectionOfIntranetSites|Boolean|Gibt an, ob die automatische Erkennung von Intranetwebsites blockiert werden soll.|
|browserBlockEnterpriseModeAccess|Boolean|Gibt an, ob der Zugriff im Unternehmensmodus blockiert werden soll.|
|browserBlockJavaScript|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer JavaScript verwendet.|
|browserBlockPlugins|Boolean|Gibt an, ob Plug-Ins blockiert werden sollen.|
|browserBlockPopups|Boolean|Gibt an, ob Popups blockiert werden sollen.|
|browserBlockSendingDoNotTrackHeader|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer den „Do not track“-Header sendet.|
|browserBlockSingleWordEntryOnIntranetSites|Boolean|Gibt an, ob Einträge mit nur einem einzigen Wort auf Intranetwebsites blockiert werden sollen.|
|browserRequireSmartScreen|Boolean|Gibt an, ob der Benutzer den Smartscreenfilter verwenden muss.|
|browserEnterpriseModeSiteListLocation|String|Speicherort der Websiteliste für den Unternehmensmodus. Dies kann eine lokale Datei, ein lokales Netzwerk oder ein HTTP-Speicherort sein.|
|browserInternetSecurityLevel|String|Internetsicherheitsstufe. Mögliche Werte sind: `userDefined`, `medium`, `mediumHigh` und `high`.|
|browserIntranetSecurityLevel|String|Intranetsicherheitsstufe. Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.|
|browserLoggingReportLocation|String|Speicherort des Protokollierungsberichts|
|browserRequireHighSecurityForRestrictedSites|Boolean|Gibt an, ob für eingeschränkte Websites die Sicherheitsstufe „Hoch“ zwingend ist.|
|browserRequireFirewall|Boolean|Gibt an, ob eine Firewall erforderlich ist.|
|browserRequireFraudWarning|Boolean|Gibt an, ob die Funktion zur Betrugswarnung erforderlich ist.|
|browserTrustedSitesSecurityLevel|String|Sicherheitsstufe für vertrauenswürdige Websites. Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.|
|cellularBlockDataRoaming|Boolean|Gibt an, ob Datenroaming blockiert werden soll.|
|diagnosticsBlockDataSubmission|Boolean|Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.|
|passwordBlockPicturePasswordAndPin|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer einen Bildcode und eine PIN verwendet.|
|passwordExpirationDays|Int32|Zeit bis zum Ablaufen des Kennworts in Tagen|
|passwordMinimumLength|Int32|Mindestlänge des Kennworts|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt|
|passwordMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen|
|passwordPreviousPasswordBlockCount|Int32|Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss. Gültige Werte: 0 bis 24.|
|passwordRequiredType|String|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Die Anzahl von fehlgeschlagenen Anmeldeversuchen, bevor eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.|
|storageRequireDeviceEncryption|Boolean|Gibt an, ob für ein Mobilgerät Verschlüsselung gefordert wird.|
|updatesRequireAutomaticUpdates|Boolean|Gibt an, ob automatische Updates erforderlich sind.|
|userAccountControlSettings|String|Einstellungen der Benutzerkontensteuerung. Mögliche Werte sind: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming` und `neverNotify`.|
|workFoldersUrl|String|URL des Arbeitsordners.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) im Antworttext zurück.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1689

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1865

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```


