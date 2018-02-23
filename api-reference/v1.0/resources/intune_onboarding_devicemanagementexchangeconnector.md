# <a name="devicemanagementexchangeconnector-resource-type"></a>deviceManagementExchangeConnector-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Entität, die eine Verbindung mit einer Exchange-Umgebung darstellt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceManagementExchangeConnectors auflisten](../api/intune_onboarding_devicemanagementexchangeconnector_list.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)-Objekte.|
|[DeviceManagementExchangeConnector abrufen](../api/intune_onboarding_devicemanagementexchangeconnector_get.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)-Objekts.|
|[DeviceManagementExchangeConnector erstellen](../api/intune_onboarding_devicemanagementexchangeconnector_create.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)|Erstellen eines neuen [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)-Objekts.|
|[DeviceManagementExchangeConnector löschen](../api/intune_onboarding_devicemanagementexchangeconnector_delete.md)|Keine|Löscht ein [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)-Objekt.|
|[DeviceManagementExchangeConnector aktualisieren](../api/intune_onboarding_devicemanagementexchangeconnector_update.md)|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)|Aktualisieren der Eigenschaften eines [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md)-Objekts.|
|[sync-Aktion](../api/intune_onboarding_devicemanagementexchangeconnector_sync.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Noch nicht dokumentiert|
|lastSyncDateTime|DateTimeOffset|Zeit der letzten Synchronisierung für Exchange Connector|
|status|String|Status von Exchange Connector. Mögliche Werte: `none`, `connectionPending`, `connected`, `disconnected`.|
|primarySmtpAddress|String|E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.|
|serverName|String|Der Name des Servers, der Exchange Connector hostet.|
|exchangeConnectorType|String|Der konfigurierte Typ von Exchange Connector. Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|version|String|Die Version des ExchangeConnectorAgent|
|exchangeAlias|String|Ein dem Exchange-Server zugewiesener Alias|
|exchangeOrganization|String|Exchange-Organisation für den Exchange-Server|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "status": "String",
  "primarySmtpAddress": "String",
  "serverName": "String",
  "exchangeConnectorType": "String",
  "version": "String",
  "exchangeAlias": "String",
  "exchangeOrganization": "String"
}
```



