---
title: WindowsAutopilotDeploymentProfileAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsAutopilotDeploymentProfileAssignment-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8267019105d42260ec346595680ea8d4805c35dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408089"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="3d21d-103">WindowsAutopilotDeploymentProfileAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3d21d-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="3d21d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3d21d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3d21d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3d21d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d21d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3d21d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d21d-107">Aktualisieren Sie die Eigenschaften eines [WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3d21d-107">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d21d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3d21d-108">Prerequisites</span></span>
<span data-ttu-id="3d21d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3d21d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3d21d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3d21d-111">Permission type</span></span>|<span data-ttu-id="3d21d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3d21d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d21d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3d21d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d21d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d21d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3d21d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3d21d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d21d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d21d-116">Not supported.</span></span>|
|<span data-ttu-id="3d21d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3d21d-117">Application</span></span>|<span data-ttu-id="3d21d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d21d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d21d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d21d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3d21d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3d21d-120">Request headers</span></span>
|<span data-ttu-id="3d21d-121">Header</span><span class="sxs-lookup"><span data-stu-id="3d21d-121">Header</span></span>|<span data-ttu-id="3d21d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3d21d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d21d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3d21d-123">Authorization</span></span>|<span data-ttu-id="3d21d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3d21d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d21d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3d21d-125">Accept</span></span>|<span data-ttu-id="3d21d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d21d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d21d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3d21d-127">Request body</span></span>
<span data-ttu-id="3d21d-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="3d21d-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="3d21d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="3d21d-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="3d21d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d21d-130">Property</span></span>|<span data-ttu-id="3d21d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3d21d-131">Type</span></span>|<span data-ttu-id="3d21d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d21d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d21d-133">id</span><span class="sxs-lookup"><span data-stu-id="3d21d-133">id</span></span>|<span data-ttu-id="3d21d-134">String</span><span class="sxs-lookup"><span data-stu-id="3d21d-134">String</span></span>|<span data-ttu-id="3d21d-135">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="3d21d-135">The key of the assignment.</span></span>|
|<span data-ttu-id="3d21d-136">target</span><span class="sxs-lookup"><span data-stu-id="3d21d-136">target</span></span>|[<span data-ttu-id="3d21d-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3d21d-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3d21d-138">Das Ziel der Zuordnung für das Windows Autopilot Bereitstellungsprofil.</span><span class="sxs-lookup"><span data-stu-id="3d21d-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="3d21d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d21d-139">Response</span></span>
<span data-ttu-id="3d21d-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3d21d-140">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d21d-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3d21d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d21d-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d21d-142">Request</span></span>
<span data-ttu-id="3d21d-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3d21d-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="3d21d-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d21d-144">Response</span></span>
<span data-ttu-id="3d21d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3d21d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




