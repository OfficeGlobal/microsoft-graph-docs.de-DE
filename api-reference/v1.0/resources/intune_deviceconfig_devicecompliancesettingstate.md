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
|id|Zeichenfolge|Schlüssel der Entität|
|Einstellung|Zeichenfolge|Klassenname und Eigenschaftenname der Einstellung|
|settingName|Zeichenfolge|Gemeldeter Einstellungsname|
|deviceId|Zeichenfolge|Gemeldete Geräte-ID|
|deviceName|Zeichenfolge|Gemeldeter Gerätename|
|userId|Zeichenfolge|Gemeldete Benutzer-ID|
|userEmail|Zeichenfolge|Gemeldete Benutzer-E-Mail-Adresse|
|userName|Zeichenfolge|Gemeldeter Benutzername|
|userPrincipalName|Zeichenfolge|Gemeldeter Benutzerprinzipalname|
|deviceModel|Zeichenfolge|Gemeldetes Gerätemodell|
|Zustand|[complianceStatus](../resources/intune_shared_compliancestatus.md)|Der Compliance-Zustand der Einstellung. Die möglichen Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}-->
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



