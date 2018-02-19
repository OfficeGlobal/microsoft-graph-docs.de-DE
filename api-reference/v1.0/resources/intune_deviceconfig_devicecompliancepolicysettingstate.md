# <a name="devicecompliancepolicysettingstate-resource-type"></a>deviceCompliancePolicySettingState-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|setting|String|Die gemeldete Einstellung|
|settingName|String|Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird|
|instanceDisplayName|String|Name der Einstellungsinstanz, die gemeldet wird.|
|state|String|Der Konformitätsstatus der Einstellung. Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.|
|errorCode|Int64|Fehlercode für die Einstellung|
|errorDescription|String|Fehlerbeschreibung|
|userId|String|UserId|
|userName|String|UserName|
|userEmail|String|UserEmail|
|userPrincipalName|String|UserPrincipalName.|
|sources|[settingSource](../resources/intune_deviceconfig_settingsource.md)-Sammlung|Beitragende Richtlinien|
|currentValue|String|Aktueller Wert der Einstellung auf dem Gerät|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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
```



