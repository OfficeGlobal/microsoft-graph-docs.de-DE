---
title: WindowsAutopilotDeploymentProfileAssignment erstellen
description: Erstellen eines neuen windowsAutopilotDeploymentProfileAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2617ce53ce660a50ad67d8846b361cba60a1cff3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959334"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="a07e2-103">WindowsAutopilotDeploymentProfileAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="a07e2-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="a07e2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a07e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a07e2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a07e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a07e2-106">Erstellen eines neuen [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a07e2-106">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a07e2-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a07e2-107">Prerequisites</span></span>
<span data-ttu-id="a07e2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a07e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a07e2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a07e2-110">Permission type</span></span>|<span data-ttu-id="a07e2-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a07e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a07e2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a07e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a07e2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07e2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a07e2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a07e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a07e2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a07e2-115">Not supported.</span></span>|
|<span data-ttu-id="a07e2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a07e2-116">Application</span></span>|<span data-ttu-id="a07e2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a07e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a07e2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a07e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a07e2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a07e2-119">Request headers</span></span>
|<span data-ttu-id="a07e2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a07e2-120">Header</span></span>|<span data-ttu-id="a07e2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a07e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a07e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a07e2-122">Authorization</span></span>|<span data-ttu-id="a07e2-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a07e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a07e2-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a07e2-124">Accept</span></span>|<span data-ttu-id="a07e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a07e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a07e2-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a07e2-126">Request body</span></span>
<span data-ttu-id="a07e2-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsAutopilotDeploymentProfileAssignment-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="a07e2-127">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="a07e2-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsAutopilotDeploymentProfileAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a07e2-128">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="a07e2-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a07e2-129">Property</span></span>|<span data-ttu-id="a07e2-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a07e2-130">Type</span></span>|<span data-ttu-id="a07e2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a07e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a07e2-132">id</span><span class="sxs-lookup"><span data-stu-id="a07e2-132">id</span></span>|<span data-ttu-id="a07e2-133">String</span><span class="sxs-lookup"><span data-stu-id="a07e2-133">String</span></span>|<span data-ttu-id="a07e2-134">Schlüssel der Zuweisung</span><span class="sxs-lookup"><span data-stu-id="a07e2-134">The key of the assignment.</span></span>|
|<span data-ttu-id="a07e2-135">target</span><span class="sxs-lookup"><span data-stu-id="a07e2-135">target</span></span>|[<span data-ttu-id="a07e2-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a07e2-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a07e2-137">Das Zuordnungsziel für das Windows Autopilot-Bereitstellungsprofil.</span><span class="sxs-lookup"><span data-stu-id="a07e2-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="a07e2-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="a07e2-138">Response</span></span>
<span data-ttu-id="a07e2-139">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a07e2-139">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a07e2-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a07e2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a07e2-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a07e2-141">Request</span></span>
<span data-ttu-id="a07e2-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a07e2-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a07e2-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="a07e2-143">Response</span></span>
<span data-ttu-id="a07e2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a07e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




