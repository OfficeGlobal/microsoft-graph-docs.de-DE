---
title: Liste windowsAutopilotDeploymentProfileAssignments
description: Listeneigenschaften und Beziehungen der WindowsAutopilotDeploymentProfileAssignment-Objekte.
author: tfitzmac
ms.openlocfilehash: 46751889ef197f56ea0681a354b276a695185a23
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308526"
---
# <a name="list-windowsautopilotdeploymentprofileassignments"></a><span data-ttu-id="11a39-103">Liste windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="11a39-103">List windowsAutopilotDeploymentProfileAssignments</span></span>

> <span data-ttu-id="11a39-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="11a39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11a39-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="11a39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11a39-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="11a39-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11a39-107">Listeneigenschaften und Beziehungen der [WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="11a39-107">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11a39-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="11a39-108">Prerequisites</span></span>
<span data-ttu-id="11a39-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11a39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11a39-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11a39-111">Permission type</span></span>|<span data-ttu-id="11a39-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11a39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11a39-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11a39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11a39-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="11a39-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="11a39-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11a39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11a39-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11a39-116">Not supported.</span></span>|
|<span data-ttu-id="11a39-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11a39-117">Application</span></span>|<span data-ttu-id="11a39-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11a39-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11a39-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11a39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="11a39-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11a39-120">Request headers</span></span>
|<span data-ttu-id="11a39-121">Header</span><span class="sxs-lookup"><span data-stu-id="11a39-121">Header</span></span>|<span data-ttu-id="11a39-122">Wert</span><span class="sxs-lookup"><span data-stu-id="11a39-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11a39-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="11a39-123">Authorization</span></span>|<span data-ttu-id="11a39-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="11a39-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11a39-125">Accept</span><span class="sxs-lookup"><span data-stu-id="11a39-125">Accept</span></span>|<span data-ttu-id="11a39-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11a39-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11a39-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11a39-127">Request body</span></span>
<span data-ttu-id="11a39-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="11a39-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11a39-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="11a39-129">Response</span></span>
<span data-ttu-id="11a39-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="11a39-130">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11a39-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11a39-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="11a39-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11a39-132">Request</span></span>
<span data-ttu-id="11a39-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11a39-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

### <a name="response"></a><span data-ttu-id="11a39-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="11a39-134">Response</span></span>
<span data-ttu-id="11a39-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11a39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





