---
title: Abrufen von iosVpnConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des IosVpnConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 46f8f47054186c2208e29f95f78ce6926ab62fe9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302324"
---
# <a name="get-iosvpnconfiguration"></a><span data-ttu-id="4d810-103">Abrufen von iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="4d810-103">Get iosVpnConfiguration</span></span>

> <span data-ttu-id="4d810-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4d810-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d810-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4d810-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d810-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4d810-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d810-107">Lesen Sie Eigenschaften und Beziehungen des [IosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4d810-107">Read properties and relationships of the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d810-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4d810-108">Prerequisites</span></span>
<span data-ttu-id="4d810-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d810-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d810-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d810-111">Permission type</span></span>|<span data-ttu-id="4d810-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d810-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d810-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d810-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d810-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d810-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4d810-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d810-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d810-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d810-116">Not supported.</span></span>|
|<span data-ttu-id="4d810-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d810-117">Application</span></span>|<span data-ttu-id="4d810-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d810-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d810-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d810-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d810-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4d810-120">Optional query parameters</span></span>
<span data-ttu-id="4d810-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4d810-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4d810-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d810-122">Request headers</span></span>
|<span data-ttu-id="4d810-123">Header</span><span class="sxs-lookup"><span data-stu-id="4d810-123">Header</span></span>|<span data-ttu-id="4d810-124">Wert</span><span class="sxs-lookup"><span data-stu-id="4d810-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d810-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4d810-125">Authorization</span></span>|<span data-ttu-id="4d810-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d810-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d810-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4d810-127">Accept</span></span>|<span data-ttu-id="4d810-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4d810-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d810-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d810-129">Request body</span></span>
<span data-ttu-id="4d810-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4d810-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d810-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d810-131">Response</span></span>
<span data-ttu-id="4d810-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [IosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4d810-132">If successful, this method returns a `200 OK` response code and [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d810-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d810-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d810-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d810-134">Request</span></span>
<span data-ttu-id="4d810-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d810-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="4d810-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d810-136">Response</span></span>
<span data-ttu-id="4d810-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d810-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





