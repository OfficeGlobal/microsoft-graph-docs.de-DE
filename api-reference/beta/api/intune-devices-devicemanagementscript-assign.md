---
title: Aktion zuweisen
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 189e7c73220ed88735ada7052367db589ad2905e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171330"
---
# <a name="assign-action"></a><span data-ttu-id="d14b5-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="d14b5-103">assign action</span></span>

> <span data-ttu-id="d14b5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d14b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d14b5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d14b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d14b5-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d14b5-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d14b5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d14b5-107">Prerequisites</span></span>
<span data-ttu-id="d14b5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d14b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d14b5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d14b5-110">Permission type</span></span>|<span data-ttu-id="d14b5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d14b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d14b5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d14b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d14b5-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d14b5-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d14b5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d14b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d14b5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d14b5-115">Not supported.</span></span>|
|<span data-ttu-id="d14b5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d14b5-116">Application</span></span>|<span data-ttu-id="d14b5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d14b5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d14b5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d14b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d14b5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d14b5-119">Request headers</span></span>
|<span data-ttu-id="d14b5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d14b5-120">Header</span></span>|<span data-ttu-id="d14b5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d14b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d14b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d14b5-122">Authorization</span></span>|<span data-ttu-id="d14b5-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d14b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d14b5-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d14b5-124">Accept</span></span>|<span data-ttu-id="d14b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d14b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d14b5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d14b5-126">Request body</span></span>
<span data-ttu-id="d14b5-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="d14b5-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d14b5-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="d14b5-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d14b5-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d14b5-129">Property</span></span>|<span data-ttu-id="d14b5-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d14b5-130">Type</span></span>|<span data-ttu-id="d14b5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d14b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d14b5-132">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="d14b5-132">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="d14b5-133">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d14b5-133">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="d14b5-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d14b5-134">Not yet documented</span></span>|
|<span data-ttu-id="d14b5-135">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="d14b5-135">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="d14b5-136">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d14b5-136">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="d14b5-137">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d14b5-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d14b5-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="d14b5-138">Response</span></span>
<span data-ttu-id="d14b5-139">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="d14b5-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d14b5-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d14b5-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d14b5-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d14b5-141">Request</span></span>
<span data-ttu-id="d14b5-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d14b5-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d14b5-143">Reaktion</span><span class="sxs-lookup"><span data-stu-id="d14b5-143">Response</span></span>
<span data-ttu-id="d14b5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d14b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




