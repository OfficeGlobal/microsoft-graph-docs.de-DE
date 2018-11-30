---
title: DeviceManagementScriptGroupAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DeviceManagementScriptGroupAssignment-Objekts.
ms.openlocfilehash: 35313860e7d2dc2d2bd6ef5380245c00c69c53d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058443"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="40cf3-103">DeviceManagementScriptGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="40cf3-103">Update deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="40cf3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="40cf3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40cf3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40cf3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40cf3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="40cf3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40cf3-107">Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="40cf3-107">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40cf3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="40cf3-108">Prerequisites</span></span>
<span data-ttu-id="40cf3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40cf3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40cf3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40cf3-111">Permission type</span></span>|<span data-ttu-id="40cf3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40cf3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40cf3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40cf3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40cf3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40cf3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="40cf3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40cf3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40cf3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40cf3-116">Not supported.</span></span>|
|<span data-ttu-id="40cf3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40cf3-117">Application</span></span>|<span data-ttu-id="40cf3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40cf3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40cf3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40cf3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="40cf3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40cf3-120">Request headers</span></span>
|<span data-ttu-id="40cf3-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="40cf3-121">Header</span></span>|<span data-ttu-id="40cf3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="40cf3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40cf3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40cf3-123">Authorization</span></span>|<span data-ttu-id="40cf3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="40cf3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40cf3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="40cf3-125">Accept</span></span>|<span data-ttu-id="40cf3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40cf3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40cf3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40cf3-127">Request body</span></span>
<span data-ttu-id="40cf3-128">Geben Sie im Textkörper Anforderung für das Objekt [DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="40cf3-128">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="40cf3-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="40cf3-129">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="40cf3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40cf3-130">Property</span></span>|<span data-ttu-id="40cf3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="40cf3-131">Type</span></span>|<span data-ttu-id="40cf3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40cf3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40cf3-133">id</span><span class="sxs-lookup"><span data-stu-id="40cf3-133">id</span></span>|<span data-ttu-id="40cf3-134">String</span><span class="sxs-lookup"><span data-stu-id="40cf3-134">String</span></span>|<span data-ttu-id="40cf3-135">Taste der Gerät Management Skript Gruppe Zuordnung Entität.</span><span class="sxs-lookup"><span data-stu-id="40cf3-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="40cf3-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="40cf3-136">targetGroupId</span></span>|<span data-ttu-id="40cf3-137">String</span><span class="sxs-lookup"><span data-stu-id="40cf3-137">String</span></span>|<span data-ttu-id="40cf3-138">Die Id des Azure Active Directory-Gruppe verwenden wir das Skript Inhaltsadressierung für.</span><span class="sxs-lookup"><span data-stu-id="40cf3-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="40cf3-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="40cf3-139">Response</span></span>
<span data-ttu-id="40cf3-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="40cf3-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40cf3-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40cf3-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="40cf3-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40cf3-142">Request</span></span>
<span data-ttu-id="40cf3-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40cf3-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 48

{
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="40cf3-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="40cf3-144">Response</span></span>
<span data-ttu-id="40cf3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40cf3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```





