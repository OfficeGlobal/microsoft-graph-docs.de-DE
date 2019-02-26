---
title: deviceManagementExchangeConnector-Ressourcentyp
description: Entität, die eine Verbindung mit einer Exchange-Umgebung darstellt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 172a8ae7bbdbad77da9b7a67d57047441e5a039d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262608"
---
# <a name="devicemanagementexchangeconnector-resource-type"></a>deviceManagementExchangeConnector-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Entität, die eine Verbindung mit einer Exchange-Umgebung darstellt.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceManagementExchangeConnectors auflisten](../api/intune-onboarding-devicemanagementexchangeconnector-list.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekte.|
|[DeviceManagementExchangeConnector abrufen](../api/intune-onboarding-devicemanagementexchangeconnector-get.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.|
|[DeviceManagementExchangeConnector erstellen](../api/intune-onboarding-devicemanagementexchangeconnector-create.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Erstellen eines neuen [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.|
|[DeviceManagementExchangeConnector löschen](../api/intune-onboarding-devicemanagementexchangeconnector-delete.md)|Keine|Löscht ein [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekt.|
|[DeviceManagementExchangeConnector aktualisieren](../api/intune-onboarding-devicemanagementexchangeconnector-update.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Aktualisieren der Eigenschaften eines [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.|
|[sync-Aktion](../api/intune-onboarding-devicemanagementexchangeconnector-sync.md)|Keine|Noch nicht dokumentiert.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Noch nicht dokumentiert|
|lastSyncDateTime|DateTimeOffset|Zeit der letzten Synchronisierung für Exchange Connector|
|status|[deviceManagementExchangeConnectorStatus](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|Exchange Connector-Status. Mögliche Werte: `none`, `connectionPending`, `connected`, `disconnected`.|
|primarySmtpAddress|Zeichenfolge|E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.|
|serverName|Zeichenfolge|Der Name des Exchange-Servers.|
|connectorServerName|Zeichenfolge|Der Name des Servers, der Exchange Connector hostet.|
|exchangeConnectorType|[deviceManagementExchangeConnectorType](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|Der konfigurierte Typ von Exchange Connector. Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|Version|Zeichenfolge|Die Version des ExchangeConnectorAgent|
|exchangeAlias|Zeichenfolge|Ein dem Exchange-Server zugewiesener Alias|
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



