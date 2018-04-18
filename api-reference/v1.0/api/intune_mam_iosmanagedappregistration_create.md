# <a name="create-iosmanagedappregistration"></a>Erstellen von „iosManagedAppRegistration“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Methode erstellt ein neues Objekt des Typs [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md).
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
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Accept|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosManagedAppRegistration“ an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosManagedAppRegistration“ erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|applicationVersion|String|App-Version. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|managementSdkVersion|String|Version des App-Verwaltungs-SDK. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|platformVersion|String|Version des Betriebssystems. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|deviceType|String|Gerätetyp des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|deviceTag|String|Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden. Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|deviceName|String|Gerätename des Hostgeräts. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|flaggedReasons|Collection von Objekten des Typs „String“|Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde. Beispiel: Die App wird auf einem gerooteten Gerät ausgeführt. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md). Mögliche Werte sind: `none` und `rootedDevice`.|
|userId|String|Benutzer-ID, zu der die App-Registrierung gehört. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|appIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|Bezeichner des App-Pakets. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|id|String|Schlüssel der Entität. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|version|String|Version der Entität. Geerbt von [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) im Antworttext zurück.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 635

{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "Bundle Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 743

{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "Bundle Id value"
  },
  "id": "47632c19-2c19-4763-192c-6347192c6347",
  "version": "Version value"
}
```



