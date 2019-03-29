---
title: WindowsAutopilotDeploymentProfileAssignments aufListen
description: AufListen von Eigenschaften und Beziehungen der windowsAutopilotDeploymentProfileAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2eda5b4be50c3dd56871f31aa5bdce089139814e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973446"
---
# <a name="list-windowsautopilotdeploymentprofileassignments"></a><span data-ttu-id="fddfc-103">WindowsAutopilotDeploymentProfileAssignments aufListen</span><span class="sxs-lookup"><span data-stu-id="fddfc-103">List windowsAutopilotDeploymentProfileAssignments</span></span>

> <span data-ttu-id="fddfc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fddfc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fddfc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fddfc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fddfc-106">AufListen von Eigenschaften und Beziehungen der [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="fddfc-106">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fddfc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fddfc-107">Prerequisites</span></span>
<span data-ttu-id="fddfc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fddfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fddfc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fddfc-110">Permission type</span></span>|<span data-ttu-id="fddfc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fddfc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fddfc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fddfc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fddfc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fddfc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fddfc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fddfc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fddfc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fddfc-115">Not supported.</span></span>|
|<span data-ttu-id="fddfc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fddfc-116">Application</span></span>|<span data-ttu-id="fddfc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fddfc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fddfc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fddfc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="fddfc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fddfc-119">Request headers</span></span>
|<span data-ttu-id="fddfc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fddfc-120">Header</span></span>|<span data-ttu-id="fddfc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fddfc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fddfc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fddfc-122">Authorization</span></span>|<span data-ttu-id="fddfc-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fddfc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fddfc-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fddfc-124">Accept</span></span>|<span data-ttu-id="fddfc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fddfc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fddfc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fddfc-126">Request body</span></span>
<span data-ttu-id="fddfc-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fddfc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fddfc-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="fddfc-128">Response</span></span>
<span data-ttu-id="fddfc-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fddfc-129">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fddfc-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fddfc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fddfc-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fddfc-131">Request</span></span>
<span data-ttu-id="fddfc-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fddfc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

### <a name="response"></a><span data-ttu-id="fddfc-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="fddfc-133">Response</span></span>
<span data-ttu-id="fddfc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fddfc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
      "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




