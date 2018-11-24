# <a name="devicecompliancesettingstate-resource-type"></a>deviceComplianceSettingState-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zustand der Gerätekompatibilitätseinstellung für ein bestimmtes Gerät.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceComplianceSettingStates auflisten](../api/intune_deviceconfig_devicecompliancesettingstate_list.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)-Sammlung|Auflisten der Eigenschaften und Beziehungen der [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)-Objekte.|
|[deviceComplianceSettingState abrufen](../api/intune_deviceconfig_devicecompliancesettingstate_get.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|Lesen von Eigenschaften und Beziehungen des [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)-Objekts.|
|[deviceComplianceSettingState erstellen](../api/intune_deviceconfig_devicecompliancesettingstate_create.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|Erstellen eines neuen [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)-Objekts.|
|[deviceComplianceSettingState löschen](../api/intune_deviceconfig_devicecompliancesettingstate_delete.md)|Keine|Löscht ein [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)-Objekt.|
|[deviceComplianceSettingState aktualisieren](../api/intune_deviceconfig_devicecompliancesettingstate_update.md)|[deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)|Aktualisieren der Eigenschaften eines [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|setting|String|Der Klassenname und der Eigenschaftenname der Einstellung.|
|settingName|String|Der gemeldete Einstellungsname|
|deviceId|String|Die gemeldete Geräte-ID|
|deviceName|String|Der gemeldete Gerätename|
|userId|String|Die gemeldete Benutzer-ID|
|userEmail|String|Die gemeldete Benutzer-E-Mail-Adresse|
|userName|String|Der gemeldete Benutzername|
|userPrincipalName|String|Der gemeldete Benutzerprinzipalname|
|deviceModel|String|Das gemeldete Gerätemodell|
|state|[complianceStatus](../resources/intune_shared_compliancestatus.md)|Der Compliance-Zustand der Einstellung. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```



