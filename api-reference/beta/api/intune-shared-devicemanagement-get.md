---
title: deviceManagement abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceManagement-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c00b60793209904ce184de25f12f1f4ad14fad1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862636"
---
# <a name="get-devicemanagement"></a>deviceManagement abrufen

> **Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune-shared-devicemanagement.md)-Objekts.

## <a name="prerequisites"></a>Voraussetzungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigung&nbsp;Typ&nbsp;(durch&nbsp;Workflow) | Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten) |
|:---|:---|
| Delegiert (Geschäfts-, Schul- oder Unikonto) | |
| &nbsp;&nbsp; **Für die Arbeit android** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **Überwachung** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
| &nbsp;&nbsp; **Unternehmen Begriffe** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Gerätekonfiguration** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **Geräteverwaltung** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **Elektronische SIM** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **Registrierung** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Zauns** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Benachrichtigung** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Onboarding** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **RBAC** | DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All |
| &nbsp;&nbsp; **Remotezugriff** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **Remoteunterstützung** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Telekommunikation Ausgaben Management** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **Problembehandlung** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **Windows Information Protection** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt|
| Anwendung | Nicht unterstützt |



## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceManagement](../resources/intune-shared-devicemanagement.md) im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a>Antwort

Hier einige Beispiele der Antwort. 

Hinweis: Die hier gezeigte Antwortobjekte der Kürze halber werden möglicherweise abgeschnitten.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

Eigenschaften für den Workflow entsprechenden werden zurückgegeben.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```



