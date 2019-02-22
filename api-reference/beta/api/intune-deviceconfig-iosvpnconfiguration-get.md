---
title: IosVpnConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des iosVpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 190bbc9ce72db899d0059039486cb0539695d82c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174361"
---
# <a name="get-iosvpnconfiguration"></a>IosVpnConfiguration abrufen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Lesen von Eigenschaften und Beziehungen des [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2383

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVpnConfiguration",
    "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "connectionName": "Connection Name value",
    "connectionType": "pulseSecure",
    "loginGroupOrDomain": "Login Group Or Domain value",
    "role": "Role value",
    "realm": "Realm value",
    "server": {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    },
    "identifier": "Identifier value",
    "customData": [
      {
        "@odata.type": "microsoft.graph.keyValue",
        "key": "Key value",
        "value": "Value value"
      }
    ],
    "customKeyValueData": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "enableSplitTunneling": true,
    "authenticationMethod": "usernameAndPassword",
    "enablePerApp": true,
    "safariDomains": [
      "Safari Domains value"
    ],
    "onDemandRules": [
      {
        "@odata.type": "microsoft.graph.vpnOnDemandRule",
        "ssids": [
          "Ssids value"
        ],
        "dnsSearchDomains": [
          "Dns Search Domains value"
        ],
        "probeUrl": "https://example.com/probeUrl/",
        "action": "evaluateConnection",
        "domainAction": "neverConnect",
        "domains": [
          "Domains value"
        ],
        "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
      }
    ],
    "proxyServer": {
      "@odata.type": "microsoft.graph.vpnProxyServer",
      "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
      "address": "Address value",
      "port": 4
    },
    "optInToDeviceIdSharing": true,
    "providerType": "appProxy",
    "userDomain": "User Domain value",
    "strictEnforcement": true,
    "cloudName": "Cloud Name value",
    "excludeList": [
      "Exclude List value"
    ]
  }
}
```




