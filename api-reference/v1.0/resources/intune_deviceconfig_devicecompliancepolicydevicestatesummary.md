# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a>deviceCompliancePolicyDeviceStateSummary-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceCompliancePolicyDeviceStateSummary abrufen](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_get.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|Lesen von Beziehungen und Eigenschaften des [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)-Objekts.|
|[deviceCompliancePolicyDeviceStateSummary aktualisieren](../api/intune_deviceconfig_devicecompliancepolicydevicestatesummary_update.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|Aktualisieren der Eigenschaften eines [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|inGracePeriodCount|Int32|Anzahl von Geräten, die sich in der Toleranzperiode befinden|
|configManagerCount|Int32|Anzahl von Geräten, deren Konformität mit System Center Configuration Manager verwaltet wird|
|id|Zeichenfolge|Schlüssel der Entität|
|unknownDeviceCount|Int32|Anzahl von unbekannten Geräten|
|notApplicableDeviceCount|Int32|Anzahl der ausgenommenen Geräte|
|compliantDeviceCount|Int32|Anzahl von konformen Geräten|
|remediatedDeviceCount|Int32|Anzahl von korrigierten Geräten|
|nonCompliantDeviceCount|Int32|Anzahl von nicht konformen Geräten|
|errorDeviceCount|Int32|Anzahl von Geräten mit Fehlern|
|conflictDeviceCount|Int32|Anzahl der Geräte mit Konflikten|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



