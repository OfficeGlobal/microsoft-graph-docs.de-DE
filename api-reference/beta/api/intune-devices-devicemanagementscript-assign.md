---
title: Aktion zuweisen
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d9fe37f3bc04495ddd69afca4dd3fb105246ad6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978269"
---
# <a name="assign-action"></a><span data-ttu-id="4197a-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="4197a-103">assign action</span></span>

> <span data-ttu-id="4197a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4197a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4197a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4197a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4197a-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4197a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4197a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4197a-107">Prerequisites</span></span>
<span data-ttu-id="4197a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4197a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4197a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4197a-110">Permission type</span></span>|<span data-ttu-id="4197a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4197a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4197a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4197a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4197a-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4197a-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4197a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4197a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4197a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4197a-115">Not supported.</span></span>|
|<span data-ttu-id="4197a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4197a-116">Application</span></span>|<span data-ttu-id="4197a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4197a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4197a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4197a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4197a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4197a-119">Request headers</span></span>
|<span data-ttu-id="4197a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4197a-120">Header</span></span>|<span data-ttu-id="4197a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4197a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4197a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4197a-122">Authorization</span></span>|<span data-ttu-id="4197a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4197a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4197a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4197a-124">Accept</span></span>|<span data-ttu-id="4197a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4197a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4197a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4197a-126">Request body</span></span>
<span data-ttu-id="4197a-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="4197a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4197a-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="4197a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4197a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4197a-129">Property</span></span>|<span data-ttu-id="4197a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4197a-130">Type</span></span>|<span data-ttu-id="4197a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4197a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4197a-132">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="4197a-132">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="4197a-133">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="4197a-133">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="4197a-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="4197a-134">Not yet documented</span></span>|
|<span data-ttu-id="4197a-135">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="4197a-135">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="4197a-136">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="4197a-136">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="4197a-137">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="4197a-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4197a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="4197a-138">Response</span></span>
<span data-ttu-id="4197a-139">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4197a-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4197a-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4197a-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4197a-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4197a-141">Request</span></span>
<span data-ttu-id="4197a-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4197a-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign

Content-type: application/json
Content-length: 550

{
  "deviceManagementScriptGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
      "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
      "targetGroupId": "Target Group Id value"
    }
  ],
  "deviceManagementScriptAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
      "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4197a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="4197a-143">Response</span></span>
<span data-ttu-id="4197a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4197a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




