# <a name="defaultmanagedappprotection-resource-type"></a>Ressourcentyp „defaultManagedAppProtection“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Richtlinie wird verwendet, um detaillierte Verwaltungseinstellungen für eine festgelegte Gruppe von Apps zu konfigurieren, die für alle Benutzer greifen, die nicht unter eine Richtlinie des Typs „targetedManagedAppProtection“ fallen.

Sie erbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „defaultManagedAppProtection“](../api/intune_mam_defaultmanagedappprotection_list.md)|Sammlung von Objekten des Typs [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md) auf.|
|[Abrufen von „defaultManagedAppProtection“](../api/intune_mam_defaultmanagedappprotection_get.md)|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md).|
|[Erstellen von „defaultManagedAppProtection“](../api/intune_mam_defaultmanagedappprotection_create.md)|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md)|Erstellt neue Objekte des Typs [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md).|
|[Löschen von „defaultManagedAppProtection“](../api/intune_mam_defaultmanagedappprotection_delete.md)|Keiner|Löscht Objekte des Typs [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md).|
|[Aktualisieren von „defaultManagedAppProtection“](../api/intune_mam_defaultmanagedappprotection_update.md)|[defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md)|Aktualisiert die Eigenschaften von Objekten des Typs [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Anzeigename der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|description|Zeichenfolge|Beschreibung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|Version|Zeichenfolge|Version der Entität Geerbt von [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|periodOfflineBeforeAccessCheck|Dauer|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät nicht mit dem Internet verbunden ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|periodOnlineBeforeAccessCheck|Dauer|Zeitraum, nach dem der Zugriff überprüft wird, wenn das Gerät mit dem Internet verbunden ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|allowedInboundDataTransferSources|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|Quellen, von denen Daten übermittelt werden dürfen. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md). Mögliche Werte sind: `allApps`, `managedApps`,`none`.|
|allowedOutboundDataTransferDestinations|[managedAppDataTransferLevel](../resources/intune_mam_managedappdatatransferlevel.md)|Ziele, an die Daten übermittelt werden dürfen. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md). Mögliche Werte sind: `allApps`, `managedApps`,`none`.|
|organizationalCredentialsRequired|Boolesch|Gibt an, ob von der Organisation bereitgestellte Anmeldeinformationen zur Nutzung der App erforderlich sind. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|allowedOutboundClipboardSharingLevel|[managedAppClipboardSharingLevel](../resources/intune_mam_managedappclipboardsharinglevel.md)|Regelt die Freigabe der Zwischenablage für Anwendungen auf dem verwalteten Gerät. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md). Mögliche Werte sind: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.|
|dataBackupBlocked|Boolesch|Gibt an, ob die Sicherung der Daten der verwalteten App blockiert werden soll. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|deviceComplianceRequired|Boolesch|Gibt an, ob Gerätekonformität erforderlich ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|managedBrowserToOpenLinksRequired|Boolesch|Gibt an, ob Internetlinks in der Managed Browser-App geöffnet werden sollen. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|saveAsBlocked|Boolesch|Gibt an, ob Benutzer das Menüelement „Speichern unter“ verwenden dürfen, um eine Kopie geschützter Dateien zu speichern. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|periodOfflineBeforeWipeIsEnforced|Dauer|Legt fest, wie lange eine App ohne Internetverbindung sein darf, bevor sämtliche verwalteten Daten gelöscht werden. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|pinRequired|Boolesch|Gibt an, ob eine PIN auf App-Ebene erforderlich ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|maximumPinRetries|Int32|Legt die Maximalanzahl von fehlerhaften PIN-Eingaben fest, bevor die verwaltete Anwendung entweder blockiert oder zurückgesetzt wird. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|simplePinBlocked|Boolesch|Gibt an, ob einfache PINs blockiert werden sollen. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumPinLength|Int32|Erforderliche PIN-Mindestlänge für PINs auf App-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|pinCharacterSet|[managedAppPinCharacterSet](../resources/intune_mam_managedapppincharacterset.md)|Zulässige Zeichensätze für PINs auf Anwendungs-Ebene, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md). Mögliche Werte sind: `numeric`, `alphanumericAndSymbol`.|
|periodBeforePinReset|Dauer|Zeitraum, nach dem die für alle Ebenen geltende PIN zurückgesetzt werden muss, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|allowedDataStorageLocations|[ManagedAppDataStorageLocation Enumerations](../resources/intune_mam_managedappdatastoragelocation.md)-Sammlung|Datenspeicherorte, an denen der Benutzer verwaltete Daten speichern darf. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|contactSyncBlocked|Boolesch|Gibt an, ob eine Synchronisierung von Kontakten mit dem Gerät des Benutzers erlaubt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|printBlocked|Boolesch|Gibt an, ob aus verwalteten Apps gedruckt werden darf. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|fingerprintBlocked|Boolesch|Gibt an, ob statt einer PIN der Fingerabdruckleser verwendet werden darf, wenn „pinRequired“ auf „true“ gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|disableAppPinIfDevicePinIsSet|Boolesch|Gibt an, ob die Verwendung der App-PIN erforderlich ist, wenn die Geräte-PIN gesetzt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumRequiredOsVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumWarningOsVersion|Zeichenfolge|Ist eine ältere Version als die angegebene Version installiert, wird in der verwalteten App die Warnmeldung angezeigt, dass kein Zugriff auf Unternehmensdaten erlaubt ist. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumRequiredAppVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|minimumWarningAppVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version wird eine Warnmeldung in der verwalteten App angezeigt. Geerbt von [managedAppProtection](../resources/intune_mam_managedappprotection.md).|
|appDataEncryptionType|[managedAppDataEncryptionType](../resources/intune_mam_managedappdataencryptiontype.md)|Typ der Verschlüsselung, die auf Daten in einer verwalteten Anwendung angewendet werden soll. (nur iOS). Mögliche Werte sind: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.|
|screenCaptureBlocked|Boolesch|Gibt an, ob Screenshots blockiert werden sollen.|
|encryptAppData|Boolesch|Gibt an, ob die Daten verwalteter Apps verschlüsselt werden sollen. (nur Android)|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolesch|Ist diese Einstellung aktiviert, ist die Verschlüsselung auf App-Ebene deaktiviert, wenn die Verschlüsselung auf Geräteebene aktiviert ist.|
|minimumRequiredSdkVersion|Zeichenfolge|Unter älteren Versionen als der angegebenen Version ist der Zugriff auf Unternehmensdaten für die verwaltete App blockiert.|
|customSettings|Collection von Objekten des Typs [keyValuePair](../resources/intune_mam_keyvaluepair.md)|Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an die von der Richtlinie betroffenen Benutzer gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst.|
|deployedAppCount|Int32|Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde|
|minimumRequiredPatchVersion|Zeichenfolge|Legt das älteste erforderliche Android-Sicherheitspatchlevel fest, mit dem einem Benutzer noch sicherer Zugriff auf die App gewährt wird.|
|minimumWarningPatchVersion|Zeichenfolge|Legt das älteste empfohlene Android-Sicherheitspatchlevel fest, mit dem einem Benutzer noch sicherer Zugriff auf die App gewährt wird.|
|faceIdBlocked|Boolesch|Gibt an, ob statt einer PIN die Face ID verwendet werden darf, wenn „pinRequired“ auf „true“ gesetzt ist.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|Apps|Sammlung von Objekten des Typs [managedMobileApp](../resources/intune_mam_managedmobileapp.md)|Liste der Apps, für die die Richtlinie bereitgestellt wurde|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md)|Navigationseigenschaft zu einer Bereitstellungsübersicht für die Konfiguration|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedAppProtection",
  "@odata.type": "microsoft.graph.defaultManagedAppProtection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
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
  "faceIdBlocked": true
}
```



