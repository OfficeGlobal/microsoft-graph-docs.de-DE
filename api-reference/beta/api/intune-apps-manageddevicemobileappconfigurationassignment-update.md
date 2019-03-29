---
title: Aktualisieren von „managedDeviceMobileAppConfigurationAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43c4c860c6f0600c7c2877e72fab1a114f0e3329
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974118"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="b3623-103">Aktualisieren von „managedDeviceMobileAppConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="b3623-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="b3623-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3623-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3623-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b3623-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3623-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b3623-106">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3623-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b3623-107">Prerequisites</span></span>
<span data-ttu-id="b3623-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3623-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3623-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3623-110">Permission type</span></span>|<span data-ttu-id="b3623-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3623-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3623-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3623-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3623-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3623-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b3623-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3623-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3623-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3623-115">Not supported.</span></span>|
|<span data-ttu-id="b3623-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b3623-116">Application</span></span>|<span data-ttu-id="b3623-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3623-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3623-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3623-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b3623-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3623-119">Request headers</span></span>
|<span data-ttu-id="b3623-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b3623-120">Header</span></span>|<span data-ttu-id="b3623-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b3623-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3623-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3623-122">Authorization</span></span>|<span data-ttu-id="b3623-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b3623-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3623-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b3623-124">Accept</span></span>|<span data-ttu-id="b3623-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3623-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3623-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3623-126">Request body</span></span>
<span data-ttu-id="b3623-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="b3623-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="b3623-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="b3623-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="b3623-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b3623-129">Property</span></span>|<span data-ttu-id="b3623-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b3623-130">Type</span></span>|<span data-ttu-id="b3623-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3623-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3623-132">id</span><span class="sxs-lookup"><span data-stu-id="b3623-132">id</span></span>|<span data-ttu-id="b3623-133">String</span><span class="sxs-lookup"><span data-stu-id="b3623-133">String</span></span>|<span data-ttu-id="b3623-134">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="b3623-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b3623-135">target</span><span class="sxs-lookup"><span data-stu-id="b3623-135">target</span></span>|[<span data-ttu-id="b3623-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b3623-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b3623-137">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="b3623-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="b3623-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3623-138">Response</span></span>
<span data-ttu-id="b3623-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b3623-139">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3623-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3623-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3623-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3623-141">Request</span></span>
<span data-ttu-id="b3623-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b3623-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b3623-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3623-143">Response</span></span>
<span data-ttu-id="b3623-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3623-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




