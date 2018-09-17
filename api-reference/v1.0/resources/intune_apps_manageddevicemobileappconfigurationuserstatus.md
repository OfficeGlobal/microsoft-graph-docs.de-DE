# <a name="manageddevicemobileappconfigurationuserstatus-resource-type"></a>managedDeviceMobileAppConfigurationUserStatus-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für den Status einer MDM-Konfiguration mobiler Apps für einen Benutzer.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedDeviceMobileAppConfigurationUserStatuses auflisten](../api/intune_apps_manageddevicemobileappconfigurationuserstatus_list.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)-Objekte.|
|[managedDeviceMobileAppConfigurationUserStatus abrufen](../api/intune_apps_manageddevicemobileappconfigurationuserstatus_get.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)|Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)-Objekts.|
|[managedDeviceMobileAppConfigurationUserStatus erstellen](../api/intune_apps_manageddevicemobileappconfigurationuserstatus_create.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)|Erstellen eines neuen [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)-Objekts.|
|[managedDeviceMobileAppConfigurationUserStatus löschen](../api/intune_apps_manageddevicemobileappconfigurationuserstatus_delete.md)|Keine|Löscht ein [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)-Objekt.|
|[managedDeviceMobileAppConfigurationUserStatus aktualisieren](../api/intune_apps_manageddevicemobileappconfigurationuserstatus_update.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)|Aktualisieren der Eigenschaften eines [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Schlüssel der Entität|
|userDisplayName|Zeichenfolge|Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört|
|devicesCount|Int32|Geräteanzahl für den Benutzer|
|Status|[complianceStatus](../resources/intune_shared_compliancestatus.md)|Konformitätsstatus des Richtlinienberichts. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.|
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
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```








