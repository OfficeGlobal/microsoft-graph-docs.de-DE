---
title: Liste macOSVpnConfigurations
description: Listeneigenschaften und Beziehungen der MacOSVpnConfiguration-Objekte.
ms.openlocfilehash: 28cdd315800e78b0f0684bf417b900c6366af3b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061948"
---
# <a name="list-macosvpnconfigurations"></a><span data-ttu-id="5d65a-103">Liste macOSVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="5d65a-103">List macOSVpnConfigurations</span></span>

> <span data-ttu-id="5d65a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5d65a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d65a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5d65a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d65a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5d65a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d65a-107">Listeneigenschaften und Beziehungen der [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="5d65a-107">List properties and relationships of the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5d65a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5d65a-108">Prerequisites</span></span>
<span data-ttu-id="5d65a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d65a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d65a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d65a-111">Permission type</span></span>|<span data-ttu-id="5d65a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d65a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d65a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d65a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d65a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d65a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5d65a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d65a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d65a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d65a-116">Not supported.</span></span>|
|<span data-ttu-id="5d65a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d65a-117">Application</span></span>|<span data-ttu-id="5d65a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d65a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d65a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d65a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5d65a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d65a-120">Request headers</span></span>
|<span data-ttu-id="5d65a-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5d65a-121">Header</span></span>|<span data-ttu-id="5d65a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5d65a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d65a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d65a-123">Authorization</span></span>|<span data-ttu-id="5d65a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5d65a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d65a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5d65a-125">Accept</span></span>|<span data-ttu-id="5d65a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d65a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d65a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d65a-127">Request body</span></span>
<span data-ttu-id="5d65a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5d65a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d65a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d65a-129">Response</span></span>
<span data-ttu-id="5d65a-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5d65a-130">If successful, this method returns a `200 OK` response code and a collection of [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d65a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d65a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5d65a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d65a-132">Request</span></span>
<span data-ttu-id="5d65a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d65a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="5d65a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d65a-134">Response</span></span>
<span data-ttu-id="5d65a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d65a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2334

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
      "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
      "optInToDeviceIdSharing": true
    }
  ]
}
```





