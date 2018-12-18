---
title: Liste windowsWifiEnterpriseEAPConfigurations
description: Listeneigenschaften und Beziehungen der WindowsWifiEnterpriseEAPConfiguration-Objekte.
author: tfitzmac
ms.openlocfilehash: 9f9755f9cdb58c9fe46dc38d398359542765dd94
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304347"
---
# <a name="list-windowswifienterpriseeapconfigurations"></a><span data-ttu-id="3d165-103">Liste windowsWifiEnterpriseEAPConfigurations</span><span class="sxs-lookup"><span data-stu-id="3d165-103">List windowsWifiEnterpriseEAPConfigurations</span></span>

> <span data-ttu-id="3d165-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3d165-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d165-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3d165-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d165-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3d165-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d165-107">Listeneigenschaften und Beziehungen der [WindowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="3d165-107">List properties and relationships of the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d165-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3d165-108">Prerequisites</span></span>
<span data-ttu-id="3d165-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d165-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d165-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3d165-111">Permission type</span></span>|<span data-ttu-id="3d165-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3d165-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d165-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3d165-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d165-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d165-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3d165-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3d165-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d165-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d165-116">Not supported.</span></span>|
|<span data-ttu-id="3d165-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3d165-117">Application</span></span>|<span data-ttu-id="3d165-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d165-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d165-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d165-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3d165-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3d165-120">Request headers</span></span>
|<span data-ttu-id="3d165-121">Header</span><span class="sxs-lookup"><span data-stu-id="3d165-121">Header</span></span>|<span data-ttu-id="3d165-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3d165-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d165-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3d165-123">Authorization</span></span>|<span data-ttu-id="3d165-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3d165-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d165-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d165-125">Accept</span></span>|<span data-ttu-id="3d165-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d165-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d165-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3d165-127">Request body</span></span>
<span data-ttu-id="3d165-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3d165-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d165-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d165-129">Response</span></span>
<span data-ttu-id="3d165-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [WindowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3d165-130">If successful, this method returns a `200 OK` response code and a collection of [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d165-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3d165-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d165-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d165-132">Request</span></span>
<span data-ttu-id="3d165-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3d165-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3d165-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d165-134">Response</span></span>
<span data-ttu-id="3d165-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3d165-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1865

{
  "value": [
    {
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
  ]
}
```





