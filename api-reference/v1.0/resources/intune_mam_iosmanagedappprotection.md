# <a name="iosmanagedappprotection-resource-type"></a>Ressourcentyp „iosManagedAppProtection“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Richtlinie wird verwendet, um detaillierte Verwaltungseinstellungen für bestimmte Sicherheitsgruppen sowie für festgelegte Gruppen von Apps auf einem iOS-Gerät zu konfigurieren.

Sie erbt von [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „iosManagedAppProtection“](../api/intune_mam_iosmanagedappprotection_list.md)|Sammlung von Objekten des Typs [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) auf.|
|[Abrufen von „iosManagedAppProtection“](../api/intune_mam_iosmanagedappprotection_get.md)|[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).|
|[Erstellen von „iosManagedAppProtection“](../api/intune_mam_iosmanagedappprotection_create.md)|[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md)|Erstellt neue Objekte des Typs [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).|
|[Löschen von „iosManagedAppProtection“](../api/intune_mam_iosmanagedappprotection_delete.md)|Keiner|Löscht Objekte des Typs [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).|
|[Aktualisieren von „iosManagedAppProtection“](../api/intune_mam_iosmanagedappprotection_update.md)|[iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md)|Aktualisiert die Eigenschaften von Objekten des Typs [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Anzeigename der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|description|String|Beschreibung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|id|String|Schlüssel der Entität Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|Version|String|Version der Entität Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Duration|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät nicht mit dem Internet verbunden ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|periodOnlineBeforeAccessCheck|Duration|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät mit dem Internet verbunden ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|Quellen, von denen Daten übermittelt werden dürfen. Geerbt von [ManagedAppProtection](../resources/intune_mam_managedappprotection.md). Mögliche Werte: `allApps`, `managedApps`, `none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|Ziele, an die Daten übermittelt werden dürfen. Geerbt von [ManagedAppProtection](../resources/intune_mam_managedappprotection.md). Mögliche Werte: `allApps`, `managedApps`, `none`.|
|organizationalCredentialsRequired|Boolescher Wert|Gibt an, ob von der Organisation bereitgestellte Anmeldeinformationen zur Nutzung der App erforderlich sind. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune_mam_managedappclipboardsharinglevel.md)|Regelt die Freigabe der Zwischenablage für Apps auf dem verwalteten Gerät. Geerbt von [ManagedAppProtection](../resources/intune_mam_managedappprotection.md). Mögliche Werte: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolescher Wert|Gibt an, ob die Sicherung der Daten der verwalteten App blockiert werden soll. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|deviceComplianceRequired|Boolescher Wert|Gibt an, ob Gerätekonformität erforderlich ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|managedBrowserToOpenLinksRequired|Boolescher Wert|Gibt an, ob Internetlinks in der Managed Browser-App geöffnet werden sollen. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|saveAsBlocked|Boolescher Wert|Gibt an, ob Benutzer das Menüelement „Speichern unter“ verwenden dürfen, um eine Kopie geschützter Dateien zu speichern. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|periodOfflineBeforeWipeIsEnforced|Duration|Legt fest, wie lange eine App ohne Internetverbindung sein darf, bevor sämtliche verwalteten Daten gelöscht werden. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|pinRequired|Boolescher Wert|Gibt an, ob eine PIN auf App-Ebene erforderlich ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|maximumPinRetries|Int32|Maximale Anzahl von falsche Pin "Wiederholen" versucht, bevor die verwaltete app blockiert oder Kennworteingaben gelöscht wird. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|simplePinBlocked|Boolescher Wert|Gibt an, ob einfache PINs blockiert werden sollen. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumPinLength|Int32|Erforderliche PIN-Mindestlänge für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune_mam_managedapppincharacterset.md)|Zulässige Zeichensätze für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [ManagedAppProtection](../resources/intune_mam_managedappprotection.md). Mögliche Werte: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Duration|Zeitraum, nach dem die für alle Ebenen geltende PIN zurückgesetzt werden muss, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|allowedDataStorageLocations|[ManagedAppDataStorageLocation](../resources/intune_mam_managedappdatastoragelocation.md) -Auflistung|Datenspeicherorte, an denen der Benutzer verwaltete Daten speichern darf. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|contactSyncBlocked|Boolescher Wert|Gibt an, ob eine Synchronisierung von Kontakten mit dem Gerät des Benutzers erlaubt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|printBlocked|Boolescher Wert|Gibt an, ob aus verwalteten Apps gedruckt werden darf.
 Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|fingerprintBlocked|Boolescher Wert|Gibt an, ob statt einer PIN der Fingerabdruckleser verwendet werden darf, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|disableAppPinIfDevicePinIsSet|Boolescher Wert|Gibt an, ob die Verwendung der App-PIN erforderlich ist, wenn die Geräte-PIN gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumRequiredOsVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumWarningOsVersion|Zeichenfolge|Ist eine ältere Version als die angegebene Version installiert, wird in der verwalteten App die Warnmeldung angezeigt, dass kein Zugriff auf Unternehmensdaten erlaubt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumRequiredAppVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumWarningAppVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version wird eine Warnmeldung in der verwalteten App angezeigt. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|isAssigned|Boolescher Wert|Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde. Geerbt von [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md).|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune_mam_managedappdataencryptiontype.md)|Typ der Verschlüsselung, die auf Daten in einer verwalteten App angewendet werden soll. Mögliche Werte: sind `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles` und `whenDeviceLocked`.|
|minimumRequiredSdkVersion|String|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert.|
|deployedAppCount|Int32|Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde|
|faceIdBlocked|Boolean|Gibt an, ob statt einer PIN die Face ID verwendet werden darf, wenn „pinRequired“ auf „true“ gesetzt ist.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|Sammlung von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Navigationseigenschaft zu einer Liste von Einschlussgruppen und Ausschlussgruppen, für die die Richtlinie bereitgestellt wurde. Geerbt von [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md).|
|apps|Sammlung von Objekten des Typs [managedMobileApp](../resources/intune_mam_managedmobileapp.md)|Liste der Apps, für die die Richtlinie bereitgestellt wurde|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md)|Navigationseigenschaft zu einer Bereitstellungsübersicht für die Konfiguration|

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
  "isAssigned": true,
  "appDataEncryptionType": "String",
  "minimumRequiredSdkVersion": "String",
  "deployedAppCount": 1024,
  "faceIdBlocked": true
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune_mam_iosmanagedappprotection.md/microsoft.graph.iosManagedAppProtection/allowedDataStorageLocations:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->



