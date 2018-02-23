# <a name="devicecompliancepolicystate-resource-type"></a>deviceCompliancePolicyState-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zustand der Gerätekompatibilitätsrichtlinien für ein bestimmtes Gerät.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceCompliancePolicyStates auflisten](../api/intune_deviceconfig_devicecompliancepolicystate_list.md)|[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)-Objekte.|
|[deviceCompliancePolicyState abrufen](../api/intune_deviceconfig_devicecompliancepolicystate_get.md)|[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)|Lesen von Eigenschaften und Beziehungen des [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)-Objekts.|
|[deviceCompliancePolicyState erstellen](../api/intune_deviceconfig_devicecompliancepolicystate_create.md)|[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)|Erstellen eines neuen [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)-Objekts.|
|[deviceCompliancePolicyState löschen](../api/intune_deviceconfig_devicecompliancepolicystate_delete.md)|Keine|Löschen eines [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).|
|[deviceCompliancePolicyState aktualisieren](../api/intune_deviceconfig_devicecompliancepolicystate_update.md)|[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)|Aktualisieren der Eigenschaften eines [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|settingStates|[deviceCompliancePolicySettingState](../resources/intune_deviceconfig_devicecompliancepolicysettingstate.md)-Sammlung|Noch nicht dokumentiert.|
|displayName|Zeichenfolge|Name der Richtlinie für diese policyBase|
|Version|Int32|Version der Richtlinie|
|platformType|Zeichenfolge|Der Plattformtyp, für den die Richtlinie gilt. Mögliche Werte: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.|
|state|Zeichenfolge|Der Compliance-Status der Richtlinie. Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.|
|settingCount|Int32|Anzahl der Einstellungen, die eine Richtlinie enthält|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
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



