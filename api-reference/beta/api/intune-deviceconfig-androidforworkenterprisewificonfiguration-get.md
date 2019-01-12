---
title: Abrufen von androidForWorkEnterpriseWiFiConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des AndroidForWorkEnterpriseWiFiConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dfaf4f5b977697336ce9047109fd3a2ecf4c20a4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918973"
---
# <a name="get-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="e011f-103">Abrufen von androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="e011f-103">Get androidForWorkEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="e011f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e011f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e011f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e011f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e011f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e011f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e011f-107">Lesen Sie Eigenschaften und Beziehungen des [AndroidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e011f-107">Read properties and relationships of the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e011f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e011f-108">Prerequisites</span></span>
<span data-ttu-id="e011f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e011f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e011f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e011f-111">Permission type</span></span>|<span data-ttu-id="e011f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e011f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e011f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e011f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e011f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e011f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e011f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e011f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e011f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e011f-116">Not supported.</span></span>|
|<span data-ttu-id="e011f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e011f-117">Application</span></span>|<span data-ttu-id="e011f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e011f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e011f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e011f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e011f-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e011f-120">Optional query parameters</span></span>
<span data-ttu-id="e011f-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e011f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e011f-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e011f-122">Request headers</span></span>
|<span data-ttu-id="e011f-123">Header</span><span class="sxs-lookup"><span data-stu-id="e011f-123">Header</span></span>|<span data-ttu-id="e011f-124">Wert</span><span class="sxs-lookup"><span data-stu-id="e011f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e011f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e011f-125">Authorization</span></span>|<span data-ttu-id="e011f-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e011f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e011f-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e011f-127">Accept</span></span>|<span data-ttu-id="e011f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e011f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e011f-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e011f-129">Request body</span></span>
<span data-ttu-id="e011f-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e011f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e011f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e011f-131">Response</span></span>
<span data-ttu-id="e011f-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AndroidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e011f-132">If successful, this method returns a `200 OK` response code and [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e011f-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e011f-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e011f-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e011f-134">Request</span></span>
<span data-ttu-id="e011f-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e011f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e011f-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e011f-136">Response</span></span>
<span data-ttu-id="e011f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e011f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1005

{
  "value": {
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
}
```





