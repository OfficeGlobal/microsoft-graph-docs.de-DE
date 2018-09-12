# <a name="devicecomplianceuserstatus-resource-type"></a>deviceComplianceUserStatus-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceComplianceUserStatuses auflisten](../api/intune_deviceconfig_devicecomplianceuserstatus_list.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)-Objekte.|
|[deviceComplianceUserStatus abrufen](../api/intune_deviceconfig_devicecomplianceuserstatus_get.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Lesen von Eigenschaften und Beziehungen des [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)-Objekts.|
|[DeviceComplianceUserStatus erstellen](../api/intune_deviceconfig_devicecomplianceuserstatus_create.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Erstellen eines neuen [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)-Objekts.|
|[DeviceComplianceUserStatus löschen](../api/intune_deviceconfig_devicecomplianceuserstatus_delete.md)|Keine|Löscht ein [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)-Objekt.|
|[DeviceComplianceUserStatus aktualisieren](../api/intune_deviceconfig_devicecomplianceuserstatus_update.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Aktualisieren der Eigenschaften eines [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Schlüssel der Entität|
|userDisplayName|Zeichenfolge|Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört|
|devicesCount|Int32|Geräteanzahl für den Benutzer|
|Status|[complianceStatus](../resources/intune_shared_compliancestatus.md)|Compliance-Status des Richtlinienberichts. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` , `notAssigned`.|
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
  "@odata.type": "microsoft.graph.deviceComplianceUserStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```








