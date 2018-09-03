# <a name="windows81generalconfiguration-resource-type"></a>windows81GeneralConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „windows81GeneralConfiguration“ verfügbar gemacht werden.

Sie erbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[windows81GeneralConfigurations auflisten](../api/intune_deviceconfig_windows81generalconfiguration_list.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)-Sammlung|Listet die Eigenschaften und Beziehungen von [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)-Objekten auf.|
|[windows81GeneralConfiguration abrufen](../api/intune_deviceconfig_windows81generalconfiguration_get.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|Liest die Eigenschaften und Beziehungen des [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)-Objekts auf.|
|[windows81GeneralConfiguration erstellen](../api/intune_deviceconfig_windows81generalconfiguration_create.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|Erstellt ein neues [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)-Objekt.|
|[windows81GeneralConfiguration löschen](../api/intune_deviceconfig_windows81generalconfiguration_delete.md)|Keine|Löscht eine [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).|
|[windows81GeneralConfiguration aktualisieren](../api/intune_deviceconfig_windows81generalconfiguration_update.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|Aktualisiert die Eigenschaften eines [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer E-Mail-Konten zu Geräten hinzufügt, die keinem Microsoft-Konto zugeordnet sind.|
|applyOnlyToWindows81|Boolescher Wert|Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt. Diese Eigenschaft ist schreibgeschützt.|
|browserBlockAutofill|Boolescher Wert|Gibt an, ob AutoAusfüllen blockiert werden soll.|
|browserBlockAutomaticDetectionOfIntranetSites|Boolescher Wert|Gibt an, ob die automatische Erkennung von Intranetwebsites blockiert werden soll.|
|browserBlockEnterpriseModeAccess|Boolescher Wert|Gibt an, ob der Zugriff im Unternehmensmodus blockiert werden soll.|
|browserBlockJavaScript|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer JavaScript verwendet.|
|browserBlockPlugins|Boolescher Wert|Gibt an, ob Plug-Ins blockiert werden sollen.|
|browserBlockPopups|Boolescher Wert|Gibt an, ob Popups blockiert werden sollen.|
|browserBlockSendingDoNotTrackHeader|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer den „Do not track“-Header sendet.|
|browserBlockSingleWordEntryOnIntranetSites|Boolescher Wert|Gibt an, ob Einträge mit nur einem einzigen Wort auf Intranetwebsites blockiert werden sollen.|
|browserRequireSmartScreen|Boolescher Wert|Gibt an, ob der Benutzer den Smartscreenfilter verwenden muss.|
|browserEnterpriseModeSiteListLocation|Zeichenfolge|Speicherort der Websiteliste für den Unternehmensmodus. Dies kann eine lokale Datei, ein lokales Netzwerk oder ein HTTP-Speicherort sein.|
|browserInternetSecurityLevel|[internetSiteSecurityLevel](../resources/intune_deviceconfig_internetsitesecuritylevel.md)|Internetsicherheitsstufe. Die möglichen Werte sind: `userDefined`, `medium`, `mediumHigh`, `high`.|
|browserIntranetSecurityLevel|[siteSecurityLevel](../resources/intune_deviceconfig_sitesecuritylevel.md)|Intranetsicherheitsstufe. Die mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.|
|browserLoggingReportLocation|Zeichenfolge|Speicherort des Protokollierungsberichts|
|browserRequireHighSecurityForRestrictedSites|Boolescher Wert|Gibt an, ob für eingeschränkte Websites die Sicherheitsstufe „Hoch“ zwingend ist.|
|browserRequireFirewall|Boolescher Wert|Gibt an, ob eine Firewall erforderlich ist.|
|browserRequireFraudWarning|Boolescher Wert|Gibt an, ob die Funktion zur Betrugswarnung erforderlich ist.|
|browserTrustedSitesSecurityLevel|[siteSecurityLevel](../resources/intune_deviceconfig_sitesecuritylevel.md)|Sicherheitsstufe für vertrauenswürdige Websites. Die mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.|
|cellularBlockDataRoaming|Boolescher Wert|Gibt an, ob Datenroaming blockiert werden soll.|
|diagnosticsBlockDataSubmission|Boolescher Wert|Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.|
|passwordBlockPicturePasswordAndPin|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer einen Bildcode und eine PIN verwendet.|
|passwordExpirationDays|Int32|Zeit bis zum Ablaufen des Kennworts in Tagen|
|passwordMinimumLength|Int32|Mindestlänge des Kennworts|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt|
|passwordMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen|
|passwordPreviousPasswordBlockCount|Int32|Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss. Gültige Werte: 0 bis 24.|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|Geforderter Kennworttyp. Die möglichen Werte sind: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Die Anzahl von fehlgeschlagenen Anmeldeversuchen, bevor eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.|
|storageRequireDeviceEncryption|Boolescher Wert|Gibt an, ob für ein Mobilgerät Verschlüsselung gefordert wird.|
|updatesRequireAutomaticUpdates|Boolescher Wert|Gibt an, ob automatische Updates erforderlich sind.|
|userAccountControlSettings|[windowsUserAccountControlSettings](../resources/intune_deviceconfig_windowsuseraccountcontrolsettings.md)|Einstellungen der Benutzerkontensteuerung. Die möglichen Werte sind: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.|
|workFoldersUrl|Zeichenfolge|Die URL des Arbeitsordners.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.deviceConfiguration",
  "@odata.type": "microsoft.graph.windows81GeneralConfiguration",
  "@odata.annotations": [
    {
      "property": "applyOnlyToWindows81",
      "capabilities": {
        "computed": true,
        "permissions": "Read"
      }
    }
  ]
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
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
  "browserEnterpriseModeSiteListLocation": "String",
  "browserInternetSecurityLevel": "String",
  "browserIntranetSecurityLevel": "String",
  "browserLoggingReportLocation": "String",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "String",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "String",
  "workFoldersUrl": "String"
}
```



