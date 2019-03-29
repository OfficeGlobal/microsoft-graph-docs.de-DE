---
title: WindowsAutopilotDeploymentProfileAssignment abrufen
description: Lesen von Eigenschaften und Beziehungen des windowsAutopilotDeploymentProfileAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 56d0979f64711024986e2230cefab3186f00f7f8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961168"
---
# <a name="get-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="2eb02-103">WindowsAutopilotDeploymentProfileAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="2eb02-103">Get windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="2eb02-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2eb02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2eb02-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2eb02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2eb02-106">Lesen von Eigenschaften und Beziehungen des [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2eb02-106">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2eb02-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2eb02-107">Prerequisites</span></span>
<span data-ttu-id="2eb02-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2eb02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2eb02-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2eb02-110">Permission type</span></span>|<span data-ttu-id="2eb02-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2eb02-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2eb02-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2eb02-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2eb02-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2eb02-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2eb02-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2eb02-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2eb02-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2eb02-115">Not supported.</span></span>|
|<span data-ttu-id="2eb02-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2eb02-116">Application</span></span>|<span data-ttu-id="2eb02-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2eb02-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2eb02-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2eb02-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2eb02-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2eb02-119">Optional query parameters</span></span>
<span data-ttu-id="2eb02-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2eb02-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2eb02-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2eb02-121">Request headers</span></span>
|<span data-ttu-id="2eb02-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2eb02-122">Header</span></span>|<span data-ttu-id="2eb02-123">Wert</span><span class="sxs-lookup"><span data-stu-id="2eb02-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2eb02-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2eb02-124">Authorization</span></span>|<span data-ttu-id="2eb02-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2eb02-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2eb02-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2eb02-126">Accept</span></span>|<span data-ttu-id="2eb02-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2eb02-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eb02-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2eb02-128">Request body</span></span>
<span data-ttu-id="2eb02-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2eb02-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2eb02-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="2eb02-130">Response</span></span>
<span data-ttu-id="2eb02-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2eb02-131">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2eb02-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2eb02-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2eb02-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2eb02-133">Request</span></span>
<span data-ttu-id="2eb02-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2eb02-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="2eb02-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2eb02-135">Response</span></span>
<span data-ttu-id="2eb02-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2eb02-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
    "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




