---
title: Liste windows10VpnConfigurations
description: Listeneigenschaften und Beziehungen der windows10VpnConfiguration-Objekte.
author: tfitzmac
ms.openlocfilehash: efc1abfff951cf7ce8d6b69072511a380b1be450
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354887"
---
# <a name="list-windows10vpnconfigurations"></a><span data-ttu-id="0d752-103">Liste windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="0d752-103">List windows10VpnConfigurations</span></span>

> <span data-ttu-id="0d752-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0d752-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d752-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d752-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d752-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0d752-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d752-107">Listeneigenschaften und Beziehungen der [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="0d752-107">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0d752-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0d752-108">Prerequisites</span></span>
<span data-ttu-id="0d752-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d752-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d752-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d752-111">Permission type</span></span>|<span data-ttu-id="0d752-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d752-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d752-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d752-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d752-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d752-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0d752-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d752-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d752-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d752-116">Not supported.</span></span>|
|<span data-ttu-id="0d752-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d752-117">Application</span></span>|<span data-ttu-id="0d752-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d752-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d752-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d752-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0d752-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d752-120">Request headers</span></span>
|<span data-ttu-id="0d752-121">Header</span><span class="sxs-lookup"><span data-stu-id="0d752-121">Header</span></span>|<span data-ttu-id="0d752-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0d752-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d752-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0d752-123">Authorization</span></span>|<span data-ttu-id="0d752-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0d752-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d752-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0d752-125">Accept</span></span>|<span data-ttu-id="0d752-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d752-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d752-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d752-127">Request body</span></span>
<span data-ttu-id="0d752-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0d752-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d752-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d752-129">Response</span></span>
<span data-ttu-id="0d752-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0d752-130">If successful, this method returns a `200 OK` response code and a collection of [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d752-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d752-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d752-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d752-132">Request</span></span>
<span data-ttu-id="0d752-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d752-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0d752-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d752-134">Response</span></span>
<span data-ttu-id="0d752-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d752-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3916

{
  "value": [
    {
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
  ]
}
```





