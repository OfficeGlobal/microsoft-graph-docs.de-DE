---
title: Ressourcentyp „androidManagedAppProtection“
description: Diese Richtlinie wird verwendet, um detaillierte Verwaltungseinstellungen für bestimmte Sicherheitsgruppen sowie für festgelegte Gruppen von Apps auf einem Android-Gerät zu konfigurieren.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46de406d0f82e18b93f91d1e1919b1a4353e4ca2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256595"
---
# <a name="androidmanagedappprotection-resource-type"></a>Ressourcentyp „androidManagedAppProtection“

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Diese Richtlinie wird verwendet, um detaillierte Verwaltungseinstellungen für bestimmte Sicherheitsgruppen sowie für festgelegte Gruppen von Apps auf einem Android-Gerät zu konfigurieren.


Sie erbt von [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „androidManagedAppProtection“](../api/intune-mam-androidmanagedappprotection-list.md)|Sammlung von Objekten des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) auf.|
|[Abrufen von „androidManagedAppProtection“](../api/intune-mam-androidmanagedappprotection-get.md)|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).|
|[Erstellen von „androidManagedAppProtection“](../api/intune-mam-androidmanagedappprotection-create.md)|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)|Erstellt neue Objekte des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).|
|[Löschen von „androidManagedAppProtection“](../api/intune-mam-androidmanagedappprotection-delete.md)|Keiner|Löscht Objekte des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).|
|[Aktualisieren von „androidManagedAppProtection“](../api/intune-mam-androidmanagedappprotection-update.md)|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)|Aktualisiert die Eigenschaften von Objekten des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Anzeigename der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|Zeichenfolge|Beschreibung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|string|Schlüssel der Entität Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|Version|Zeichenfolge|Version der Entität Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Dauer|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät nicht mit dem Internet verbunden ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOnlineBeforeAccessCheck|Dauer|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät mit dem Internet verbunden ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Quellen, von denen Daten übermittelt werden dürfen. Von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)geerbt. Mögliche Werte sind: `allApps`, `managedApps` und `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Ziele, an die Daten übermittelt werden dürfen. Von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)geerbt. Mögliche Werte: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean|Gibt an, ob von der Organisation bereitgestellte Anmeldeinformationen zur Nutzung der App erforderlich sind. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|Regelt die Freigabe der Zwischenablage für Apps auf dem verwalteten Gerät. Von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)geerbt. Mögliche Werte: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean|Gibt an, ob die Sicherung der Daten der verwalteten App blockiert werden soll. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|deviceComplianceRequired|Boolean|Gibt an, ob Gerätekonformität erforderlich ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|managedBrowserToOpenLinksRequired|Boolean|Gibt an, ob Internetlinks in der Managed Browser-App geöffnet werden sollen. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|saveAsBlocked|Boolean|Gibt an, ob Benutzer das Menüelement „Speichern unter“ verwenden dürfen, um eine Kopie geschützter Dateien zu speichern. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|periodOfflineBeforeWipeIsEnforced|Dauer|Legt fest, wie lange eine App ohne Internetverbindung sein darf, bevor sämtliche verwalteten Daten gelöscht werden. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinRequired|Boolean|Gibt an, ob eine PIN auf App-Ebene erforderlich ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|maximumPinRetries|Int32|Maximale Anzahl fehlerhafter PIN-Wiederholungsversuche, bevor die verwaltete App blockiert oder gelöscht wird. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|simplePinBlocked|Boolean|Gibt an, ob einfache PINs blockiert werden sollen. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumPinLength|Int32|Erforderliche PIN-Mindestlänge für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Zulässige Zeichensätze für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Von [ManagedAppProtection](../resources/intune-mam-managedappprotection.md)geerbt. Mögliche Werte: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Dauer|Zeitraum, nach dem die für alle Ebenen geltende PIN zurückgesetzt werden muss, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|allowedDataStorageLocations|[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) -Sammlung|Datenspeicherorte, an denen der Benutzer verwaltete Daten speichern darf. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|contactSyncBlocked|Boolean|Gibt an, ob eine Synchronisierung von Kontakten mit dem Gerät des Benutzers erlaubt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|printBlocked|Boolean|Gibt an, ob aus verwalteten Apps gedruckt werden darf.
 Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|fingerprintBlocked|Boolean|Gibt an, ob statt einer PIN der Fingerabdruckleser verwendet werden darf, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|disableAppPinIfDevicePinIsSet|Boolean|Gibt an, ob die Verwendung der App-PIN erforderlich ist, wenn die Geräte-PIN gesetzt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredOsVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningOsVersion|Zeichenfolge|Ist eine ältere Version als die angegebene Version installiert, wird in der verwalteten App die Warnmeldung angezeigt, dass kein Zugriff auf Unternehmensdaten erlaubt ist. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumRequiredAppVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|minimumWarningAppVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version wird eine Warnmeldung in der verwalteten App angezeigt. Geerbt von [managedAppProtection](../resources/intune-mam-managedappprotection.md).|
|isAssigned|Boolescher Wert|Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde. Geerbt von [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md).|
|screenCaptureBlocked|Boolean|Gibt an, ob verwaltete Benutzer Screenshots von verwalteten Apps anfertigen dürfen.|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|Ist diese Einstellung aktiviert, ist die Verschlüsselung auf App-Ebene deaktiviert, wenn die Verschlüsselung auf Geräteebene aktiviert ist.|
|encryptAppData|Boolean|Gibt an, ob die Anwendungsdaten verwalteter Apps verschlüsselt werden sollen.|
|deployedAppCount|Int32|Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde|
|minimumRequiredPatchVersion|Zeichenfolge|Legt das älteste erforderliche Android-Sicherheitspatchlevel fest, mit dem einem Benutzer noch sicherer Zugriff auf die App gewährt wird.|
|minimumWarningPatchVersion|String|Legt das älteste empfohlene Android-Sicherheitspatchlevel fest, mit dem einem Benutzer noch sicherer Zugriff auf die App gewährt wird.|

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
  "@odata.type": "microsoft.graph.androidManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
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
  "isAssigned": true,
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 1024,
  "minimumRequiredPatchVersion": "String",
  "minimumWarningPatchVersion": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-androidmanagedappprotection.md/microsoft.graph.androidManagedAppProtection/allowedDataStorageLocations:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->


