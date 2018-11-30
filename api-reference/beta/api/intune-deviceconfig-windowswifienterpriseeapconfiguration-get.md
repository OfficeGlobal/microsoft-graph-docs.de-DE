---
title: Abrufen von windowsWifiEnterpriseEAPConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des WindowsWifiEnterpriseEAPConfiguration-Objekts.
ms.openlocfilehash: 8d4b718bdae430e21386a3fa035fe153340acfa6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062133"
---
# <a name="get-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="41d55-103">Abrufen von windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="41d55-103">Get windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="41d55-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="41d55-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41d55-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="41d55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41d55-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="41d55-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41d55-107">Lesen Sie Eigenschaften und Beziehungen des [WindowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="41d55-107">Read properties and relationships of the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41d55-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="41d55-108">Prerequisites</span></span>
<span data-ttu-id="41d55-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41d55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41d55-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="41d55-111">Permission type</span></span>|<span data-ttu-id="41d55-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="41d55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41d55-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="41d55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41d55-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d55-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="41d55-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="41d55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41d55-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41d55-116">Not supported.</span></span>|
|<span data-ttu-id="41d55-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="41d55-117">Application</span></span>|<span data-ttu-id="41d55-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41d55-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41d55-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="41d55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41d55-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="41d55-120">Optional query parameters</span></span>
<span data-ttu-id="41d55-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="41d55-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="41d55-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="41d55-122">Request headers</span></span>
|<span data-ttu-id="41d55-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="41d55-123">Header</span></span>|<span data-ttu-id="41d55-124">Wert</span><span class="sxs-lookup"><span data-stu-id="41d55-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41d55-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="41d55-125">Authorization</span></span>|<span data-ttu-id="41d55-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="41d55-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41d55-127">Accept</span><span class="sxs-lookup"><span data-stu-id="41d55-127">Accept</span></span>|<span data-ttu-id="41d55-128">application/json</span><span class="sxs-lookup"><span data-stu-id="41d55-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41d55-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="41d55-129">Request body</span></span>
<span data-ttu-id="41d55-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="41d55-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41d55-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="41d55-131">Response</span></span>
<span data-ttu-id="41d55-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [WindowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="41d55-132">If successful, this method returns a `200 OK` response code and [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41d55-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="41d55-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="41d55-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="41d55-134">Request</span></span>
<span data-ttu-id="41d55-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="41d55-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="41d55-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="41d55-136">Response</span></span>
<span data-ttu-id="41d55-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="41d55-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1773

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
    "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "preSharedKey": "Pre Shared Key value",
    "wifiSecurityType": "wpaPersonal",
    "meteredConnectionLimit": "fixed",
    "ssid": "Ssid value",
    "networkName": "Network Name value",
    "connectAutomatically": true,
    "connectToPreferredNetwork": true,
    "connectWhenNetworkNameIsHidden": true,
    "proxySetting": "manual",
    "proxyManualAddress": "Proxy Manual Address value",
    "proxyManualPort": 15,
    "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
    "forceFIPSCompliance": true,
    "networkSingleSignOn": "prelogon",
    "maximumAuthenticationTimeoutInSeconds": 5,
    "promptForAdditionalAuthenticationCredentials": true,
    "enablePairwiseMasterKeyCaching": true,
    "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
    "maximumNumberOfPairwiseMasterKeysInCache": 8,
    "enablePreAuthentication": true,
    "maximumPreAuthenticationAttempts": 0,
    "eapType": "leap",
    "trustedServerCertificateNames": [
      "Trusted Server Certificate Names value"
    ],
    "authenticationMethod": "usernameAndPassword",
    "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
    "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
  }
}
```





