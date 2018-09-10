# <a name="detectedapp-resource-type"></a>detectedApp-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine verwaltete oder nicht verwaltete App, die auf einem verwalteten Gerät installiert ist. Nicht verwaltete Apps werden nur für als unternehmenseigen gekennzeichnete Geräte angezeigt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[detectedApps auflisten](../api/intune_devices_detectedapp_list.md)|[detectedApp](../resources/intune_devices_detectedapp.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [detectedApp](../resources/intune_devices_detectedapp.md)-Objekte.|
|[detectedApp abrufen](../api/intune_devices_detectedapp_get.md)|[detectedApp](../resources/intune_devices_detectedapp.md)|Auflisten von Eigenschaften und Beziehungen des [detectedApp](../resources/intune_devices_detectedapp.md)-Objekts.|
|[detectedApp erstellen](../api/intune_devices_detectedapp_create.md)|[detectedApp](../resources/intune_devices_detectedapp.md)|Erstellen eines neuen [detectedApp](../resources/intune_devices_detectedapp.md)-Objekts.|
|[detectedApp löschen](../api/intune_devices_detectedapp_delete.md)|Keine|Löscht ein [detectedApp](../resources/intune_devices_detectedapp.md)-Objekt.|
|[detectedApp aktualisieren](../api/intune_devices_detectedapp_update.md)|[detectedApp](../resources/intune_devices_detectedapp.md)|Aktualisieren der Eigenschaften eines [detectedApp](../resources/intune_devices_detectedapp.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|String|Eindeutiger Bezeichner für die erkannte Anwendung. Dieser wird automatisch von Intune generiert, wenn die Anwendung erstellt wird. Schreibgeschützt.|
|displayName|String|Name der ermittelten Anwendung. Schreibgeschützt.|
|version|String|Version der ermittelten Anwendung. Schreibgeschützt.|
|sizeInByte|Int64|Größe der ermittelten Anwendung in Byte. Schreibgeschützt.|
|deviceCount|Int32|Die Anzahl von Geräten, auf denen diese Anwendung installiert ist.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managedDevices|[managedDevice](../resources/intune_devices_manageddevice.md)-Sammlung|Die Geräte, auf denen die ermittelte Anwendung installiert ist.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```








