# <a name="deviceconfigurationstate-resource-type"></a>deviceConfigurationState-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Gerätekonfigurationsstatus für ein bestimmtes Gerät.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceConfigurationStates auflisten](../api/intune_deviceconfig_deviceconfigurationstate_list.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)-Objekte.|
|[deviceConfigurationState abrufen](../api/intune_deviceconfig_deviceconfigurationstate_get.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|Lesen von Eigenschaften und Beziehungen des [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)-Objekts.|
|[deviceConfigurationState erstellen](../api/intune_deviceconfig_deviceconfigurationstate_create.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|Erstellen eines neuen [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)-Objekts.|
|[deviceConfigurationState löschen](../api/intune_deviceconfig_deviceconfigurationstate_delete.md)|Keine|Löscht ein [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)-Objekt.|
|[deviceConfigurationState aktualisieren](../api/intune_deviceconfig_deviceconfigurationstate_update.md)|[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)|Aktualisieren der Eigenschaften eines [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität.|
|settingStates|[deviceConfigurationSettingState](../resources/intune_deviceconfig_deviceconfigurationsettingstate.md)-Sammlung|Noch nicht dokumentiert|
|displayName|String|Der Name der Richtlinie für diese policyBase|
|version|Int32|Die Version der Richtlinie|
|platformType|String|Plattformtyp, für den die Richtlinie gilt. Mögliche Werte: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.|
|state|String|Der Compliance-Status der Richtlinie. Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.|
|settingCount|Int32|Anzahl der Einstellungen, die eine Richtlinie enthält|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
      "setting": "String",
      "settingName": "String",
      "instanceDisplayName": "String",
      "state": "String",
      "errorCode": 1024,
      "errorDescription": "String",
      "userId": "String",
      "userName": "String",
      "userEmail": "String",
      "userPrincipalName": "String",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "String",
          "displayName": "String"
        }
      ],
      "currentValue": "String"
    }
  ],
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024
}
```



