---
title: AndroidForWorkEnterpriseWiFiConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der androidForWorkEnterpriseWiFiConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5dc91b25fde99639880239abf6e7550541dfeaa
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145458"
---
# <a name="list-androidforworkenterprisewificonfigurations"></a><span data-ttu-id="ab735-103">AndroidForWorkEnterpriseWiFiConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="ab735-103">List androidForWorkEnterpriseWiFiConfigurations</span></span>

> <span data-ttu-id="ab735-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ab735-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab735-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ab735-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab735-106">AufListen von Eigenschaften und Beziehungen der [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="ab735-106">List properties and relationships of the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab735-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ab735-107">Prerequisites</span></span>
<span data-ttu-id="ab735-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ab735-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ab735-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ab735-110">Permission type</span></span>|<span data-ttu-id="ab735-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ab735-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab735-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ab735-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab735-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab735-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ab735-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ab735-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab735-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab735-115">Not supported.</span></span>|
|<span data-ttu-id="ab735-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ab735-116">Application</span></span>|<span data-ttu-id="ab735-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab735-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab735-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab735-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ab735-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ab735-119">Request headers</span></span>
|<span data-ttu-id="ab735-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ab735-120">Header</span></span>|<span data-ttu-id="ab735-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ab735-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab735-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab735-122">Authorization</span></span>|<span data-ttu-id="ab735-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ab735-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab735-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ab735-124">Accept</span></span>|<span data-ttu-id="ab735-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ab735-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab735-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ab735-126">Request body</span></span>
<span data-ttu-id="ab735-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ab735-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab735-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab735-128">Response</span></span>
<span data-ttu-id="ab735-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ab735-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab735-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ab735-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab735-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab735-131">Request</span></span>
<span data-ttu-id="ab735-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ab735-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ab735-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab735-133">Response</span></span>
<span data-ttu-id="ab735-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ab735-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1061

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
      "id": "742d953a-953a-742d-3a95-2d743a952d74",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "networkName": "Network Name value",
      "ssid": "Ssid value",
      "connectAutomatically": true,
      "connectWhenNetworkNameIsHidden": true,
      "wiFiSecurityType": "wpaEnterprise",
      "eapType": "eapTtls",
      "authenticationMethod": "usernameAndPassword",
      "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
      "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
      "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
    }
  ]
}
```




