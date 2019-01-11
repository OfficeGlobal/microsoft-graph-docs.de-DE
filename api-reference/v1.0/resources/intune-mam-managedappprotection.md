---
title: managedAppProtection-Ressourcentyp
description: Diese Richtlinie wird verwendet, um detaillierte Verwaltungseinstellungen für eine bestimmte Gruppe von Apps zu konfigurieren.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cb5c6f6a158a79bdc9bd19094b79ef7510db1f3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861817"
---
# <a name="managedappprotection-resource-type"></a>managedAppProtection-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Richtlinie wird verwendet, um detaillierte Verwaltungseinstellungen für eine bestimmte Gruppe von Apps zu konfigurieren.

Erbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedAppProtections auflisten](../api/intune-mam-managedappprotection-list.md)|[managedAppProtection](../resources/intune-mam-managedappprotection.md)-Sammlung|Listet die Eigenschaften und Beziehungen von [managedAppProtection](../resources/intune-mam-managedappprotection.md)-Objekten auf.|
|[managedAppProtection abrufen](../api/intune-mam-managedappprotection-get.md)|[managedAppProtection](../resources/intune-mam-managedappprotection.md)|Liest die Eigenschaften und Beziehungen des [managedAppProtection](../resources/intune-mam-managedappprotection.md)-Objekts.|
|[targetApps-Aktion](../api/intune-mam-managedappprotection-targetapps.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Anzeigename der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|String|Beschreibung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|String|Schlüssel der Entität Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|Version|String|Version der Entität Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Duration|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät nicht mit dem Internet verbunden ist.|
|periodOnlineBeforeAccessCheck|Duration|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät mit dem Internet verbunden ist.|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Quellen, von denen Daten übermittelt werden dürfen. Mögliche Werte: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune-mam-managedappdatatransferlevel.md)|Ziele, an die Daten übermittelt werden dürfen. Mögliche Werte: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolean|Gibt an, ob von der Organisation bereitgestellte Anmeldeinformationen zur Nutzung der App erforderlich sind.|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune-mam-managedappclipboardsharinglevel.md)|Regelt die Freigabe der Zwischenablage für Apps auf dem verwalteten Gerät. Mögliche Werte: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolean|Gibt an, ob die Sicherung der Daten der verwalteten App blockiert werden soll.|
|deviceComplianceRequired|Boolean|Gibt an, ob Gerätekonformität erforderlich ist.|
|managedBrowserToOpenLinksRequired|Boolean|Gibt an, ob Internetlinks in der Managed Browser-App geöffnet werden sollen.|
|saveAsBlocked|Boolean|Gibt an, ob Benutzer das Menüelement „Speichern unter“ verwenden dürfen, um eine Kopie geschützter Dateien zu speichern.|
|periodOfflineBeforeWipeIsEnforced|Duration|Legt fest, wie lange eine App ohne Internetverbindung sein darf, bevor sämtliche verwalteten Daten gelöscht werden.|
|pinRequired|Boolean|Gibt an, ob eine PIN auf App-Ebene erforderlich ist.|
|maximumPinRetries|Int32|Maximale Anzahl von falsche Pin "Wiederholen" versucht, bevor die verwaltete app blockiert oder Kennworteingaben gelöscht wird.|
|simplePinBlocked|Boolean|Gibt an, ob einfache PINs blockiert werden sollen.|
|minimumPinLength|Int32|Erforderliche PIN-Mindestlänge für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist.|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune-mam-managedapppincharacterset.md)|Zulässige Zeichensätze für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Mögliche Werte: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duration|Zeitraum, nach dem die für alle Ebenen geltende PIN zurückgesetzt werden muss, wenn „pinRequired“ auf „true“ gesetzt ist.|
|allowedDataStorageLocations|[ManagedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) -Auflistung|Datenspeicherorte, an denen der Benutzer verwaltete Daten speichern darf.|
|contactSyncBlocked|Boolean|Gibt an, ob eine Synchronisierung von Kontakten mit dem Gerät des Benutzers erlaubt ist.|
|printBlocked|Boolean|Gibt an, ob über verwaltete Apps gedruckt werden darf.|
|fingerprintBlocked|Boolean|Gibt an, ob statt einer PIN der Fingerabdruckleser verwendet werden darf, wenn „pinRequired“ auf „true“ gesetzt ist.|
|disableAppPinIfDevicePinIsSet|Boolean|Gibt an, ob die Verwendung der App-PIN erforderlich ist, wenn die Geräte-PIN gesetzt ist.|
|minimumRequiredOsVersion|String|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert.|
|minimumWarningOsVersion|String|Ist eine ältere Version als die angegebene Version installiert, wird in der verwalteten App die Warnmeldung angezeigt, dass kein Zugriff auf Unternehmensdaten erlaubt ist.|
|minimumRequiredAppVersion|String|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert.|
|minimumWarningAppVersion|String|Unter älteren Versionen als der angegebenen Version wird eine Warnmeldung in der verwalteten App angezeigt.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtection",
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
  "minimumWarningAppVersion": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-managedappprotection.md/microsoft.graph.managedAppProtection/allowedDataStorageLocations:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->


