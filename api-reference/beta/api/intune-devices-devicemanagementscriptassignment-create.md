---
title: Erstellen von deviceManagementScriptAssignment
description: Erstellen eines neuen DeviceManagementScriptAssignment-Objekts.
ms.openlocfilehash: 7191b08e0517e219e8fcc97778424ed3e35540ea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063529"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="d599c-103">Erstellen von deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="d599c-103">Create deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="d599c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d599c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d599c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d599c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d599c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d599c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d599c-107">Erstellen eines neuen [DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d599c-107">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d599c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d599c-108">Prerequisites</span></span>
<span data-ttu-id="d599c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d599c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d599c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d599c-111">Permission type</span></span>|<span data-ttu-id="d599c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d599c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d599c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d599c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d599c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d599c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d599c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d599c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d599c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d599c-116">Not supported.</span></span>|
|<span data-ttu-id="d599c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d599c-117">Application</span></span>|<span data-ttu-id="d599c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d599c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d599c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d599c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d599c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d599c-120">Request headers</span></span>
|<span data-ttu-id="d599c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d599c-121">Header</span></span>|<span data-ttu-id="d599c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d599c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d599c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d599c-123">Authorization</span></span>|<span data-ttu-id="d599c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d599c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d599c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d599c-125">Accept</span></span>|<span data-ttu-id="d599c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d599c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d599c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d599c-127">Request body</span></span>
<span data-ttu-id="d599c-128">Geben Sie im Textkörper Anforderung für das Objekt DeviceManagementScriptAssignment eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d599c-128">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="d599c-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DeviceManagementScriptAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="d599c-129">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="d599c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d599c-130">Property</span></span>|<span data-ttu-id="d599c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d599c-131">Type</span></span>|<span data-ttu-id="d599c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d599c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d599c-133">id</span><span class="sxs-lookup"><span data-stu-id="d599c-133">id</span></span>|<span data-ttu-id="d599c-134">String</span><span class="sxs-lookup"><span data-stu-id="d599c-134">String</span></span>|<span data-ttu-id="d599c-135">Taste der Gerät Management Skript Gruppe Zuordnung Entität.</span><span class="sxs-lookup"><span data-stu-id="d599c-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="d599c-136">target</span><span class="sxs-lookup"><span data-stu-id="d599c-136">target</span></span>|[<span data-ttu-id="d599c-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d599c-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d599c-138">Die Id des Azure Active Directory-Gruppe verwenden wir das Skript Inhaltsadressierung für.</span><span class="sxs-lookup"><span data-stu-id="d599c-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="d599c-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="d599c-139">Response</span></span>
<span data-ttu-id="d599c-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d599c-140">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d599c-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d599c-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="d599c-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d599c-142">Request</span></span>
<span data-ttu-id="d599c-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d599c-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d599c-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="d599c-144">Response</span></span>
<span data-ttu-id="d599c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d599c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





