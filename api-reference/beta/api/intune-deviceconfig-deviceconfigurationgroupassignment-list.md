---
title: DeviceConfigurationGroupAssignments aufListen
description: AufListen von Eigenschaften und Beziehungen der deviceConfigurationGroupAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2f5d8262aa3b8c0cc19c4c85631a0a23a7aa5ba8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976540"
---
# <a name="list-deviceconfigurationgroupassignments"></a><span data-ttu-id="2d3fe-103">DeviceConfigurationGroupAssignments aufListen</span><span class="sxs-lookup"><span data-stu-id="2d3fe-103">List deviceConfigurationGroupAssignments</span></span>

> <span data-ttu-id="2d3fe-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d3fe-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d3fe-106">AufListen von Eigenschaften und Beziehungen der [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-106">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d3fe-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2d3fe-107">Prerequisites</span></span>
<span data-ttu-id="2d3fe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d3fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d3fe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2d3fe-110">Permission type</span></span>|<span data-ttu-id="2d3fe-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2d3fe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d3fe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2d3fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d3fe-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d3fe-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2d3fe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2d3fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d3fe-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d3fe-115">Not supported.</span></span>|
|<span data-ttu-id="2d3fe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2d3fe-116">Application</span></span>|<span data-ttu-id="2d3fe-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2d3fe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d3fe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d3fe-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2d3fe-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2d3fe-119">Request headers</span></span>
|<span data-ttu-id="2d3fe-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2d3fe-120">Header</span></span>|<span data-ttu-id="2d3fe-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2d3fe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d3fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d3fe-122">Authorization</span></span>|<span data-ttu-id="2d3fe-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2d3fe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d3fe-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2d3fe-124">Accept</span></span>|<span data-ttu-id="2d3fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d3fe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d3fe-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2d3fe-126">Request body</span></span>
<span data-ttu-id="2d3fe-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d3fe-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d3fe-128">Response</span></span>
<span data-ttu-id="2d3fe-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d3fe-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2d3fe-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d3fe-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2d3fe-131">Request</span></span>
<span data-ttu-id="2d3fe-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="2d3fe-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="2d3fe-133">Response</span></span>
<span data-ttu-id="2d3fe-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




