---
title: Ressourcentyp „defaultManagedAppProtection“
description: Diese Richtlinie wird verwendet, um detaillierte Verwaltungseinstellungen für eine festgelegte Gruppe von Apps zu konfigurieren, die für alle Benutzer greifen, die nicht unter eine Richtlinie des Typs „targetedManagedAppProtection“ fallen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: db1d82cf03e9263f3af7c4aa1cd72fe4bb2b70ff
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572481"
---
# <a name="defaultmanagedappprotection-resource-type"></a>Ressourcentyp „defaultManagedAppProtection“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Diese Richtlinie wird verwendet, um detaillierte Verwaltungseinstellungen für eine festgelegte Gruppe von Apps zu konfigurieren, die für alle Benutzer greifen, die nicht unter eine Richtlinie des Typs „targetedManagedAppProtection“ fallen.


Sie erbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „defaultManagedAppProtection“](../api/intune-mam-defaultmanagedappprotection-list.md)|Sammlung von Objekten des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) auf.|
|[Abrufen von „defaultManagedAppProtection“](../api/intune-mam-defaultmanagedappprotection-get.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|
|[Erstellen von „defaultManagedAppProtection“](../api/intune-mam-defaultmanagedappprotection-create.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Erstellt neue Objekte des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|
|[Löschen von „defaultManagedAppProtection“](../api/intune-mam-defaultmanagedappprotection-delete.md)|Keiner|Löscht Objekte des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|
|[Aktualisieren von „defaultManagedAppProtection“](../api/intune-mam-defaultmanagedappprotection-update.md)|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)|Aktualisiert die Eigenschaften von Objekten des Typs [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Anzeigename der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|Zeichenfolge|Beschreibung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz. Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|String|Schlüssel der Entität Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|Version|String|Version der Entität Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Dauer|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät nicht mit dem Internet verbunden ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOnlineBeforeAccessCheck|Dauer|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät mit dem Internet verbunden ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Quellen, von denen Daten übermittelt werden dürfen. Von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)geerbt. Mögliche Werte sind: `allApps`, `managedApps` und `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Ziele, an die Daten übermittelt werden dürfen. Von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)geerbt. Mögliche Werte: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolesch|Gibt an, ob von der Organisation bereitgestellte Anmeldeinformationen zur Nutzung der App erforderlich sind. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|Regelt die Freigabe der Zwischenablage für Apps auf dem verwalteten Gerät. Von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)geerbt. Mögliche Werte: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolesch|Gibt an, ob die Sicherung der Daten der verwalteten App blockiert werden soll. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|deviceComplianceRequired|Boolesch|Gibt an, ob Gerätekonformität erforderlich ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|managedBrowserToOpenLinksRequired|Boolesch|Gibt an, ob Internetlinks in der Managed Browser-App geöffnet werden sollen. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|saveAsBlocked|Boolesch|Gibt an, ob Benutzer das Menüelement „Speichern unter“ verwenden dürfen, um eine Kopie geschützter Dateien zu speichern. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOfflineBeforeWipeIsEnforced|Dauer|Legt fest, wie lange eine App ohne Internetverbindung sein darf, bevor sämtliche verwalteten Daten gelöscht werden. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinRequired|Boolescher Wert|Gibt an, ob eine PIN auf App-Ebene erforderlich ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|maximumPinRetries|Int32|Maximale Anzahl fehlerhafter PIN-Wiederholungsversuche, bevor die verwaltete App blockiert oder gelöscht wird. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|simplePinBlocked|Boolean|Gibt an, ob einfache PINs blockiert werden sollen. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumPinLength|Int32|Erforderliche PIN-Mindestlänge für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Zulässige Zeichensätze für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)geerbt. Mögliche Werte: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Dauer|Zeitraum, nach dem die für alle Ebenen geltende PIN zurückgesetzt werden muss, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) -Sammlung|Datenspeicherorte, an denen der Benutzer verwaltete Daten speichern darf. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|contactSyncBlocked|Boolesch|Gibt an, ob eine Synchronisierung von Kontakten mit dem Gerät des Benutzers erlaubt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|printBlocked|Boolesch|Gibt an, ob über verwaltete Apps gedruckt werden darf. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|fingerprintBlocked|Boolescher Wert|Gibt an, ob statt einer PIN der Fingerabdruckleser verwendet werden darf, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|disableAppPinIfDevicePinIsSet|Boolescher Wert|Gibt an, ob die Verwendung der App-PIN erforderlich ist, wenn die Geräte-PIN gesetzt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredOsVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningOsVersion|Zeichenfolge|Ist eine ältere Version als die angegebene Version installiert, wird in der verwalteten App die Warnmeldung angezeigt, dass kein Zugriff auf Unternehmensdaten erlaubt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredAppVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningAppVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version wird eine Warnmeldung in der verwalteten App angezeigt. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWipeOsVersion|Zeichenfolge|Versionen, die kleiner als oder gleich der angegebenen Version sind, wischen die verwaltete APP und die zugehörigen Unternehmensdaten ab. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWipeAppVersion|Zeichenfolge|Versionen, die kleiner als oder gleich der angegebenen Version sind, wischen die verwaltete APP und die zugehörigen Unternehmensdaten ab. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Definiert ein verwaltetes App-Verhalten, entweder Block oder Wipe, wenn das Gerät Rooted oder jailbroken ist, wenn DeviceComplianceRequired auf true festgelegt ist. Von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)geerbt. Mögliche Werte sind: `block`, `wipe` und `warn`.|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Definiert ein verwaltetes App-Verhalten, entweder Block oder Wipe, basierend auf der maximalen Anzahl fehlerhafter PIN-Wiederholungsversuche. Von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)geerbt. Mögliche Werte sind: `block`, `wipe` und `warn`.|
|pinRequiredInsteadOfBiometricTimeout|Dauer|Timeout in Minuten für eine APP-Pin anstelle von nicht-Biometrie-Kennungen, die von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md) geerbt wurden|
|allowedOutboundClipboardSharingExceptionLength|Int32|Geben Sie die Anzahl von Zeichen an, die aus org-Daten und-Konten in eine beliebige Anwendung Ausschneiden oder kopiert werden dürfen. Diese Einstellung überschreibt die AllowedOutboundClipboardSharingLevel-Einschränkung. Der Standardwert "0" bedeutet, dass keine Ausnahme zulässig ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|Typ der Verschlüsselung, die auf Daten in einer verwalteten App angewendet werden soll. (nur iOS). Mögliche Werte sind: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles` und `whenDeviceLocked`.|
|screenCaptureBlocked|Boolesch|Gibt an, ob Screenshots blockiert werden sollen. (nur Android)|
|encryptAppData|Boolean|Gibt an, ob die Daten verwalteter Apps verschlüsselt werden sollen. (nur Android)|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolesch|Wenn diese Einstellung aktiviert ist, ist die Verschlüsselung auf App-Ebene deaktiviert, wenn die Verschlüsselung auf Geräteebene aktiviert ist. (nur Android)|
|minimumRequiredSdkVersion|String|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert. (nur iOS)|
|customSettings|Collection von Objekten des Typs [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an die von der Richtlinie betroffenen Benutzer gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst.|
|deployedAppCount|Int32|Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde|
|minimumRequiredPatchVersion|Zeichenfolge|Legt das älteste erforderliche Android-Sicherheitspatchlevel fest, mit dem einem Benutzer noch sicherer Zugriff auf die App gewährt wird. (nur Android)|
|minimumWarningPatchVersion|String|Legt das älteste empfohlene Android-Sicherheitspatchlevel fest, mit dem einem Benutzer noch sicherer Zugriff auf die App gewährt wird. (nur Android)|
|exemptedAppProtocols|[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung|iOS-apps in dieser Liste sind von der Richtlinie ausgenommen und können Daten von verwalteten apps empfangen. (nur iOS)|
|exemptedAppPackages|[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung|Android-App-Pakete in dieser Liste sind von der Richtlinie ausgenommen und können Daten von verwalteten apps empfangen. (nur Android)|
|faceIdBlocked|Boolean|Gibt an, ob statt einer PIN die Face ID verwendet werden darf, wenn „pinRequired“ auf „true“ gesetzt ist. (nur iOS)|
|Eigenschaften minimumwipesdkversion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert.|
|minimumWipePatchVersion|Zeichenfolge|Die Android-Sicherheits Patchebene, die kleiner oder gleich dem angegebenen Wert ist, wischt die verwaltete APP und die zugehörigen Unternehmensdaten ab. (nur Android)|
|allowedIosDeviceModels|Zeichenfolge|Durch Semikolons getrennte Liste der Gerätemodelle, die als Zeichenfolge zulässig sind, damit die verwaltete APP funktioniert. (nur iOS)|
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Definiert ein verwaltetes App-Verhalten, entweder Block oder Wipe, wenn das angegebene Gerätemodell nicht zulässig ist. (nur iOS). Mögliche Werte sind: `block`, `wipe` und `warn`.|
|allowedAndroidDeviceManufacturers|Zeichenfolge|Durch Semikolons getrennte Liste der Gerätehersteller, die als Zeichenfolge zulässig sind, damit die verwaltete APP funktioniert. (nur Android)|
|Appactionifandroiddevicemanufacturernotallowed zur|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Definiert ein verwaltetes App-Verhalten, entweder blockieren oder löschen, wenn der angegebene Gerätehersteller nicht zulässig ist. (Nur Android). Mögliche Werte sind: `block`, `wipe` und `warn`.|
|thirdPartyKeyboardsBlocked|Boolesch|Definiert, ob Drittanbieter-Tastaturen beim Zugriff auf eine verwaltete App zulässig sind. (nur iOS)|
|filterOpenInToOnlyManagedApps|Boolesch|Definiert, ob der Open-in-Vorgang von der verwalteten APP zu den ausgewählten Filesharing-Speicherorten unterstützt wird. Diese Einstellung gilt nur, wenn AllowedOutboundDataTransferDestinations auf ManagedApps und DisableProtectionOfManagedOutboundOpenInData auf false festgelegt ist. (nur iOS)|
|disableProtectionOfManagedOutboundOpenInData|Boolesch|Deaktivieren des Schutzes von Daten, die über die IOS openin-Option an andere apps übertragen werden. Diese Einstellung ist nur zulässig, wenn AllowedOutboundDataTransferDestinations auf ManagedApps festgelegt ist. (nur iOS)|
|Protectinbounddatafromunknownsources zur|Boolesch|Schützen Sie eingehende Daten aus unbekannten Quellen. Diese Einstellung ist nur zulässig, wenn AllowedInboundDataTransferSources auf allApps festgelegt ist. (nur iOS)|
|requiredAndroidSafetyNetDeviceAttestationType|[androidManagedAppSafetyNetDeviceAttestationType](../resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)|Definiert die Android-SafetyNet-Geräte Bescheinigungs Anforderung für eine verwaltete app. Mögliche Werte sind: `none`, `basicIntegrity` und `basicIntegrityAndDeviceCertification`.|
|appActionIfAndroidSafetyNetDeviceAttestationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Definiert ein verwaltetes App-Verhalten, entweder warnen oder blockieren, wenn die angegebene Android-SafetyNet-Bestätigungs requirment fehlschlägt. Mögliche Werte sind: `block`, `wipe` und `warn`.|
|requiredAndroidSafetyNetAppsVerificationType|[androidManagedAppSafetyNetAppsVerificationType](../resources/intune-mam-androidmanagedappsafetynetappsverificationtype.md)|Definiert die Android-SafetyNet-apps-Verifizierungs Anforderung für eine verwaltete app. Mögliche Werte sind: `none` und `enabled`.|
|appActionIfAndroidSafetyNetAppsVerificationFailed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Definiert ein verwaltetes App-Verhalten, entweder warnen oder blockieren, wenn der angegebene Android-requirment fehlschlägt. Mögliche Werte sind: `block`, `wipe` und `warn`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|apps|Sammlung von Objekten des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Liste der Apps, für die die Richtlinie bereitgestellt wurde|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Navigationseigenschaft zu einer Bereitstellungsübersicht für die Konfiguration|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": true,
  "maximumPinRetries": 1024,
  "simplePinBlocked": true,
  "minimumPinLength": 1024,
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String",
  "minimumWipeOsVersion": "String",
  "minimumWipeAppVersion": "String",
  "appActionIfDeviceComplianceRequired": "String",
  "appActionIfMaximumPinRetriesExceeded": "String",
  "pinRequiredInsteadOfBiometricTimeout": "String (duration)",
  "allowedOutboundClipboardSharingExceptionLength": 1024,
  "appDataEncryptionType": "String",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "String",
  "minimumWipePatchVersion": "String",
  "allowedIosDeviceModels": "String",
  "appActionIfIosDeviceModelNotAllowed": "String",
  "allowedAndroidDeviceManufacturers": "String",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true,
  "requiredAndroidSafetyNetDeviceAttestationType": "String",
  "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
  "requiredAndroidSafetyNetAppsVerificationType": "String",
  "appActionIfAndroidSafetyNetAppsVerificationFailed": "String"
}
```




