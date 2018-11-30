---
title: Erstellen von deviceManagementScriptGroupAssignment
description: Erstellen eines neuen DeviceManagementScriptGroupAssignment-Objekts.
ms.openlocfilehash: 3a92632ad1ab900ddff8371ce37bedb4f16f6d55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058781"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="f0ed8-103">Erstellen von deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f0ed8-103">Create deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="f0ed8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f0ed8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0ed8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f0ed8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0ed8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f0ed8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0ed8-107">Erstellen eines neuen [DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f0ed8-107">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0ed8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f0ed8-108">Prerequisites</span></span>
<span data-ttu-id="f0ed8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0ed8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0ed8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f0ed8-111">Permission type</span></span>|<span data-ttu-id="f0ed8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f0ed8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0ed8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f0ed8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0ed8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0ed8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f0ed8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f0ed8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0ed8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f0ed8-116">Not supported.</span></span>|
|<span data-ttu-id="f0ed8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f0ed8-117">Application</span></span>|<span data-ttu-id="f0ed8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f0ed8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0ed8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0ed8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="f0ed8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f0ed8-120">Request headers</span></span>
|<span data-ttu-id="f0ed8-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f0ed8-121">Header</span></span>|<span data-ttu-id="f0ed8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f0ed8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0ed8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0ed8-123">Authorization</span></span>|<span data-ttu-id="f0ed8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f0ed8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0ed8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0ed8-125">Accept</span></span>|<span data-ttu-id="f0ed8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0ed8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0ed8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f0ed8-127">Request body</span></span>
<span data-ttu-id="f0ed8-128">Geben Sie im Textkörper Anforderung für das Objekt DeviceManagementScriptGroupAssignment eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f0ed8-128">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="f0ed8-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DeviceManagementScriptGroupAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="f0ed8-129">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="f0ed8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0ed8-130">Property</span></span>|<span data-ttu-id="f0ed8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f0ed8-131">Type</span></span>|<span data-ttu-id="f0ed8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0ed8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0ed8-133">id</span><span class="sxs-lookup"><span data-stu-id="f0ed8-133">id</span></span>|<span data-ttu-id="f0ed8-134">String</span><span class="sxs-lookup"><span data-stu-id="f0ed8-134">String</span></span>|<span data-ttu-id="f0ed8-135">Taste der Gerät Management Skript Gruppe Zuordnung Entität.</span><span class="sxs-lookup"><span data-stu-id="f0ed8-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="f0ed8-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="f0ed8-136">targetGroupId</span></span>|<span data-ttu-id="f0ed8-137">String</span><span class="sxs-lookup"><span data-stu-id="f0ed8-137">String</span></span>|<span data-ttu-id="f0ed8-138">Die Id des Azure Active Directory-Gruppe verwenden wir das Skript Inhaltsadressierung für.</span><span class="sxs-lookup"><span data-stu-id="f0ed8-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="f0ed8-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0ed8-139">Response</span></span>
<span data-ttu-id="f0ed8-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f0ed8-140">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0ed8-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f0ed8-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0ed8-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0ed8-142">Request</span></span>
<span data-ttu-id="f0ed8-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f0ed8-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="f0ed8-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0ed8-144">Response</span></span>
<span data-ttu-id="f0ed8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f0ed8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```





