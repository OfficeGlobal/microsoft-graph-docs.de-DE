---
title: windows81GeneralConfiguration-Ressourcentyp
description: In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „windows81GeneralConfiguration“ verfügbar gemacht werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de99fdccd10d0594dc8e7ae798640163f46da011
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262398"
---
# <a name="windows81generalconfiguration-resource-type"></a>windows81GeneralConfiguration-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „windows81GeneralConfiguration“ verfügbar gemacht werden.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[windows81GeneralConfigurations auflisten](../api/intune-deviceconfig-windows81generalconfiguration-list.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)-Sammlung|Listet die Eigenschaften und Beziehungen von [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)-Objekten auf.|
|[windows81GeneralConfiguration abrufen](../api/intune-deviceconfig-windows81generalconfiguration-get.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|Liest die Eigenschaften und Beziehungen des [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)-Objekts auf.|
|[windows81GeneralConfiguration erstellen](../api/intune-deviceconfig-windows81generalconfiguration-create.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|Erstellt ein neues [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)-Objekt.|
|[windows81GeneralConfiguration löschen](../api/intune-deviceconfig-windows81generalconfiguration-delete.md)|Keine|Löscht eine [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).|
|[windows81GeneralConfiguration aktualisieren](../api/intune-deviceconfig-windows81generalconfiguration-update.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|Aktualisiert die Eigenschaften eines [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
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
|browserRequireSmartScreen|Boolescher Wert|Gibt an, ob der Benutzer den Smartscreenfilter verwenden muss.|
|browserEnterpriseModeSiteListLocation|String|Speicherort der Websiteliste für den Unternehmensmodus. Dies kann eine lokale Datei, ein lokales Netzwerk oder ein HTTP-Speicherort sein.|
|browserInternetSecurityLevel|[internetSiteSecurityLevel](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|Internetsicherheitsstufe. Mögliche Werte: `userDefined`, `medium`, `mediumHigh`, `high`.|
|browserIntranetSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|Intranetsicherheitsstufe. Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.|
|browserLoggingReportLocation|Zeichenfolge|Speicherort des Protokollierungsberichts|
|browserRequireHighSecurityForRestrictedSites|Boolean|Gibt an, ob für eingeschränkte Websites die Sicherheitsstufe „Hoch“ zwingend ist.|
|browserRequireFirewall|Boolean|Gibt an, ob eine Firewall erforderlich ist.|
|browserRequireFraudWarning|Boolean|Gibt an, ob die Funktion zur Betrugswarnung erforderlich ist.|
|browserTrustedSitesSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|Sicherheitsstufe für vertrauenswürdige Websites. Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.|
|cellularBlockDataRoaming|Boolean|Gibt an, ob Datenroaming blockiert werden soll.|
|diagnosticsBlockDataSubmission|Boolean|Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.|
|passwordBlockPicturePasswordAndPin|Boolean|Gibt an, ob verhindert werden soll, dass der Benutzer einen Bildcode und eine PIN verwendet.|
|passwordExpirationDays|Int32|Zeit bis zum Ablaufen des Kennworts in Tagen|
|passwordMinimumLength|Int32|Mindestlänge des Kennworts|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt|
|passwordMinimumCharacterSetCount|Int32|Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen|
|passwordPreviousPasswordBlockCount|Int32|Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss. Gültige Werte: 0 bis 24.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Die Anzahl von fehlgeschlagenen Anmeldeversuchen, bevor eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.|
|storageRequireDeviceEncryption|Boolean|Gibt an, ob für ein Mobilgerät Verschlüsselung gefordert wird.|
|updatesRequireAutomaticUpdates|Boolescher Wert|Gibt an, ob automatische Updates erforderlich sind.|
|userAccountControlSettings|[windowsUserAccountControlSettings](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|Einstellungen der Benutzerkontensteuerung. Mögliche Werte: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.|
|workFoldersUrl|Zeichenfolge|Die URL des Arbeitsordners.|

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
  "@odata.type": "microsoft.graph.windows81GeneralConfiguration"
}
-->
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



