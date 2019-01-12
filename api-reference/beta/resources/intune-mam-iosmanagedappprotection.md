---
title: Ressourcentyp „iosManagedAppProtection“
description: Diese Richtlinie wird verwendet, um detaillierte Verwaltungseinstellungen für bestimmte Sicherheitsgruppen sowie für festgelegte Gruppen von Apps auf einem iOS-Gerät zu konfigurieren.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0834b335df5188f1db0cf245d3911a40b2837522
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912722"
---
# <a name="iosmanagedappprotection-resource-type"></a>Ressourcentyp „iosManagedAppProtection“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Richtlinie wird verwendet, um detaillierte Verwaltungseinstellungen für bestimmte Sicherheitsgruppen sowie für festgelegte Gruppen von Apps auf einem iOS-Gerät zu konfigurieren.

Sie erbt von [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „iosManagedAppProtection“](../api/intune-mam-iosmanagedappprotection-list.md)|Sammlung von Objekten des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) auf.|
|[Abrufen von „iosManagedAppProtection“](../api/intune-mam-iosmanagedappprotection-get.md)|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).|
|[Erstellen von „iosManagedAppProtection“](../api/intune-mam-iosmanagedappprotection-create.md)|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|Erstellt neue Objekte des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).|
|[Löschen von „iosManagedAppProtection“](../api/intune-mam-iosmanagedappprotection-delete.md)|Keiner|Löscht Objekte des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).|
|[Aktualisieren von „iosManagedAppProtection“](../api/intune-mam-iosmanagedappprotection-update.md)|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)|Aktualisiert die Eigenschaften von Objekten des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Anzeigename der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|Zeichenfolge|Beschreibung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|Version|Zeichenfolge|Version der Entität Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Duration|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät nicht mit dem Internet verbunden ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOnlineBeforeAccessCheck|Duration|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät mit dem Internet verbunden ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Quellen, von denen Daten übermittelt werden dürfen. Geerbt von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md). Mögliche Werte: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Ziele, an die Daten übermittelt werden dürfen. Geerbt von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md). Mögliche Werte: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolescher Wert|Gibt an, ob von der Organisation bereitgestellte Anmeldeinformationen zur Nutzung der App erforderlich sind. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|Regelt die Freigabe der Zwischenablage für Apps auf dem verwalteten Gerät. Geerbt von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md). Mögliche Werte: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolescher Wert|Gibt an, ob die Sicherung der Daten der verwalteten App blockiert werden soll. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|deviceComplianceRequired|Boolescher Wert|Gibt an, ob Gerätekonformität erforderlich ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|managedBrowserToOpenLinksRequired|Boolescher Wert|Gibt an, ob Internetlinks in der Managed Browser-App geöffnet werden sollen. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|saveAsBlocked|Boolescher Wert|Gibt an, ob Benutzer das Menüelement „Speichern unter“ verwenden dürfen, um eine Kopie geschützter Dateien zu speichern. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOfflineBeforeWipeIsEnforced|Duration|Legt fest, wie lange eine App ohne Internetverbindung sein darf, bevor sämtliche verwalteten Daten gelöscht werden. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinRequired|Boolescher Wert|Gibt an, ob eine PIN auf App-Ebene erforderlich ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|maximumPinRetries|Int32|Maximale Anzahl von falsche Pin "Wiederholen" versucht, bevor die verwaltete app blockiert oder Kennworteingaben gelöscht wird. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|simplePinBlocked|Boolescher Wert|Gibt an, ob einfache PINs blockiert werden sollen. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumPinLength|Int32|Erforderliche PIN-Mindestlänge für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Zulässige Zeichensätze für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md). Mögliche Werte: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duration|Zeitraum, nach dem die für alle Ebenen geltende PIN zurückgesetzt werden muss, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedDataStorageLocations|[ManagedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) -Auflistung|Datenspeicherorte, an denen der Benutzer verwaltete Daten speichern darf. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|contactSyncBlocked|Boolescher Wert|Gibt an, ob eine Synchronisierung von Kontakten mit dem Gerät des Benutzers erlaubt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|printBlocked|Boolescher Wert|Gibt an, ob aus verwalteten Apps gedruckt werden darf.
 Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|fingerprintBlocked|Boolescher Wert|Gibt an, ob statt einer PIN der Fingerabdruckleser verwendet werden darf, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|disableAppPinIfDevicePinIsSet|Boolescher Wert|Gibt an, ob die Verwendung der App-PIN erforderlich ist, wenn die Geräte-PIN gesetzt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredOsVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningOsVersion|Zeichenfolge|Ist eine ältere Version als die angegebene Version installiert, wird in der verwalteten App die Warnmeldung angezeigt, dass kein Zugriff auf Unternehmensdaten erlaubt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredAppVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningAppVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version wird eine Warnmeldung in der verwalteten App angezeigt. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWipeOsVersion|Zeichenfolge|Die Versionen kleiner oder gleich der angegebenen Version der verwalteten app und den zugehörigen Mandantendaten Wischen wird. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWipeAppVersion|Zeichenfolge|Die Versionen kleiner oder gleich der angegebenen Version der verwalteten app und den zugehörigen Mandantendaten Wischen wird. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|appActionIfDeviceComplianceRequired|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Definiert ein Verhalten verwalteten app blockieren oder Wischen, wenn das Gerät entweder Ausgangspunkt oder Jailbroken, wenn DeviceComplianceRequired festgelegt ist auf "true". Geerbt von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md). Mögliche Werte sind: `block` und `wipe`.|
|appActionIfMaximumPinRetriesExceeded|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Definiert eine verwaltete app Verhalten, entweder blockieren oder Wischen, basierend auf die maximale Anzahl der Wiederholungsversuche falsche Pin. Geerbt von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md). Mögliche Werte sind: `block` und `wipe`.|
|pinRequiredInsteadOfBiometricTimeout|Duration|Timeout für eine app Pin anstelle von nicht Biometrik Kennung Inherited aus [ManagedAppProtection](../resources/intune-mam-managedappprotection.md) in Minuten|
|isAssigned|Boolescher Wert|Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde. Geerbt von [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).|
|targetedAppManagementLevels|[appManagementLevel](../resources/intune-mam-appmanagementlevel.md)|Die vorgesehene app Management Ebenen für diese Richtlinie Inherited aus [TargetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md). Mögliche Werte: sind `unspecified`, `unmanaged`, `mdm` und `androidEnterprise`.|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune-mam-managedappdataencryptiontype.md)|Typ der Verschlüsselung, die auf Daten in einer verwalteten App angewendet werden soll. Mögliche Werte: sind `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles` und `whenDeviceLocked`.|
|minimumRequiredSdkVersion|String|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert.|
|deployedAppCount|Int32|Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde|
|faceIdBlocked|Boolean|Gibt an, ob statt einer PIN die Face ID verwendet werden darf, wenn „pinRequired“ auf „true“ gesetzt ist.|
|exemptedAppProtocols|[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung|Apps in dieser Liste werden aus der Richtlinie ausgenommen und Daten von verwalteten apps empfangen werden.|
|minimumWipeSdkVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert.|
|allowedIosDeviceModels|Zeichenfolge|Durch Semikolons getrennte Liste der Gerätemodelle zulässig als Zeichenfolge für die verwaltete app funktioniert.|
|appActionIfIosDeviceModelNotAllowed|[managedAppRemediationAction](../resources/intune-mam-managedappremediationaction.md)|Definiert ein Verhalten verwalteten app blockieren oder Wischen, wenn das angegebene Gerätemodell nicht zulässig ist. Mögliche Werte sind: `block` und `wipe`.|
|thirdPartyKeyboardsBlocked|Boolescher Wert|Legt fest, ob beim Zugriff auf einen verwalteten app Drittanbieter Tastaturen zulässig sind|
|filterOpenInToOnlyManagedApps|Boolescher Wert|Legt fest, ob öffnen in Vorgang an die ausgewählten Signalen erhält Speicherorte aus der verwalteten app unterstützt wird. Diese Einstellung gilt nur, wenn AllowedOutboundDataTransferDestinations auf ManagedApps festgelegt ist und DisableProtectionOfManagedOutboundOpenInData auf False festgelegt ist.|
|disableProtectionOfManagedOutboundOpenInData|Boolescher Wert|Deaktivieren Sie den Schutz von Daten an andere apps über IOS OpenIn Option übertragen. Diese Einstellung ist nur zulässig, true zurück, wenn AllowedOutboundDataTransferDestinations auf ManagedApps festgelegt ist.|
|protectInboundDataFromUnknownSources|Boolescher Wert|Schützen Sie eingehende Daten von unbekannten Quelle. Diese Einstellung ist nur zulässig, true zurück, wenn AllowedInboundDataTransferSources auf AllApps festgelegt ist.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|Sammlung von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Navigationseigenschaft zu einer Liste von Einschlussgruppen und Ausschlussgruppen, für die die Richtlinie bereitgestellt wurde. Geerbt von [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).|
|apps|Sammlung von Objekten des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Liste der Apps, für die die Richtlinie bereitgestellt wurde|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Navigationseigenschaft zu einer Bereitstellungsübersicht für die Konfiguration|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
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
  "isAssigned": true,
  "targetedAppManagementLevels": "String",
  "appDataEncryptionType": "String",
  "minimumRequiredSdkVersion": "String",
  "deployedAppCount": 1024,
  "faceIdBlocked": true,
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "minimumWipeSdkVersion": "String",
  "allowedIosDeviceModels": "String",
  "appActionIfIosDeviceModelNotAllowed": "String",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true
}
```





