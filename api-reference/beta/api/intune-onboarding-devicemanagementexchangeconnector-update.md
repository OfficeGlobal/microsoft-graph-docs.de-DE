---
title: deviceManagementExchangeConnector aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementExchangeConnector-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 877493e0ef2234942abf2b1b90d4493b73afb615
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946112"
---
# <a name="update-devicemanagementexchangeconnector"></a>deviceManagementExchangeConnector aktualisieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Aktualisieren der Eigenschaften eines [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)-Objekts.
## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a>Anforderungsheader
|Header|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Noch nicht dokumentiert|
|lastSyncDateTime|DateTimeOffset|Zeit der letzten Synchronisierung für Exchange Connector|
|status|[deviceManagementExchangeConnectorStatus](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|Exchange Connectorstatus. Mögliche Werte: sind `none`, `connectionPending`, `connected` und `disconnected`.|
|primarySmtpAddress|String|E-Mail-Adresse, die zum Konfigurieren von Exchange Connector zwischen Diensten verwendet wird.|
|serverName|String|Der Name des Exchange-Servers.|
|connectorServerName|String|Der Name des Servers, der Exchange Connector hostet.|
|exchangeConnectorType|[deviceManagementExchangeConnectorType](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|Der konfigurierte Typ von Exchange Connector. Mögliche Werte: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|Version|String|Die Version des ExchangeConnectorAgent|
|exchangeAlias|String|Ein dem Exchange-Server zugewiesener Alias|
|exchangeOrganization|String|Exchange-Organisation für den Exchange-Server|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) im Antworttext zurück.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
Content-type: application/json
Content-length: 418

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```





