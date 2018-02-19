# <a name="devicemanagement-resource-type"></a>deviceManagement-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceManagement abrufen](../api/intune_devices_devicemanagement_get.md)|[deviceManagement](../resources/intune_devices_devicemanagement.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_devices_devicemanagement.md)-Objekts.|
|[deviceManagement aktualisieren](../api/intune_devices_devicemanagement_update.md)|[deviceManagement](../resources/intune_devices_devicemanagement.md)|Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_devices_devicemanagement.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für das Gerät|
|subscriptionState|String|Abonnementstatus für Verwaltung mobiler Geräte des Mandanten. Mögliche Werte: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|Apple Push Notification-Zertifikat.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md)|Geräteübersicht|
|detectedApps|[detectedApp](../resources/intune_devices_detectedapp.md)-Sammlung|Die Liste der erkannten Apps, die einem Gerät zugeordnet sind.|
|managedDevices|[managedDevice](../resources/intune_devices_manageddevice.md)-Sammlung|Die Liste der verwalteten Geräte|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```



