# <a name="androidgeneraldeviceconfiguration-resource-type"></a>androidGeneralDeviceConfiguration-Ressourcentyp 

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „androidGeneralDeviceConfiguration“ verfügbar gemacht werden.

Erbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[androidGeneralDeviceConfigurations auflisten](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_list.md)|[androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)-Objekte.|
|[androidGeneralDeviceConfiguration abrufen](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_get.md)|[androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)-Objekts.|
|[androidGeneralDeviceConfiguration erstellen](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_create.md)|[androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)|Ein neues [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)-Objekt erstellen.|
|[androidGeneralDeviceConfiguration löschen](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_delete.md)|Keine|Löscht eine [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).|
|[androidGeneralDeviceConfiguration aktualisieren](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_update.md)|[androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)|Aktualisiert die Eigenschaften eines [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Beschreibung|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|appsBlockClipboardSharing|Boolescher Wert|Gibt an, ob die gemeinsame Nutzung der Zwischenablage zum Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.|
|appsBlockCopyPaste|Boolescher Wert|Gibt an, ob Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.|
|appsBlockYouTube|Boolescher Wert|Gibt an, ob die YouTube-App blockiert werden soll.|
|bluetoothBlocked|Boolescher Wert|Gibt an, ob Bluetooth blockiert werden soll.|
|cameraBlocked|Boolescher Wert|Gibt an, ob die Verwendung der Kamera blockiert werden soll.|
|cellularBlockDataRoaming|Boolescher Wert|Gibt an, ob Datenroaming blockiert werden soll.|
|cellularBlockMessaging|Boolescher Wert|Gibt an, ob SMS-/MMS-Nachrichten blockiert werden sollen.|
|cellularBlockVoiceRoaming|Boolescher Wert|Gibt an, ob Sprachroaming blockiert werden soll.|
|cellularBlockWifiTethering|Boolescher Wert|Gibt an, ob die Synchronisierung von WLAN-Tethering blockiert werden soll.|
|compliantAppsList|Sammlung von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)|Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“). Diese Sammlung darf maximal 10.000 Elemente enthalten.|
|compliantAppListType|Zeichenfolge|Typ der in „compliantAppsList“ definierten Liste. Mögliche Werte sind: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|diagnosticDataBlockSubmission|Boolescher Wert|Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.|
|locationServicesBlocked|Boolescher Wert|Gibt an, ob die Ortungsdienste blockiert werden sollen.|
|googleAccountBlockAutoSync|Boolescher Wert|Gibt an, ob die automatische Synchronisierung von Google-Konten blockiert werden soll.|
|googlePlayStoreBlocked|Boolescher Wert|Gibt an, ob der Google Play-Store blockiert werden soll.|
|kioskModeBlockSleepButton|Boolescher Wert|Gibt an, ob die Standbytaste im Kiosk-Modus blockiert werden soll.|
|kioskModeBlockVolumeButtons|Boolescher Wert|Gibt an, ob die Lautstärkeregler im Kiosk-Modus blockiert werden sollen.|
|kioskModeApps|Sammlung von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)|Eine Liste der Apps, die ausgeführt werden können, wenn sich das Gerät im Kiosk-Modus befindet. Diese Sammlung darf maximal 500 Elemente enthalten.|
|nfcBlocked|Boolescher Wert|Gibt an, ob NFC (Near Field Communication) blockiert werden soll.|
|passwordBlockFingerprintUnlock|Boolescher Wert|Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.|
|passwordBlockTrustAgents|Boolescher Wert|Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts. Gültige Werte: 1 bis 365.|
|passwordMinimumLength|Int32|Mindestlänge von Kennwörtern Gültige Werte: 4 bis 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt.|
|passwordPreviousPasswordBlockCount|Int32|Anzahl der zuletzt verwendeten Kennwörter nicht erneut verwendet werden dürfen. Gültige Werte: 0 bis 24.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird. Gültige Werte: 4 bis 11.|
|passwordRequiredType|Zeichenfolge|Geforderter Kennworttyp. Mögliche Werte: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.|
|passwordRequired|Boolescher Wert|Gibt an, ob ein Kennwort erforderlich ist.|
|powerOffBlocked|Boolescher Wert|Gibt an, ob das Ausschalten des Geräts blockiert werden soll.|
|factoryResetBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer Zurücksetzung auf Werkseinstellungen durchführt.|
|screenCaptureBlocked|Boolescher Wert|Gibt an, ob Screenshots blockiert werden sollen.|
|deviceSharingAllowed|Boolescher Wert|Gibt an, ob der Gerätefreigabemodus zugelassen wird.|
|storageBlockGoogleBackup|Boolescher Wert|Gibt an, ob die Google-Sicherung blockiert werden soll.|
|storageBlockRemovableStorage|Boolescher Wert|Gibt an, ob die Verwendung von Wechselmedien blockiert werden soll.|
|storageRequireDeviceEncryption|Boolescher Wert|Gibt an, ob Geräteverschlüsselung erforderlich ist.|
|storageRequireRemovableStorageEncryption|Boolescher Wert|Gibt an, ob die Wechselmedienverschlüsselung erforderlich ist.|
|voiceAssistantBlocked|Boolescher Wert|Gibt an, ob die Verwendung des Sprach-Assistenten blockiert werden soll.|
|voiceDialingBlocked|Boolescher Wert|Gibt an, ob das Sprachwahlverfahren blockiert werden soll.|
|webBrowserBlockPopups|Boolescher Wert|Gibt an, ob Popups innerhalb des Webbrowsers blockiert werden sollen.|
|webBrowserBlockAutofill|Boolescher Wert|Gibt an, ob das AutoAusfüllen-Feature blockiert werden soll.|
|webBrowserBlockJavaScript|Boolescher Wert|Gibt an, ob JavaScript im Webbrowser blockiert werden soll.|
|webBrowserBlocked|Boolescher Wert|Gibt an, ob der Webbrowser blockiert werden soll.|
|webBrowserCookieSettings|Zeichenfolge|Cookieeinstellungen in Ihrem Webbrowser. Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|wiFiBlocked|Boolescher Wert|Gibt an, ob die Synchronisierung der WLAN-Funktion blockiert werden soll.|
|appsInstallAllowList|Sammlung von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)|Liste von Apps, die auf dem KNOX-Gerät installiert werden können. Diese Sammlung darf maximal 500 Elemente enthalten.|
|appsLaunchBlockList|Sammlung von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)|Liste von Apps, die nicht auf dem KNOX-Gerät gestartet werden können. Diese Sammlung darf maximal 500 Elemente enthalten.|
|appsHideList|Sammlung von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)|Liste von Apps, die auf dem KNOX-Gerät ausgeblendet werden sollen. Diese Sammlung darf maximal 500 Elemente enthalten.|
|securityRequireVerifyApps|Boolescher Wert|Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|Sammlung von Objekten des Typs [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|Sammlung von Objekten des Typs [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|Sammlung von Objekten des Typs [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceSettingStateSummaries|Sammlung von Objekten des Typs [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "String",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "securityRequireVerifyApps": true
}
```


