---
title: Ressourcentyp „macOSGeneralDeviceConfiguration“
description: In diesem Artikel werden die deklarierten Methoden, Eigenschaften und Beziehungen beschrieben, die von der Ressource „macOSGeneralDeviceConfiguration“ verfügbar gemacht werden.
ms.openlocfilehash: 1b46ca91e5a9648b8fa63d3d0a8b565275921c52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064078"
---
# <a name="macosgeneraldeviceconfiguration-resource-type"></a>Ressourcentyp „macOSGeneralDeviceConfiguration“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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
|id|String|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Collection von Objekten des Typs „String“|Liste der Bereich Tags für diese Instanz der Entität. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolesch|Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt. Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden. Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden. Diese Eigenschaft ist schreibgeschützt. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|compliantAppsList|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“). Diese Collection darf maximal 10.000 Elemente enthalten.|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Typ der in „compliantAppsList“ definierten Liste. Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.|
|emailInDomainSuffixes|Collection von Objekten des Typs „String“|E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.|
|passwordBlockSimple|Boolean|Unterbindet die Verwendung einfacher Kennwörter.|
|passwordExpirationDays|Int32|Zeit in Tagen bis zum Ablaufen des Kennworts|
|passwordMinimumCharacterSetCount|Int32|Anzahl von Zeichensätzen, die ein Kennwort enthalten muss. Gültige Werte: 0 bis 4.|
|passwordMinimumLength|Int32|Mindestlänge von Kennwörtern|
|passwordMinutesOfInactivityBeforeLock|Int32|Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt|
|passwordPreviousPasswordBlockCount|Int32|Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Geforderter Kennworttyp. Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.|
|passwordRequired|Boolean|Legt fest, ob ein Kennwort gefordert wird.|
|keychainBlockCloudSync|Boolesch|Gibt an, ob iCloud Schlüsselsammlung Synchronisierung blockierte (Mac OS 10.12 und höher) ist.|
|airPrintBlocked|Boolesch|Gibt an, ob AirPrint blockierte (Mac OS 10.12 und höher) ist.|
|airPrintForceTrustedTLS|Boolesch|Gibt an, ob vertrauenswürdige Zertifikate für Drucken TLS-Kommunikation (Mac OS 10.13 und höher) erforderlich sind.|
|airPrintBlockiBeaconDiscovery|Boolesch|Gibt an, ob iBeacon Ermittlung von AirPrint Drucker ausgeschlossen wird. Dies verhindert, dass falsche AirPrint Bluetooth Beacons vor Phishing für den Netzwerkdatenverkehr (Mac OS 10.3 und höher).|
|safariBlockAutofill|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer AutoAusfüllen in Safari verwendet.|
|cameraBlocked|Boolescher Wert|Gibt an, ob verhindert werden soll, dass der Benutzer auf die Kamera des Geräts zugreift.|
|iTunesBlockMusicService|Boolescher Wert|Gibt an, ob Musik Service blockieren und Musik-app im klassischen Modus zurücksetzen.|
|spotlightBlockInternetResults|Boolescher Wert|Gibt an, ob Spotlight blockieren aus einer Internet-Suche Ergebnisse zurückgegeben.|
|keyboardBlockDictation|Boolescher Wert|Gibt an, ob die Benutzer mit Dictation Input blockieren.|
|definitionLookupBlocked|Boolescher Wert|Gibt an, ob Definition Lookup blockieren.|
|appleWatchBlockAutoUnlock|Boolesch|Gibt an, ob oder blockieren Benutzer ihre Mac mit Apple Watch entsperren.|
|iTunesBlockFileSharing|Boolesch|Gibt an, ob Dateien verhindern blockieren übertragen iTunes verwenden.|
|iCloudBlockDocumentSync|Boolescher Wert|Gibt an, ob die iCloud-Dokumentsynchronisierung blockiert werden soll.|
|iCloudBlockMail|Boolesch|Gibt an, ob iCloud aus der Synchronisierung von e-Mail-Nachrichten zu blockieren.|
|iCloudBlockAddressBook|Boolesch|Gibt an, ob iCloud aus der Synchronisierung von Kontakten zu blockieren.|
|iCloudBlockCalendar|Boolesch|Gibt an, ob iCloud aus der Synchronisierung von Kalendern blockieren.|
|iCloudBlockReminders|Boolesch|Gibt an, ob iCloud aus der Synchronisierung Erinnerungen blockieren.|
|iCloudBlockBookmarks|Boolesch|Gibt an, ob iCloud von Lesezeichen synchronisieren blockieren.|
|iCloudBlockNotes|Boolesch|Gibt an, ob iCloud aus der Synchronisierung von Notizen zu blockieren.|
|airDropBlocked|Boolescher Wert|Gibt an, ob AirDrop zulassen.|
|passwordBlockModification|Boolesch|Gibt an, ob Kennung für die Änderung zu ermöglichen.|
|passwordBlockFingerprintUnlock|Boolescher Wert|Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.|

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
  "passwordBlockFingerprintUnlock": true
}
```





