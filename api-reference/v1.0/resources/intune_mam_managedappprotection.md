# <a name="managedappprotection-resource-type"></a>managedAppProtection-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Richtlinie wird verwendet, um detaillierte Verwaltungseinstellungen für eine bestimmte Gruppe von Apps zu konfigurieren.

Erbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedAppProtections auflisten](../api/intune_mam_managedappprotection_list.md)|[managedAppProtection](../resources/intune_mam_managedappprotection.md)-Sammlung|Listet die Eigenschaften und Beziehungen von [managedAppProtection](../resources/intune_mam_managedappprotection.md)-Objekten auf.|
|[managedAppProtection abrufen](../api/intune_mam_managedappprotection_get.md)|[managedAppProtection](../resources/intune_mam_managedappprotection.md)|Liest die Eigenschaften und Beziehungen des [managedAppProtection](../resources/intune_mam_managedappprotection.md)-Objekts.|
|[targetApps-Aktion](../api/intune_mam_managedappprotection_targetapps.md)|Keine|Noch nicht dokumentiert.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Anzeigename der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|Beschreibung|Zeichenfolge|Beschreibung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|Version|Zeichenfolge|Version der Entität Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Dauer|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät nicht mit dem Internet verbunden ist.|
|periodOnlineBeforeAccessCheck|Dauer|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät mit dem Internet verbunden ist.|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|Quellen, von denen Daten übermittelt werden dürfen. Mögliche Werte: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|Ziele, an die Daten übermittelt werden dürfen. Mögliche Werte: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolescher Wert|Gibt an, ob von der Organisation bereitgestellte Anmeldeinformationen zur Nutzung der App erforderlich sind.|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune_mam_managedappclipboardsharinglevel.md)|Regelt die Freigabe der Zwischenablage für Apps auf dem verwalteten Gerät. Mögliche Werte: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolescher Wert|Gibt an, ob die Sicherung der Daten der verwalteten App blockiert werden soll.|
|deviceComplianceRequired|Boolescher Wert|Gibt an, ob Gerätekonformität erforderlich ist.|
|managedBrowserToOpenLinksRequired|Boolescher Wert|Gibt an, ob Internetlinks in der Managed Browser-App geöffnet werden sollen.|
|saveAsBlocked|Boolescher Wert|Gibt an, ob Benutzer das Menüelement „Speichern unter“ verwenden dürfen, um eine Kopie geschützter Dateien zu speichern.|
|periodOfflineBeforeWipeIsEnforced|Dauer|Legt fest, wie lange eine App ohne Internetverbindung sein darf, bevor sämtliche verwalteten Daten gelöscht werden.|
|pinRequired|Boolescher Wert|Gibt an, ob eine PIN auf App-Ebene erforderlich ist.|
|maximumPinRetries|Int32|Maximale Anzahl von falsche Pin "Wiederholen" versucht, bevor die verwaltete app blockiert oder Kennworteingaben gelöscht wird.|
|simplePinBlocked|Boolescher Wert|Gibt an, ob einfache PINs blockiert werden sollen.|
|minimumPinLength|Int32|Erforderliche PIN-Mindestlänge für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist.|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune_mam_managedapppincharacterset.md)|Zulässige Zeichensätze für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Mögliche Werte: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Dauer|Zeitraum, nach dem die für alle Ebenen geltende PIN zurückgesetzt werden muss, wenn „pinRequired“ auf „true“ gesetzt ist.|
|allowedDataStorageLocations|[ManagedAppDataStorageLocation](../resources/intune_mam_managedappdatastoragelocation.md) -Auflistung|Datenspeicherorte, an denen der Benutzer verwaltete Daten speichern darf.|
|contactSyncBlocked|Boolescher Wert|Gibt an, ob eine Synchronisierung von Kontakten mit dem Gerät des Benutzers erlaubt ist.|
|printBlocked|Boolescher Wert|Gibt an, ob über verwaltete Apps gedruckt werden darf.|
|fingerprintBlocked|Boolescher Wert|Gibt an, ob statt einer PIN der Fingerabdruckleser verwendet werden darf, wenn „pinRequired“ auf „true“ gesetzt ist.|
|disableAppPinIfDevicePinIsSet|Boolescher Wert|Gibt an, ob die Verwendung der App-PIN erforderlich ist, wenn die Geräte-PIN gesetzt ist.|
|minimumRequiredOsVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert.|
|minimumWarningOsVersion|Zeichenfolge|Ist eine ältere Version als die angegebene Version installiert, wird in der verwalteten App die Warnmeldung angezeigt, dass kein Zugriff auf Unternehmensdaten erlaubt ist.|
|minimumRequiredAppVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert.|
|minimumWarningAppVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version wird eine Warnmeldung in der verwalteten App angezeigt.|

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
     "Warning: /api-reference/v1.0/resources/intune_mam_managedappprotection.md/microsoft.graph.managedAppProtection/allowedDataStorageLocations:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->


