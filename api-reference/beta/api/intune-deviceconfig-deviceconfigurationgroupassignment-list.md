---
title: Liste deviceConfigurationGroupAssignments
description: Listeneigenschaften und Beziehungen der DeviceConfigurationGroupAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 34e222c249f25f854c5b5183fccbbb46738c4f10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807784"
---
# <a name="list-deviceconfigurationgroupassignments"></a><span data-ttu-id="11390-103">Liste deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="11390-103">List deviceConfigurationGroupAssignments</span></span>

> <span data-ttu-id="11390-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="11390-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11390-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="11390-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11390-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="11390-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11390-107">Listeneigenschaften und Beziehungen der [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="11390-107">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11390-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="11390-108">Prerequisites</span></span>
<span data-ttu-id="11390-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11390-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11390-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11390-111">Permission type</span></span>|<span data-ttu-id="11390-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11390-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11390-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11390-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11390-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="11390-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="11390-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11390-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11390-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11390-116">Not supported.</span></span>|
|<span data-ttu-id="11390-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11390-117">Application</span></span>|<span data-ttu-id="11390-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11390-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11390-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11390-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="11390-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11390-120">Request headers</span></span>
|<span data-ttu-id="11390-121">Header</span><span class="sxs-lookup"><span data-stu-id="11390-121">Header</span></span>|<span data-ttu-id="11390-122">Wert</span><span class="sxs-lookup"><span data-stu-id="11390-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11390-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="11390-123">Authorization</span></span>|<span data-ttu-id="11390-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="11390-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11390-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="11390-125">Accept</span></span>|<span data-ttu-id="11390-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11390-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11390-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11390-127">Request body</span></span>
<span data-ttu-id="11390-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="11390-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11390-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="11390-129">Response</span></span>
<span data-ttu-id="11390-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="11390-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11390-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11390-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="11390-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11390-132">Request</span></span>
<span data-ttu-id="11390-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11390-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="11390-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="11390-134">Response</span></span>
<span data-ttu-id="11390-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11390-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 244

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ]
}
```





