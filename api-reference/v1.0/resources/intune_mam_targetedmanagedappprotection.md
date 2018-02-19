# <a name="targetedmanagedappprotection-resource-type"></a>Ressourcentyp „targetedManagedAppProtection“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Richtlinie wird verwendet, um detaillierte Verwaltungseinstellungen für bestimmte Sicherheitsgruppen zu konfigurieren.

Sie erbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „targetedManagedAppProtection“](../api/intune_mam_targetedmanagedappprotection_list.md)|Sammlung von Objekten des Typs [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md) auf.|
|[Abrufen von „targetedManagedAppProtection“](../api/intune_mam_targetedmanagedappprotection_get.md)|[targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md).|
|[Aktion „assign“](../api/intune_mam_targetedmanagedappprotection_assign.md)|Keiner|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Anzeigename der Richtlinie. Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|description|String|Beschreibung der Richtlinie. Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der Richtlinie. Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Richtlinie. Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|id|String|Schlüssel der Entität. Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|version|String|Version der Entität. Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Duration|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät nicht mit dem Internet verbunden ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|periodOnlineBeforeAccessCheck|Duration|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät mit dem Internet verbunden ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|allowedInboundDataTransferSources|String|Quellen, von denen Daten übermittelt werden dürfen. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md). Mögliche Werte sind: `allApps`, `managedApps` und `none`.|
|allowedOutboundDataTransferDestinations|String|Ziele, an die Daten übermittelt werden dürfen. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md). Mögliche Werte sind: `allApps`, `managedApps` und `none`.|
|organizationalCredentialsRequired|Boolean|Gibt an, ob von der Organisation bereitgestellte Anmeldeinformationen zur Nutzung der App erforderlich sind. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|allowedOutboundClipboardSharingLevel|String|Regelt die Freigabe der Zwischenablage für Apps auf dem verwalteten Gerät. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md). Mögliche Werte sind: `allApps`, `managedAppsWithPasteIn`, `managedApps` und `blocked`.|
|dataBackupBlocked|Boolean|Gibt an, ob die Sicherung der Daten der verwalteten App blockiert werden soll. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|deviceComplianceRequired|Boolean|Gibt an, ob Gerätekonformität erforderlich ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|managedBrowserToOpenLinksRequired|Boolean|Gibt an, ob Internetlinks in der Managed Browser-App geöffnet werden sollen. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|saveAsBlocked|Boolean|Gibt an, ob Benutzer das Menüelement „Speichern unter“ verwenden dürfen, um eine Kopie geschützter Dateien zu speichern. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|periodOfflineBeforeWipeIsEnforced|Duration|Legt fest, wie lange eine App ohne Internetverbindung sein darf, bevor sämtliche verwalteten Daten gelöscht werden. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|pinRequired|Boolean|Gibt an, ob eine PIN auf App-Ebene erforderlich ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|maximumPinRetries|Int32|Legt die Maximalanzahl von fehlerhaften PIN-Eingaben fest, nach der die verwaltete App zurückgesetzt wird. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|simplePinBlocked|Boolean|Gibt an, ob einfache PINs blockiert werden sollen. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumPinLength|Int32|Erforderliche PIN-Mindestlänge für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|pinCharacterSet|String|Zulässige Zeichensätze für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md). Mögliche Werte sind: `numeric` und `alphanumericAndSymbol`.|
|periodBeforePinReset|Duration|Zeitraum, nach dem die für alle Ebenen geltende PIN zurückgesetzt werden muss, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|allowedDataStorageLocations|String-Sammlung|Datenspeicherorte, an denen der Benutzer verwaltete Daten speichern darf. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|contactSyncBlocked|Boolean|Gibt an, ob eine Synchronisierung von Kontakten mit dem Gerät des Benutzers erlaubt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|printBlocked|Boolean|Gibt an, ob über verwaltete Apps gedruckt werden darf. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|fingerprintBlocked|Boolean|Gibt an, ob statt einer PIN der Fingerabdruckleser verwendet werden darf, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|disableAppPinIfDevicePinIsSet|Boolean|Gibt an, ob die Verwendung der App-PIN erforderlich ist, wenn die Geräte-PIN gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumRequiredOsVersion|String|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumWarningOsVersion|String|Ist eine ältere Version als die angegebene Version installiert, wird in der verwalteten App die Warnmeldung angezeigt, dass kein Zugriff auf Unternehmensdaten erlaubt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumRequiredAppVersion|String|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumWarningAppVersion|String|Unter älteren Versionen als der angegebenen Version wird eine Warnmeldung in der verwalteten App angezeigt. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|isAssigned|Boolean|Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|Sammlung von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Navigationseigenschaft zu einer Liste von Einschlussgruppen und Ausschlussgruppen, für die die Richtlinie bereitgestellt wurde.|

## <a name="json-representation"></a>JSON-Darstellung
Unten sehen Sie eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
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
  "isAssigned": true
}
```



