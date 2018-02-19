# <a name="devicemanagement-resource-type"></a>deviceManagement-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Singleton-Entität, die als Container für Android for Work-Einstellungsfunktionen unter der Geräteverwaltung dient.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceManagement abrufen](../api/intune_androidforwork_devicemanagement_get.md)|[deviceManagement](../resources/intune_androidforwork_devicemanagement.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_androidforwork_devicemanagement.md)-Objekts.|
|[deviceManagement aktualisieren](../api/intune_androidforwork_devicemanagement_update.md)|[deviceManagement](../resources/intune_androidforwork_devicemanagement.md)|Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_androidforwork_devicemanagement.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Noch nicht dokumentiert.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|Die Singleton-Entität mit Android for Work-Einstellungen.|
|androidForWorkAppConfigurationSchemas|[androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md)-Sammlung|Android for Work-App – Konfigurationsschemaentitäten|
|androidForWorkEnrollmentProfiles|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)-Sammlung|Android for Work-Registrierungsprofilentitäten.|

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
  "id": "String (identifier)"
}
```



