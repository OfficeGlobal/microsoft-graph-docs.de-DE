# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Singleton-Entität, die als Container für alle Geräte-App-Verwaltungsfunktionen dient.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceAppManagement abrufen](../api/intune_apps_deviceappmanagement_get.md)|[deviceAppManagement](../resources/intune_apps_deviceappmanagement.md)|Lesen von Eigenschaften und Beziehungen des [deviceAppManagement](../resources/intune_apps_deviceappmanagement.md)-Objekts.|
|[deviceAppManagement aktualisieren](../api/intune_apps_deviceappmanagement_update.md)|[deviceAppManagement](../resources/intune_apps_deviceappmanagement.md)|Aktualisieren der Eigenschaften eines [deviceAppManagement](../resources/intune_apps_deviceappmanagement.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|mobileApps|[mobileApp](../resources/intune_apps_mobileapp.md)-Sammlung|Die mobilen Apps.|
|mobileAppCategories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)-Sammlung|Die Kategorien der mobilen Apps.|
|mobileAppConfigurations|[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)-Sammlung|Die Konfigurationen der mobilen Apps für verwaltete Geräte.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



