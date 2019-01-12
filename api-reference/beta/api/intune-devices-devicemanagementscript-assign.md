---
title: Aktion „assign“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a3a54693fcb2c689827e41d811cd616d428dc83f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934394"
---
# <a name="assign-action"></a><span data-ttu-id="ea9d1-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="ea9d1-103">assign action</span></span>

> <span data-ttu-id="ea9d1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ea9d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea9d1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ea9d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea9d1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ea9d1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea9d1-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ea9d1-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea9d1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ea9d1-108">Prerequisites</span></span>
<span data-ttu-id="ea9d1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea9d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea9d1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ea9d1-111">Permission type</span></span>|<span data-ttu-id="ea9d1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ea9d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea9d1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ea9d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea9d1-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea9d1-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ea9d1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ea9d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea9d1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea9d1-116">Not supported.</span></span>|
|<span data-ttu-id="ea9d1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ea9d1-117">Application</span></span>|<span data-ttu-id="ea9d1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea9d1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea9d1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea9d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="ea9d1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea9d1-120">Request headers</span></span>
|<span data-ttu-id="ea9d1-121">Header</span><span class="sxs-lookup"><span data-stu-id="ea9d1-121">Header</span></span>|<span data-ttu-id="ea9d1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ea9d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea9d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea9d1-123">Authorization</span></span>|<span data-ttu-id="ea9d1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ea9d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea9d1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ea9d1-125">Accept</span></span>|<span data-ttu-id="ea9d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea9d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea9d1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea9d1-127">Request body</span></span>
<span data-ttu-id="ea9d1-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="ea9d1-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ea9d1-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="ea9d1-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ea9d1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ea9d1-130">Property</span></span>|<span data-ttu-id="ea9d1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ea9d1-131">Type</span></span>|<span data-ttu-id="ea9d1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea9d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea9d1-133">deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="ea9d1-133">deviceManagementScriptGroupAssignments</span></span>|<span data-ttu-id="ea9d1-134">[DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ea9d1-134">[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) collection</span></span>|<span data-ttu-id="ea9d1-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ea9d1-135">Not yet documented</span></span>|
|<span data-ttu-id="ea9d1-136">deviceManagementScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="ea9d1-136">deviceManagementScriptAssignments</span></span>|<span data-ttu-id="ea9d1-137">[DeviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ea9d1-137">[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) collection</span></span>|<span data-ttu-id="ea9d1-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ea9d1-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ea9d1-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea9d1-139">Response</span></span>
<span data-ttu-id="ea9d1-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="ea9d1-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ea9d1-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ea9d1-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea9d1-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea9d1-142">Request</span></span>
<span data-ttu-id="ea9d1-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea9d1-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ea9d1-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea9d1-144">Response</span></span>
<span data-ttu-id="ea9d1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea9d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





