---
title: DeviceManagementScriptAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DeviceManagementScriptAssignment-Objekts.
ms.openlocfilehash: c69cc71181eb1a46a3505e474991079e5e196590
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065465"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="436c9-103">DeviceManagementScriptAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="436c9-103">Update deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="436c9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="436c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="436c9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="436c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="436c9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="436c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="436c9-107">Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="436c9-107">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="436c9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="436c9-108">Prerequisites</span></span>
<span data-ttu-id="436c9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="436c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="436c9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="436c9-111">Permission type</span></span>|<span data-ttu-id="436c9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="436c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="436c9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="436c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="436c9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="436c9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="436c9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="436c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="436c9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="436c9-116">Not supported.</span></span>|
|<span data-ttu-id="436c9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="436c9-117">Application</span></span>|<span data-ttu-id="436c9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="436c9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="436c9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="436c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="436c9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="436c9-120">Request headers</span></span>
|<span data-ttu-id="436c9-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="436c9-121">Header</span></span>|<span data-ttu-id="436c9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="436c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="436c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="436c9-123">Authorization</span></span>|<span data-ttu-id="436c9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="436c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="436c9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="436c9-125">Accept</span></span>|<span data-ttu-id="436c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="436c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="436c9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="436c9-127">Request body</span></span>
<span data-ttu-id="436c9-128">Geben Sie im Textkörper Anforderung für das Objekt [DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="436c9-128">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="436c9-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="436c9-129">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="436c9-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="436c9-130">Property</span></span>|<span data-ttu-id="436c9-131">Typ</span><span class="sxs-lookup"><span data-stu-id="436c9-131">Type</span></span>|<span data-ttu-id="436c9-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="436c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="436c9-133">id</span><span class="sxs-lookup"><span data-stu-id="436c9-133">id</span></span>|<span data-ttu-id="436c9-134">String</span><span class="sxs-lookup"><span data-stu-id="436c9-134">String</span></span>|<span data-ttu-id="436c9-135">Taste der Gerät Management Skript Gruppe Zuordnung Entität.</span><span class="sxs-lookup"><span data-stu-id="436c9-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="436c9-136">target</span><span class="sxs-lookup"><span data-stu-id="436c9-136">target</span></span>|[<span data-ttu-id="436c9-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="436c9-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="436c9-138">Die Id des Azure Active Directory-Gruppe verwenden wir das Skript Inhaltsadressierung für.</span><span class="sxs-lookup"><span data-stu-id="436c9-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="436c9-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="436c9-139">Response</span></span>
<span data-ttu-id="436c9-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="436c9-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="436c9-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="436c9-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="436c9-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="436c9-142">Request</span></span>
<span data-ttu-id="436c9-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="436c9-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="436c9-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="436c9-144">Response</span></span>
<span data-ttu-id="436c9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="436c9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





