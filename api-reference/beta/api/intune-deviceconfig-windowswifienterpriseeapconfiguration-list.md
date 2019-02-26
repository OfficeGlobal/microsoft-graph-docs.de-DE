---
title: WindowsWifiEnterpriseEAPConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der windowsWifiEnterpriseEAPConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13da9a8db093dc66ce3ab046a12d60918cd393cc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149910"
---
# <a name="list-windowswifienterpriseeapconfigurations"></a><span data-ttu-id="bdb51-103">WindowsWifiEnterpriseEAPConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="bdb51-103">List windowsWifiEnterpriseEAPConfigurations</span></span>

> <span data-ttu-id="bdb51-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bdb51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdb51-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bdb51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdb51-106">AufListen von Eigenschaften und Beziehungen der [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="bdb51-106">List properties and relationships of the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdb51-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bdb51-107">Prerequisites</span></span>
<span data-ttu-id="bdb51-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bdb51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bdb51-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bdb51-110">Permission type</span></span>|<span data-ttu-id="bdb51-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bdb51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdb51-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bdb51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bdb51-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdb51-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bdb51-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bdb51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdb51-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bdb51-115">Not supported.</span></span>|
|<span data-ttu-id="bdb51-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bdb51-116">Application</span></span>|<span data-ttu-id="bdb51-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bdb51-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdb51-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdb51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bdb51-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bdb51-119">Request headers</span></span>
|<span data-ttu-id="bdb51-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bdb51-120">Header</span></span>|<span data-ttu-id="bdb51-121">Wert</span><span class="sxs-lookup"><span data-stu-id="bdb51-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdb51-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdb51-122">Authorization</span></span>|<span data-ttu-id="bdb51-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bdb51-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdb51-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bdb51-124">Accept</span></span>|<span data-ttu-id="bdb51-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bdb51-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdb51-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bdb51-126">Request body</span></span>
<span data-ttu-id="bdb51-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bdb51-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdb51-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdb51-128">Response</span></span>
<span data-ttu-id="bdb51-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bdb51-129">If successful, this method returns a `200 OK` response code and a collection of [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdb51-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bdb51-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdb51-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdb51-131">Request</span></span>
<span data-ttu-id="bdb51-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bdb51-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="bdb51-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdb51-133">Response</span></span>
<span data-ttu-id="bdb51-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bdb51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




