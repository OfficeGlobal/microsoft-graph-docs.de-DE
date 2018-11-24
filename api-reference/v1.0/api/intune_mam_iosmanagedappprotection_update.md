# <a name="update-iosmanagedappprotection"></a>Aktualisieren von „iosManagedAppProtection“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md).
## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementApps.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Accept|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) erstellen.

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
|allowedDataStorageLocations|[ManagedAppDataStorageLocation](../resources/intune_mam_managedappdatastoragelocation.md) -Auflistung|Datenspeicherorte, an denen der Benutzer verwaltete Daten speichern darf. Geerbt von [ManagedAppProtection](../resources/intune_mam_managedappprotection.md). Mögliche Werte sind: `oneDriveForBusiness`, `sharePoint` und `localStorage`.|
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



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md) im Antworttext zurück.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
Content-type: application/json
Content-length: 1568

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "isAssigned": true,
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1740

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "isAssigned": true,
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true
}
```



