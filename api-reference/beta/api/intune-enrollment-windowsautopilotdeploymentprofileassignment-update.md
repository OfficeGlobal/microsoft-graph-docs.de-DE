---
title: WindowsAutopilotDeploymentProfileAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines windowsAutopilotDeploymentProfileAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e73550b19c1dfa4dd8bc6159408201282c4e07a2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155251"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="456a6-103">WindowsAutopilotDeploymentProfileAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="456a6-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="456a6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="456a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="456a6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="456a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="456a6-106">Aktualisieren der Eigenschaften eines [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="456a6-106">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="456a6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="456a6-107">Prerequisites</span></span>
<span data-ttu-id="456a6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="456a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="456a6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="456a6-110">Permission type</span></span>|<span data-ttu-id="456a6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="456a6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="456a6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="456a6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="456a6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="456a6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="456a6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="456a6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="456a6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="456a6-115">Not supported.</span></span>|
|<span data-ttu-id="456a6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="456a6-116">Application</span></span>|<span data-ttu-id="456a6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="456a6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="456a6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="456a6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="456a6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="456a6-119">Request headers</span></span>
|<span data-ttu-id="456a6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="456a6-120">Header</span></span>|<span data-ttu-id="456a6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="456a6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="456a6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="456a6-122">Authorization</span></span>|<span data-ttu-id="456a6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="456a6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="456a6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="456a6-124">Accept</span></span>|<span data-ttu-id="456a6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="456a6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="456a6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="456a6-126">Request body</span></span>
<span data-ttu-id="456a6-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="456a6-127">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="456a6-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="456a6-128">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="456a6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="456a6-129">Property</span></span>|<span data-ttu-id="456a6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="456a6-130">Type</span></span>|<span data-ttu-id="456a6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="456a6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="456a6-132">id</span><span class="sxs-lookup"><span data-stu-id="456a6-132">id</span></span>|<span data-ttu-id="456a6-133">String</span><span class="sxs-lookup"><span data-stu-id="456a6-133">String</span></span>|<span data-ttu-id="456a6-134">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="456a6-134">The key of the assignment.</span></span>|
|<span data-ttu-id="456a6-135">target</span><span class="sxs-lookup"><span data-stu-id="456a6-135">target</span></span>|[<span data-ttu-id="456a6-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="456a6-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="456a6-137">Das Zuordnungsziel für das Windows Autopilot-Bereitstellungsprofil.</span><span class="sxs-lookup"><span data-stu-id="456a6-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="456a6-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="456a6-138">Response</span></span>
<span data-ttu-id="456a6-139">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="456a6-139">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="456a6-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="456a6-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="456a6-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="456a6-141">Request</span></span>
<span data-ttu-id="456a6-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="456a6-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="456a6-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="456a6-143">Response</span></span>
<span data-ttu-id="456a6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="456a6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




