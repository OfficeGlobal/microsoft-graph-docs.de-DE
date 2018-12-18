---
title: deviceManagementExchangeConnector-Ressourcentyp
description: Entität, die eine Verbindung mit einer Exchange-Umgebung darstellt.
author: tfitzmac
ms.openlocfilehash: 726afd7957f8e95d38b68065b1bc99f884a9208d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312026"
---
# <a name="devicemanagementexchangeconnector-resource-type"></a>deviceManagementExchangeConnector-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Entität, die eine Verbindung mit einer Exchange-Umgebung darstellt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceManagementExchangeConnectors auflisten](../api/intune-onboarding-devicemanagementexchangeconnector-list.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekte.|
|[DeviceManagementExchangeConnector abrufen](../api/intune-onboarding-devicemanagementexchangeconnector-get.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.|
|[DeviceManagementExchangeConnector erstellen](../api/intune-onboarding-devicemanagementexchangeconnector-create.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Erstellen eines neuen [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.|
|[DeviceManagementExchangeConnector löschen](../api/intune-onboarding-devicemanagementexchangeconnector-delete.md)|Keine|Löscht ein [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekt.|
|[DeviceManagementExchangeConnector aktualisieren](../api/intune-onboarding-devicemanagementexchangeconnector-update.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Aktualisieren der Eigenschaften eines [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.|
|[sync-Aktion](../api/intune-onboarding-devicemanagementexchangeconnector-sync.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Noch nicht dokumentiert|
|lastSyncDateTime|DateTimeOffset|Zeit der letzten Synchronisierung für Exchange Connector|
|status|[deviceManagementExchangeConnectorStatus](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|Exchange Connectorstatus. Mögliche Werte: sind `none`, `connectionPending`, `connected` und `disconnected`.|
|primarySmtpAddress|String|E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.|
|serverName|String|Der Name des Exchange-Servers.|
|connectorServerName|String|Der Name des Servers, der Exchange Connector hostet.|
|exchangeConnectorType|[deviceManagementExchangeConnectorType](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|Der konfigurierte Typ von Exchange Connector. Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|Version|String|Die Version des ExchangeConnectorAgent|
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
  "connectorServerName": "String",
  "exchangeConnectorType": "String",
  "version": "String",
  "exchangeAlias": "String",
  "exchangeOrganization": "String"
}
```





