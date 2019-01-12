---
title: Abrufen von macOSVpnConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des MacOSVpnConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b0e01f3adccf44732779febf66cfe9456cd3c7a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913415"
---
# <a name="get-macosvpnconfiguration"></a><span data-ttu-id="34baf-103">Abrufen von macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="34baf-103">Get macOSVpnConfiguration</span></span>

> <span data-ttu-id="34baf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34baf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34baf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34baf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34baf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="34baf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34baf-107">Lesen Sie Eigenschaften und Beziehungen des [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="34baf-107">Read properties and relationships of the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="34baf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="34baf-108">Prerequisites</span></span>
<span data-ttu-id="34baf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34baf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34baf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34baf-111">Permission type</span></span>|<span data-ttu-id="34baf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34baf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34baf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34baf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34baf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34baf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="34baf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34baf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34baf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34baf-116">Not supported.</span></span>|
|<span data-ttu-id="34baf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34baf-117">Application</span></span>|<span data-ttu-id="34baf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34baf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34baf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34baf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34baf-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="34baf-120">Optional query parameters</span></span>
<span data-ttu-id="34baf-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="34baf-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="34baf-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="34baf-122">Request headers</span></span>
|<span data-ttu-id="34baf-123">Header</span><span class="sxs-lookup"><span data-stu-id="34baf-123">Header</span></span>|<span data-ttu-id="34baf-124">Wert</span><span class="sxs-lookup"><span data-stu-id="34baf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34baf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="34baf-125">Authorization</span></span>|<span data-ttu-id="34baf-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="34baf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34baf-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="34baf-127">Accept</span></span>|<span data-ttu-id="34baf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="34baf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34baf-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="34baf-129">Request body</span></span>
<span data-ttu-id="34baf-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="34baf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34baf-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="34baf-131">Response</span></span>
<span data-ttu-id="34baf-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="34baf-132">If successful, this method returns a `200 OK` response code and [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34baf-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34baf-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="34baf-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34baf-134">Request</span></span>
<span data-ttu-id="34baf-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="34baf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="34baf-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="34baf-136">Response</span></span>
<span data-ttu-id="34baf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34baf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2184

{
  "value": {
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
}
```





