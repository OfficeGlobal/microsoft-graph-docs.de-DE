# <a name="manageddevicemobileappconfiguration-resource-type"></a>managedDeviceMobileAppConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedDeviceMobileAppConfigurations auflisten](../api/intune_apps_manageddevicemobileappconfiguration_list.md)|[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)-Objekte.|
|[managedDeviceMobileAppConfiguration abrufen](../api/intune_apps_manageddevicemobileappconfiguration_get.md)|[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität.|
|targetedMobileApps|String-Sammlung|Die zugeordnete App.|
|createdDateTime|DateTimeOffset|DateTime der Erstellung des Objekts.|
|description|String|Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration.|
|lastModifiedDateTime|DateTimeOffset|DateTime der letzten Änderung des Objekts.|
|displayName|String|Vom Administrator bereitgestellter Name der Gerätekonfiguration.|
|version|Int32|Version der Gerätekonfiguration.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)-Sammlung|Die Liste der Gruppenzuweisungen für die App-Konfiguration.|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md)-Sammlung|Liste von ManagedDeviceMobileAppConfigurationUserStatus.|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md)|Zusammenfassung der App-Konfiguration-Gerätestatus.|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md)|Zusammenfassung der App-Konfiguration-Benutzerstatus.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



