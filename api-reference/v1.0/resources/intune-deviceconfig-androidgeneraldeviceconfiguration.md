---
title: 'androidGeneralDeviceConfiguration-Ressourcentyp '
description: In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „androidGeneralDeviceConfiguration“ verfügbar gemacht werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b0f3edb9d53cc42ec92d3330966cafec4bedcfa
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259521"
---
# <a name="androidgeneraldeviceconfiguration-resource-type"></a>androidGeneralDeviceConfiguration-Ressourcentyp 

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „androidGeneralDeviceConfiguration“ verfügbar gemacht werden.


Erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[androidGeneralDeviceConfigurations auflisten](../api/intune-deviceconfig-androidgeneraldeviceconfiguration-list.md)|[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md)-Objekte.|
|[androidGeneralDeviceConfiguration abrufen](../api/intune-deviceconfig-androidgeneraldeviceconfiguration-get.md)|[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md)-Objekts.|
|[androidGeneralDeviceConfiguration erstellen](../api/intune-deviceconfig-androidgeneraldeviceconfiguration-create.md)|[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md)|Ein neues [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md)-Objekt erstellen.|
|[androidGeneralDeviceConfiguration löschen](../api/intune-deviceconfig-androidgeneraldeviceconfiguration-delete.md)|Keine|Löscht eine [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).|
|[androidGeneralDeviceConfiguration aktualisieren](../api/intune-deviceconfig-androidgeneraldeviceconfiguration-update.md)|[androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md)|Aktualisiert die Eigenschaften eines [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|appsBlockClipboardSharing|Boolean|Gibt an, ob die gemeinsame Nutzung der Zwischenablage zum Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.|
|appsBlockCopyPaste|Boolean|Gibt an, ob Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.|
|appsBlockYouTube|Boolean|Gibt an, ob die YouTube-App blockiert werden soll.|
|bluetoothBlocked|Boolean|Gibt an, ob Bluetooth blockiert werden soll.|
|cameraBlocked|Boolean|Gibt an, ob die Verwendung der Kamera blockiert werden soll.|
|cellularBlockDataRoaming|Boolean|Gibt an, ob Datenroaming blockiert werden soll.|
|cellularBlockMessaging|Boolean|Gibt an, ob SMS-/MMS-Nachrichten blockiert werden sollen.|
|cellularBlockVoiceRoaming|Boolean|Gibt an, ob Sprachroaming blockiert werden soll.|
|cellularBlockWifiTethering|Boolean|Gibt an, ob die Synchronisierung von WLAN-Tethering blockiert werden soll.|
|compliantAppsList|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“). Diese Collection darf maximal 10.000 Elemente enthalten.|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Typ der in „compliantAppsList“ definierten Liste. Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.|
|diagnosticDataBlockSubmission|Boolean|Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.|
|locationServicesBlocked|Boolean|Gibt an, ob die Ortungsdienste blockiert werden sollen.|
|googleAccountBlockAutoSync|Boolean|Gibt an, ob die automatische Synchronisierung von Google-Konten blockiert werden soll.|
|googlePlayStoreBlocked|Boolescher Wert|Gibt an, ob der Google Play-Store blockiert werden soll.|
|kioskModeBlockSleepButton|Boolean|Gibt an, ob die Standbytaste im Kioskmodus blockiert werden soll.|
|kioskModeBlockVolumeButtons|Boolean|Gibt an, ob die Lautstärkeregler im Kioskmodus blockiert werden sollen.|
|kioskModeApps|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Eine Liste der Apps, die ausgeführt werden können, wenn sich das Gerät im Kioskmodus befindet. Diese Collection darf maximal 500 Elemente enthalten.|
|nfcBlocked|Boolean|Gibt an, ob NFC (Near Field Communication) blockiert werden soll.|
|passwordBlockFingerprintUnlock|Boolean|Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.|
|passwordBlockTrustAgents|Boolean|Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts. Gültige Werte: 1 bis 365.|
|passwordMinimumLength|Int32|Mindestlänge von Kennwörtern. Gültige Werte: 4 bis 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt|
|passwordPreviousPasswordBlockCount|Int32|Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen. Gültige Werte: 0 bis 24.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird. Gültige Werte 1 bis 16|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.|
|passwordRequired|Boolean|Gibt an, ob ein Kennwort erforderlich ist.|
|powerOffBlocked|Boolean|Gibt an, ob das Ausschalten des Geräts blockiert werden soll.|
|factoryResetBlocked|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer eine Zurücksetzung auf die Werkseinstellungen durchführt.|
|screenCaptureBlocked|Boolean|Gibt an, ob Screenshots blockiert werden sollen.|
|deviceSharingAllowed|Boolean|Gibt an, ob der Gerätefreigabemodus zugelassen wird.|
|storageBlockGoogleBackup|Boolean|Gibt an, ob die Google-Sicherung blockiert werden soll.|
|storageBlockRemovableStorage|Boolean|Gibt an, ob die Verwendung von Wechselmedien blockiert werden soll.|
|storageRequireDeviceEncryption|Boolean|Gibt an, ob eine Geräteverschlüsselung erforderlich ist.|
|storageRequireRemovableStorageEncryption|Boolean|Gibt an, ob die Verschlüsselung von Wechselmedien erforderlich ist.|
|voiceAssistantBlocked|Boolean|Gibt an, ob die Verwendung des Sprach-Assistenten blockiert werden soll.|
|voiceDialingBlocked|Boolean|Gibt an, ob das Sprachwahlverfahren blockiert werden soll.|
|webBrowserBlockPopups|Boolean|Gibt an, ob Popups innerhalb des Webbrowsers blockiert werden sollen.|
|webBrowserBlockAutofill|Boolean|Gibt an, ob das AutoAusfüllen-Feature des Webbrowsers blockiert werden soll.|
|webBrowserBlockJavaScript|Boolean|Gibt an, ob JavaScript im Webbrowser blockiert werden soll.|
|webBrowserBlocked|Boolean|Gibt an, ob der Webbrowser blockiert werden soll.|
|webBrowserCookieSettings|[webBrowserCookieSettings](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|Cookieeinstellungen des Webbrowsers. Mögliche Werte: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|wiFiBlocked|Boolescher Wert|Gibt an, ob die WLAN-Synchronisierung blockiert werden soll.|
|appsInstallAllowList|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Liste von Apps, die auf dem KNOX-Gerät installiert werden dürfen. Diese Collection darf maximal 500 Elemente enthalten.|
|appsLaunchBlockList|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Liste von Apps, die auf dem KNOX-Gerät nicht gestartet werden dürfen. Diese Collection darf maximal 500 Elemente enthalten.|
|appsHideList|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Liste von Apps, die auf dem KNOX-Gerät ausgeblendet werden sollen. Diese Collection darf maximal 500 Elemente enthalten.|
|securityRequireVerifyApps|Boolean|Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
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



