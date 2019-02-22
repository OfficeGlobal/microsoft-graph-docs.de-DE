---
title: DeviceManagementScriptGroupAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines deviceManagementScriptGroupAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1b13eabebcce3fffcaf4b817eb75aeb9ae13701
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160634"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="0ad76-103">DeviceManagementScriptGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0ad76-103">Update deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="0ad76-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ad76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ad76-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0ad76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ad76-106">Aktualisieren der Eigenschaften eines [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0ad76-106">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ad76-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0ad76-107">Prerequisites</span></span>
<span data-ttu-id="0ad76-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0ad76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0ad76-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0ad76-110">Permission type</span></span>|<span data-ttu-id="0ad76-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0ad76-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ad76-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0ad76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ad76-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ad76-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0ad76-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0ad76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ad76-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ad76-115">Not supported.</span></span>|
|<span data-ttu-id="0ad76-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0ad76-116">Application</span></span>|<span data-ttu-id="0ad76-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ad76-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ad76-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ad76-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="0ad76-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0ad76-119">Request headers</span></span>
|<span data-ttu-id="0ad76-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0ad76-120">Header</span></span>|<span data-ttu-id="0ad76-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0ad76-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ad76-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ad76-122">Authorization</span></span>|<span data-ttu-id="0ad76-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0ad76-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ad76-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0ad76-124">Accept</span></span>|<span data-ttu-id="0ad76-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ad76-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ad76-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0ad76-126">Request body</span></span>
<span data-ttu-id="0ad76-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="0ad76-127">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="0ad76-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0ad76-128">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="0ad76-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0ad76-129">Property</span></span>|<span data-ttu-id="0ad76-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0ad76-130">Type</span></span>|<span data-ttu-id="0ad76-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ad76-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ad76-132">id</span><span class="sxs-lookup"><span data-stu-id="0ad76-132">id</span></span>|<span data-ttu-id="0ad76-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ad76-133">String</span></span>|<span data-ttu-id="0ad76-134">Schlüssel der Zuordnungs Entität "Device Management Script Group".</span><span class="sxs-lookup"><span data-stu-id="0ad76-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="0ad76-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="0ad76-135">targetGroupId</span></span>|<span data-ttu-id="0ad76-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ad76-136">String</span></span>|<span data-ttu-id="0ad76-137">Die ID der Azure Active Directory-Gruppe, auf die wir das Skript ausrichten.</span><span class="sxs-lookup"><span data-stu-id="0ad76-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="0ad76-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ad76-138">Response</span></span>
<span data-ttu-id="0ad76-139">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0ad76-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ad76-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0ad76-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ad76-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ad76-141">Request</span></span>
<span data-ttu-id="0ad76-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0ad76-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="0ad76-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ad76-143">Response</span></span>
<span data-ttu-id="0ad76-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ad76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




