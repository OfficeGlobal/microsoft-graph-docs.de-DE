---
title: Ressourcentyp „macOSGeneralDeviceConfiguration“
description: In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „macOSGeneralDeviceConfiguration“ verfügbar gemacht werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8fadc8f8aa91caec0596650765c1feada58cecc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146242"
---
# <a name="macosgeneraldeviceconfiguration-resource-type"></a>Ressourcentyp „macOSGeneralDeviceConfiguration“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „macOSGeneralDeviceConfiguration“ verfügbar gemacht werden.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „macOSGeneralDeviceConfiguration“](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-list.md)|Sammlung von Objekten des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) auf.|
|[Abrufen von „macOSGeneralDeviceConfiguration“](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-get.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Erstellen von „macOSGeneralDeviceConfiguration“](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-create.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Erstellt neue Objekte des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Löschen von „macOSGeneralDeviceConfiguration“](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-delete.md)|Keiner|Löscht Objekte des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Aktualisieren von „macOSGeneralDeviceConfiguration“](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-update.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Aktualisiert die Eigenschaften von Objekten des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolescher Wert|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt. Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind. Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|compliantAppsList|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“). Diese Collection darf maximal 10.000 Elemente enthalten.|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Typ der in „compliantAppsList“ definierten Liste. Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.|
|emailInDomainSuffixes|String collection|E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.|
|passwordBlockSimple|Boolean|Unterbindet die Verwendung einfacher Kennwörter.|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts|
|passwordMinimumCharacterSetCount|Int32|Anzahl von Zeichensätzen, die ein Kennwort enthalten muss. Gültige Werte: 0 bis 4.|
|passwordMinimumLength|Int32|Mindestlänge von Kennwörtern|
|passwordMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt|
|passwordPreviousPasswordBlockCount|Int32|Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passwordRequired|Boolescher Wert|Legt fest, ob ein Kennwort gefordert wird.|
|keychainBlockCloudSync|Boolescher Wert|Gibt an, ob die iCloud-Schlüsselbund Synchronisierung blockiert ist (macOS 10,12 und höher).|
|airPrintBlocked|Boolescher Wert|Gibt an, ob der druckDruck blockiert ist (macOS 10,12 und höher).|
|airPrintForceTrustedTLS|Boolescher Wert|Gibt an, ob vertrauenswürdige Zertifikate für die TLS-Druckkommunikation erforderlich sind (macOS 10,13 und höher).|
|airPrintBlockiBeaconDiscovery|Boolescher Wert|Gibt an, ob die iBeacon-Erkennung von Druckern blockiert wird. Dadurch wird verhindert, dass falsche druckfunk-Bluetooth-Baken für Netzwerkdatenverkehr von Phishing (macOS 10,3 und höher).|
|safariBlockAutofill|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.|
|cameraBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.|
|iTunesBlockMusicService|Boolescher Wert|Gibt an, ob der Musikdienst blockiert und die Musik-app im klassischen Modus wiederhergestellt werden soll.|
|spotlightBlockInternetResults|Boolescher Wert|Gibt an, ob Spotlight die Rückgabe von Ergebnissen aus einer Internet Suche blockieren soll.|
|keyboardBlockDictation|Boolescher Wert|Gibt an, ob die Verwendung der Diktat Eingabe durch den Benutzer blockiert werden soll.|
|definitionLookupBlocked|Boolescher Wert|Gibt an, ob die Definitions Suche blockiert werden soll.|
|appleWatchBlockAutoUnlock|Boolescher Wert|Gibt an, ob Benutzer das Aufheben der Sperre für Ihren Mac mit Apple Watch blockieren möchten.|
|iTunesBlockFileSharing|Boolescher Wert|Gibt an, ob das Übertragen von Dateien mithilfe von iTunes verhindert werden soll.|
|iCloudBlockDocumentSync|Boolescher Wert|Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.|
|iCloudBlockMail|Boolescher Wert|Gibt an, ob die Synchronisierung von e-Mails durch iCloud blockiert werden soll.|
|iCloudBlockAddressBook|Boolescher Wert|Gibt an, ob die Synchronisierung von Kontakten durch iCloud verhindert werden soll.|
|iCloudBlockCalendar|Boolescher Wert|Gibt an, ob das Synchronisieren von Kalendern für iCloud verhindert werden soll.|
|iCloudBlockReminders|Boolescher Wert|Gibt an, ob das Synchronisieren von Erinnerungen durch iCloud verhindert werden soll.|
|iCloudBlockBookmarks|Boolescher Wert|Gibt an, ob das Synchronisieren von Textmarken durch iCloud verhindert werden soll.|
|iCloudBlockNotes|Boolescher Wert|Gibt an, ob das Synchronisieren von Notizen durch iCloud verhindert werden soll.|
|airDropBlocked|Boolescher Wert|Gibt an, ob das abLegen zugelassen werden soll.|
|passwordBlockModification|Boolescher Wert|Gibt an, ob die Änderung von Passwörtern zulässig ist.|
|passwordBlockFingerprintUnlock|Boolean|Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.|
|passwordBlockAutoFill|Boolescher Wert|Gibt an, ob das Feature AutoFill passwords blockiert werden soll.|
|passwordBlockProximityRequests|Boolescher Wert|Gibt an, ob das Anfordern von Kennwörtern von benachbarten Geräten blockiert werden soll.|
|passwordBlockAirDropSharing|Boolescher Wert|Gibt an, ob das Freigeben von Kennwörtern mit der Funktion für Kennwörter blockiert werden soll.|
|softwareUpdatesEnforcedDelayInDays|Int32|Legt fest, wie viele Tage ein Software Update für ein überwachte Gerät delyed wird. Gültige Werte: 0 bis 90.|
|softwareUpdatesForceDelayed|Boolescher Wert|Gibt an, ob die Benutzersicht barkeit von Softwareupdates verzögert werden soll, wenn sich das Gerät im überwachten Modus befindet.|
|contentCachingBlocked|Boolescher Wert|Gibt an, ob das Zwischenspeichern von Inhalten zulässig ist.|

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
  "@odata.type": "microsoft.graph.macOSGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
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
  "emailInDomainSuffixes": [
    "String"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 1024,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true
}
```




