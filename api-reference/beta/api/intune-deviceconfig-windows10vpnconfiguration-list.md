---
title: Windows10VpnConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der windows10VpnConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4672352e448faef7b6495de37e37a590ae3ede42
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145815"
---
# <a name="list-windows10vpnconfigurations"></a><span data-ttu-id="d0f93-103">Windows10VpnConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="d0f93-103">List windows10VpnConfigurations</span></span>

> <span data-ttu-id="d0f93-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d0f93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0f93-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d0f93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0f93-106">AufListen von Eigenschaften und Beziehungen der [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="d0f93-106">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0f93-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d0f93-107">Prerequisites</span></span>
<span data-ttu-id="d0f93-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d0f93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d0f93-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d0f93-110">Permission type</span></span>|<span data-ttu-id="d0f93-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d0f93-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0f93-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d0f93-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0f93-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0f93-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d0f93-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d0f93-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0f93-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d0f93-115">Not supported.</span></span>|
|<span data-ttu-id="d0f93-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d0f93-116">Application</span></span>|<span data-ttu-id="d0f93-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d0f93-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0f93-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0f93-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d0f93-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d0f93-119">Request headers</span></span>
|<span data-ttu-id="d0f93-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d0f93-120">Header</span></span>|<span data-ttu-id="d0f93-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d0f93-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0f93-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0f93-122">Authorization</span></span>|<span data-ttu-id="d0f93-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d0f93-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0f93-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d0f93-124">Accept</span></span>|<span data-ttu-id="d0f93-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0f93-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0f93-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d0f93-126">Request body</span></span>
<span data-ttu-id="d0f93-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d0f93-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0f93-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0f93-128">Response</span></span>
<span data-ttu-id="d0f93-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d0f93-129">If successful, this method returns a `200 OK` response code and a collection of [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0f93-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d0f93-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0f93-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0f93-131">Request</span></span>
<span data-ttu-id="d0f93-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d0f93-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d0f93-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0f93-133">Response</span></span>
<span data-ttu-id="d0f93-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d0f93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4064

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
          "proxyServerUri": "Proxy Server Uri value",
          "autoTrigger": true,
          "persistent": true
        }
      ],
      "trustedNetworkDomains": [
        "Trusted Network Domains value"
      ]
    }
  ]
}
```




