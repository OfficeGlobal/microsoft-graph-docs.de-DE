---
title: DeviceManagementScriptAssignment erstellen
description: Erstellen eines neuen deviceManagementScriptAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11147c2b273da300d5c9f9123b8dde7e49d8d2cc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975406"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="ff7b7-103">DeviceManagementScriptAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="ff7b7-103">Create deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="ff7b7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff7b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff7b7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ff7b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff7b7-106">Erstellen eines neuen [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ff7b7-106">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff7b7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ff7b7-107">Prerequisites</span></span>
<span data-ttu-id="ff7b7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff7b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff7b7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff7b7-110">Permission type</span></span>|<span data-ttu-id="ff7b7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff7b7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff7b7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff7b7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff7b7-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff7b7-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ff7b7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff7b7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff7b7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff7b7-115">Not supported.</span></span>|
|<span data-ttu-id="ff7b7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff7b7-116">Application</span></span>|<span data-ttu-id="ff7b7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff7b7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff7b7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff7b7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ff7b7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff7b7-119">Request headers</span></span>
|<span data-ttu-id="ff7b7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ff7b7-120">Header</span></span>|<span data-ttu-id="ff7b7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ff7b7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff7b7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff7b7-122">Authorization</span></span>|<span data-ttu-id="ff7b7-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ff7b7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff7b7-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ff7b7-124">Accept</span></span>|<span data-ttu-id="ff7b7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff7b7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff7b7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff7b7-126">Request body</span></span>
<span data-ttu-id="ff7b7-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceManagementScriptAssignment-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ff7b7-127">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="ff7b7-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceManagementScriptAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ff7b7-128">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="ff7b7-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff7b7-129">Property</span></span>|<span data-ttu-id="ff7b7-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ff7b7-130">Type</span></span>|<span data-ttu-id="ff7b7-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff7b7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff7b7-132">id</span><span class="sxs-lookup"><span data-stu-id="ff7b7-132">id</span></span>|<span data-ttu-id="ff7b7-133">String</span><span class="sxs-lookup"><span data-stu-id="ff7b7-133">String</span></span>|<span data-ttu-id="ff7b7-134">Schlüssel der Zuordnungs Entität "Device Management Script Group".</span><span class="sxs-lookup"><span data-stu-id="ff7b7-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="ff7b7-135">target</span><span class="sxs-lookup"><span data-stu-id="ff7b7-135">target</span></span>|[<span data-ttu-id="ff7b7-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ff7b7-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ff7b7-137">Die ID der Azure Active Directory-Gruppe, auf die wir das Skript ausrichten.</span><span class="sxs-lookup"><span data-stu-id="ff7b7-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="ff7b7-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff7b7-138">Response</span></span>
<span data-ttu-id="ff7b7-139">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ff7b7-139">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff7b7-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff7b7-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff7b7-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff7b7-141">Request</span></span>
<span data-ttu-id="ff7b7-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff7b7-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ff7b7-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff7b7-143">Response</span></span>
<span data-ttu-id="ff7b7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff7b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




