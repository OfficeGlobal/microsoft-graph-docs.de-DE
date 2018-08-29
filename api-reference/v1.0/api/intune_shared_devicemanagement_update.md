# <a name="update-devicemanagement"></a>Aktualisieren von „deviceManagement“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_shared_devicemanagement.md)-Objekts.
## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

| Berechtigung &nbsp; Typ &nbsp; (vom Workflow &nbsp;) | Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten) |
|:---|:---|
| Delegiert (Geschäfts- oder Schulkonto) |
| &nbsp; &nbsp; Überwachung | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; Unternehmensbedingungen | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; Unternehmens-Registrierung | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp; &nbsp; Geräte-Konfiguration | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; Geräteverwaltung | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp; &nbsp; Endpunkt-Schutz | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp; &nbsp; Registrierung | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; Benachrichtigung | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; Onboarding | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; RBAC | DeviceManagementRBAC.ReadWrite.All |
| &nbsp; &nbsp; Remote-Unterstützung | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; Telecom-Ausgaben-Verwaltung | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; Problembehandlung | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp; &nbsp; Windows Information Schutz | DeviceManagementApps.ReadWrite.All |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt|
| Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Autorisierung|Bearer&lt;token&gt; erforderlich|
|Akzeptieren|Anwendung/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagement](../resources/intune_shared_devicemanagement.md) an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagement](../resources/intune_shared_devicemanagement.md) erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Eindeutiger Bezeichner für das Gerät|
|**Geräte-Konfiguration**|
|Einstellungen|[deviceManagementSettings](../resources/intune_deviceconfig_devicemanagementsettings.md)|Einstellungen auf Kontoebene.|
|**Geräteverwaltung**|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune_devices_devicemanagementsubscriptionstate.md)|Zustand des Abonnements bei der Verwaltung des mobilen Gerätes des Mandanten. Mögliche Werte: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|
|**Onboarding**|
|intuneBrand|[intuneBrand](../resources/intune_onboarding_intunebrand.md)|„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst werden.|

Die Anforderung des Body-Eigenschaft-Supports variiert je nach Workflow.

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagement](../resources/intune_shared_devicemanagement.md) im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```

### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen gekürzt. Zurückgegebene Eigenschaften variieren je nach Workflow und Kontext.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```



