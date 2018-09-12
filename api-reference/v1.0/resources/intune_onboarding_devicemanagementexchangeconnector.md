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
|ID|Zeichenfolge|Noch nicht dokumentiert|
|lastSyncDateTime|DateTimeOffset|Zeit der letzten Synchronisierung für Exchange Connector|
|Status|[deviceManagementExchangeConnectorStatus](../resources/intune_onboarding_devicemanagementexchangeconnectorstatus.md)|Status des Exchange Connectors. Mögliche Werte: sind `none`, `connectionPending`, `connected` und `disconnected`.|
|primarySmtpAddress|Zeichenfolge|E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.|
|serverName|Zeichenfolge|Der Name des Exchange Servers.|
|connectorServerName|Zeichenfolge|Der Name des Servers, der Exchange Connector hostet.|
|exchangeConnectorType|[deviceManagementExchangeConnectorType](../resources/intune_onboarding_devicemanagementexchangeconnectortype.md)|Der konfigurierte Typ von Exchange Connector. Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|Version|Zeichenfolge|Die Version des ExchangeConnectorAgent|
|exchangeAlias|Zeichenfolge|Ein dem Exchange-Server zugewiesener Alias|
|exchangeOrganization|Zeichenfolge|Exchange-Organisation für den Exchange-Server|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeConnector"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "status": "String",
  "primarySmtpAddress": "String",
  "serverName": "String",
  "connectorServerName": "String",
  "exchangeConnectorType": "String",
  "version": "String",
  "exchangeAlias": "String",
  "exchangeOrganization": "String"
}
```








