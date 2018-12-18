---
title: Abrufen von windows10VpnConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des windows10VpnConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 140de467a4f10d097d84c59e0dae3bb1fb18721a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352941"
---
# <a name="get-windows10vpnconfiguration"></a><span data-ttu-id="ff069-103">Abrufen von windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff069-103">Get windows10VpnConfiguration</span></span>

> <span data-ttu-id="ff069-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ff069-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff069-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff069-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff069-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff069-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff069-107">Lesen Sie Eigenschaften und Beziehungen des [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ff069-107">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff069-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ff069-108">Prerequisites</span></span>
<span data-ttu-id="ff069-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff069-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff069-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff069-111">Permission type</span></span>|<span data-ttu-id="ff069-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff069-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff069-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff069-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff069-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff069-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ff069-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff069-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff069-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff069-116">Not supported.</span></span>|
|<span data-ttu-id="ff069-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff069-117">Application</span></span>|<span data-ttu-id="ff069-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff069-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff069-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff069-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff069-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ff069-120">Optional query parameters</span></span>
<span data-ttu-id="ff069-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ff069-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ff069-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff069-122">Request headers</span></span>
|<span data-ttu-id="ff069-123">Header</span><span class="sxs-lookup"><span data-stu-id="ff069-123">Header</span></span>|<span data-ttu-id="ff069-124">Wert</span><span class="sxs-lookup"><span data-stu-id="ff069-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff069-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ff069-125">Authorization</span></span>|<span data-ttu-id="ff069-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ff069-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff069-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ff069-127">Accept</span></span>|<span data-ttu-id="ff069-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ff069-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff069-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff069-129">Request body</span></span>
<span data-ttu-id="ff069-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ff069-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff069-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff069-131">Response</span></span>
<span data-ttu-id="ff069-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ff069-132">If successful, this method returns a `200 OK` response code and [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff069-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff069-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff069-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff069-134">Request</span></span>
<span data-ttu-id="ff069-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff069-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ff069-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff069-136">Response</span></span>
<span data-ttu-id="ff069-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff069-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3676

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
    "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
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
    "servers": [
      {
        "@odata.type": "microsoft.graph.vpnServer",
        "description": "Description value",
        "address": "Address value",
        "isDefaultServer": true
      }
    ],
    "customXml": "Y3VzdG9tWG1s",
    "profileTarget": "device",
    "connectionType": "f5EdgeClient",
    "enableSplitTunneling": true,
    "enableAlwaysOn": true,
    "enableDeviceTunnel": true,
    "enableDnsRegistration": true,
    "dnsSuffixes": [
      "Dns Suffixes value"
    ],
    "authenticationMethod": "usernameAndPassword",
    "rememberUserCredentials": true,
    "enableConditionalAccess": true,
    "enableSingleSignOnWithAlternateCertificate": true,
    "singleSignOnEku": {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    },
    "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
    "eapXml": "ZWFwWG1s",
    "proxyServer": {
      "@odata.type": "microsoft.graph.windows10VpnProxyServer",
      "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
      "address": "Address value",
      "port": 4,
      "bypassProxyServerForLocalAddress": true
    },
    "associatedApps": [
      {
        "@odata.type": "microsoft.graph.windows10AssociatedApps",
        "appType": "universal",
        "identifier": "Identifier value"
      }
    ],
    "onlyAssociatedAppsCanUseConnection": true,
    "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
    "trafficRules": [
      {
        "@odata.type": "microsoft.graph.vpnTrafficRule",
        "name": "Name value",
        "protocols": 9,
        "localPortRanges": [
          {
            "@odata.type": "microsoft.graph.numberRange",
            "lowerNumber": 11,
            "upperNumber": 11
          }
        ],
        "remotePortRanges": [
          {
            "@odata.type": "microsoft.graph.numberRange",
            "lowerNumber": 11,
            "upperNumber": 11
          }
        ],
        "localAddressRanges": [
          {
            "@odata.type": "microsoft.graph.iPv4Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
          }
        ],
        "remoteAddressRanges": [
          {
            "@odata.type": "microsoft.graph.iPv4Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
          }
        ],
        "appId": "App Id value",
        "appType": "desktop",
        "routingPolicyType": "splitTunnel",
        "claims": "Claims value"
      }
    ],
    "routes": [
      {
        "@odata.type": "microsoft.graph.vpnRoute",
        "destinationPrefix": "Destination Prefix value",
        "prefixSize": 10
      }
    ],
    "dnsRules": [
      {
        "@odata.type": "microsoft.graph.vpnDnsRule",
        "name": "Name value",
        "servers": [
          "Servers value"
        ],
        "proxyServerUri": "Proxy Server Uri value"
      }
    ]
  }
}
```





