---
title: Aktualisieren von „managedDeviceMobileAppConfigurationAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceMobileAppConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dccf48cfefb0e5a9f09fd51e998a1172280f72d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982567"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="5f05a-103">Aktualisieren von „managedDeviceMobileAppConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="5f05a-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="5f05a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5f05a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f05a-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5f05a-105">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f05a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5f05a-106">Prerequisites</span></span>
<span data-ttu-id="5f05a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f05a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f05a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f05a-109">Permission type</span></span>|<span data-ttu-id="5f05a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f05a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f05a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f05a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5f05a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f05a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5f05a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f05a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f05a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f05a-114">Not supported.</span></span>|
|<span data-ttu-id="5f05a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f05a-115">Application</span></span>|<span data-ttu-id="5f05a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f05a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f05a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f05a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5f05a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f05a-118">Request headers</span></span>
|<span data-ttu-id="5f05a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5f05a-119">Header</span></span>|<span data-ttu-id="5f05a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5f05a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f05a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f05a-121">Authorization</span></span>|<span data-ttu-id="5f05a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5f05a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f05a-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5f05a-123">Accept</span></span>|<span data-ttu-id="5f05a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5f05a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f05a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5f05a-125">Request body</span></span>
<span data-ttu-id="5f05a-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="5f05a-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="5f05a-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="5f05a-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="5f05a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f05a-128">Property</span></span>|<span data-ttu-id="5f05a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5f05a-129">Type</span></span>|<span data-ttu-id="5f05a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f05a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f05a-131">id</span><span class="sxs-lookup"><span data-stu-id="5f05a-131">id</span></span>|<span data-ttu-id="5f05a-132">String</span><span class="sxs-lookup"><span data-stu-id="5f05a-132">String</span></span>|<span data-ttu-id="5f05a-133">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="5f05a-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5f05a-134">target</span><span class="sxs-lookup"><span data-stu-id="5f05a-134">target</span></span>|[<span data-ttu-id="5f05a-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5f05a-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5f05a-136">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="5f05a-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="5f05a-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f05a-137">Response</span></span>
<span data-ttu-id="5f05a-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5f05a-138">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f05a-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f05a-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f05a-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f05a-140">Request</span></span>
<span data-ttu-id="5f05a-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5f05a-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="5f05a-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f05a-142">Response</span></span>
<span data-ttu-id="5f05a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f05a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



