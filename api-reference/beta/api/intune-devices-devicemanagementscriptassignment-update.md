---
title: DeviceManagementScriptAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementScriptAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35085405f8b28066f3774e9f27fe1471e2cc1654
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153424"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="73282-103">DeviceManagementScriptAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="73282-103">Update deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="73282-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="73282-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73282-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="73282-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73282-106">Aktualisieren der Eigenschaften eines [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="73282-106">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73282-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="73282-107">Prerequisites</span></span>
<span data-ttu-id="73282-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="73282-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="73282-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73282-110">Permission type</span></span>|<span data-ttu-id="73282-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73282-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73282-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73282-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73282-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73282-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="73282-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73282-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73282-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73282-115">Not supported.</span></span>|
|<span data-ttu-id="73282-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73282-116">Application</span></span>|<span data-ttu-id="73282-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73282-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73282-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73282-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="73282-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73282-119">Request headers</span></span>
|<span data-ttu-id="73282-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="73282-120">Header</span></span>|<span data-ttu-id="73282-121">Wert</span><span class="sxs-lookup"><span data-stu-id="73282-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73282-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73282-122">Authorization</span></span>|<span data-ttu-id="73282-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="73282-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73282-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="73282-124">Accept</span></span>|<span data-ttu-id="73282-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73282-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73282-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73282-126">Request body</span></span>
<span data-ttu-id="73282-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="73282-127">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="73282-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="73282-128">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="73282-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73282-129">Property</span></span>|<span data-ttu-id="73282-130">Typ</span><span class="sxs-lookup"><span data-stu-id="73282-130">Type</span></span>|<span data-ttu-id="73282-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73282-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73282-132">id</span><span class="sxs-lookup"><span data-stu-id="73282-132">id</span></span>|<span data-ttu-id="73282-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73282-133">String</span></span>|<span data-ttu-id="73282-134">Schlüssel der Zuordnungs Entität "Device Management Script Group".</span><span class="sxs-lookup"><span data-stu-id="73282-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="73282-135">target</span><span class="sxs-lookup"><span data-stu-id="73282-135">target</span></span>|[<span data-ttu-id="73282-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="73282-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="73282-137">Die ID der Azure Active Directory-Gruppe, auf die wir das Skript ausrichten.</span><span class="sxs-lookup"><span data-stu-id="73282-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="73282-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="73282-138">Response</span></span>
<span data-ttu-id="73282-139">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="73282-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73282-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73282-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="73282-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73282-141">Request</span></span>
<span data-ttu-id="73282-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73282-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="73282-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="73282-143">Response</span></span>
<span data-ttu-id="73282-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73282-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




