---
title: Erstellen von windowsAutopilotDeploymentProfileAssignment
description: Erstellen eines neuen WindowsAutopilotDeploymentProfileAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a336ac9540c90cdebf452a08037bd46d5fa33d01
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983625"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="dd028-103">Erstellen von windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="dd028-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="dd028-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dd028-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd028-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd028-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd028-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dd028-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd028-107">Erstellen eines neuen [WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="dd028-107">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd028-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dd028-108">Prerequisites</span></span>
<span data-ttu-id="dd028-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd028-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd028-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd028-111">Permission type</span></span>|<span data-ttu-id="dd028-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd028-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd028-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd028-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd028-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd028-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dd028-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd028-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd028-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd028-116">Not supported.</span></span>|
|<span data-ttu-id="dd028-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd028-117">Application</span></span>|<span data-ttu-id="dd028-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd028-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd028-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd028-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="dd028-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd028-120">Request headers</span></span>
|<span data-ttu-id="dd028-121">Header</span><span class="sxs-lookup"><span data-stu-id="dd028-121">Header</span></span>|<span data-ttu-id="dd028-122">Wert</span><span class="sxs-lookup"><span data-stu-id="dd028-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd028-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd028-123">Authorization</span></span>|<span data-ttu-id="dd028-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dd028-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd028-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dd028-125">Accept</span></span>|<span data-ttu-id="dd028-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd028-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd028-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd028-127">Request body</span></span>
<span data-ttu-id="dd028-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsAutopilotDeploymentProfileAssignment eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="dd028-128">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="dd028-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsAutopilotDeploymentProfileAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="dd028-129">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="dd028-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dd028-130">Property</span></span>|<span data-ttu-id="dd028-131">Typ</span><span class="sxs-lookup"><span data-stu-id="dd028-131">Type</span></span>|<span data-ttu-id="dd028-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd028-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd028-133">id</span><span class="sxs-lookup"><span data-stu-id="dd028-133">id</span></span>|<span data-ttu-id="dd028-134">String</span><span class="sxs-lookup"><span data-stu-id="dd028-134">String</span></span>|<span data-ttu-id="dd028-135">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="dd028-135">The key of the assignment.</span></span>|
|<span data-ttu-id="dd028-136">target</span><span class="sxs-lookup"><span data-stu-id="dd028-136">target</span></span>|[<span data-ttu-id="dd028-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="dd028-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="dd028-138">Das Ziel der Zuordnung für das Windows Autopilot Bereitstellungsprofil.</span><span class="sxs-lookup"><span data-stu-id="dd028-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="dd028-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd028-139">Response</span></span>
<span data-ttu-id="dd028-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="dd028-140">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd028-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd028-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd028-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd028-142">Request</span></span>
<span data-ttu-id="dd028-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd028-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="dd028-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd028-144">Response</span></span>
<span data-ttu-id="dd028-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd028-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





