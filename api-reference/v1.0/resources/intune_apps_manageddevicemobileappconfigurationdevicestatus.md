# <a name="manageddevicemobileappconfigurationdevicestatus-resource-type"></a>Ressourcentyp managedDeviceMobileAppConfigurationDeviceStatus

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für den Status einer MDM-Konfiguration mobiler Anwendungen für einen Benutzer.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflistung von managedDeviceMobileAppConfigurationDeviceStatuses](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_list.md)|[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)-Auflistung|Auflistung von Eigenschaften und Beziehungen der [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) -Objekte.|
|[Abrufen von managedDeviceMobileAppConfigurationDeviceStatus](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_get.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)|Lesen von Eigenschaften und Beziehungen des Objekts [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md).|
|[Erstellen von managedDeviceMobileAppConfigurationDeviceStatus](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_create.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)|Erstellen eines neuen [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) -Objekts.|
|[Löschen von ManagedDeviceMobileAppConfigurationDeviceStatus](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_delete.md)|Keine|Löscht [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md).|
|[ManagedDeviceMobileAppConfigurationDeviceStatus aktualisieren](../api/intune_apps_manageddevicemobileappconfigurationdevicestatus_update.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md)|Aktualisieren der Eigenschaften eines [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune_apps_manageddevicemobileappconfigurationdevicestatus.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|deviceDisplayName|Zeichenfolge|Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist|
|userName|Zeichenfolge|Gemeldeter Benutzername|
|deviceModel|Zeichenfolge|Gemeldetes Gerätemodell|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität|
|Status|[complianceStatus](../resources/intune_shared_compliancestatus.md)|Compliance-Status des Richtlinienberichts. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Richtlinienberichts|
|userPrincipalName|Zeichenfolge|Benutzer-Prinzipalname|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```








