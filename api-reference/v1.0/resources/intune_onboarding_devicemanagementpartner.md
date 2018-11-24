# <a name="devicemanagementpartner-resource-type"></a>deviceManagementPartner-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Entität, die eine Verbindung mit dem Geräteverwaltungspartner darstellt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceManagementPartners auflisten](../api/intune_onboarding_devicemanagementpartner_list.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Objekte.|
|[deviceManagementPartner abrufen](../api/intune_onboarding_devicemanagementpartner_get.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Objekts.|
|[deviceManagementPartner erstellen](../api/intune_onboarding_devicemanagementpartner_create.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|Erstellen eines neuen [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Objekts.|
|[deviceManagementPartner löschen](../api/intune_onboarding_devicemanagementpartner_delete.md)|Keine|Löscht ein [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Objekt.|
|[deviceManagementPartner aktualisieren](../api/intune_onboarding_devicemanagementpartner_update.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|Aktualisieren der Eigenschaften eines [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Noch nicht dokumentiert|
|lastHeartbeatDateTime|DateTimeOffset|Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to Device management Partner“ durch den Administrator|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune_onboarding_devicemanagementpartnertenantstate.md)|Partner-Status, der diesen Mandanten. Mögliche Werte sind: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected` und `unresponsive`.|
|partnerAppType|[deviceManagementPartnerAppType](../resources/intune_onboarding_devicemanagementpartnerapptype.md)|Partner-App-Typ. Mögliche Werte sind: `unknown`, `singleTenantApp` und `multiTenantApp`.|
|singleTenantAppId|String|ID der Partner-App mit einem einzelnen Mandanten|
|displayName|String|Anzeigename für Partner|
|isConfigured|Boolescher Wert|Gibt an, ob Geräteverwaltungspartner konfiguriert ist.|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|DateTime in UTC, zu der PartnerDevices entfernt werden|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|DateTime in UTC, zu der PartnerDevices als nicht kompatibel gekennzeichnet werden|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "String",
  "displayName": "String",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)"
}
```



