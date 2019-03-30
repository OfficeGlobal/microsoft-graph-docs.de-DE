---
title: targetedManagedAppPolicyAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines targetedManagedAppPolicyAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32e03d719a631e1237eafac4404f9a9607dde188
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988056"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="7939a-103">targetedManagedAppPolicyAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7939a-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="7939a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7939a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7939a-105">Aktualisieren der Eigenschaften eines [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7939a-105">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7939a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7939a-106">Prerequisites</span></span>
<span data-ttu-id="7939a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7939a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7939a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7939a-109">Permission type</span></span>|<span data-ttu-id="7939a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7939a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7939a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7939a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7939a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7939a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7939a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7939a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7939a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7939a-114">Not supported.</span></span>|
|<span data-ttu-id="7939a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7939a-115">Application</span></span>|<span data-ttu-id="7939a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7939a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7939a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7939a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7939a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7939a-118">Request headers</span></span>
|<span data-ttu-id="7939a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7939a-119">Header</span></span>|<span data-ttu-id="7939a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7939a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7939a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7939a-121">Authorization</span></span>|<span data-ttu-id="7939a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7939a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7939a-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7939a-123">Accept</span></span>|<span data-ttu-id="7939a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7939a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7939a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7939a-125">Request body</span></span>
<span data-ttu-id="7939a-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7939a-126">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="7939a-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7939a-127">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="7939a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7939a-128">Property</span></span>|<span data-ttu-id="7939a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7939a-129">Type</span></span>|<span data-ttu-id="7939a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7939a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7939a-131">id</span><span class="sxs-lookup"><span data-stu-id="7939a-131">id</span></span>|<span data-ttu-id="7939a-132">String</span><span class="sxs-lookup"><span data-stu-id="7939a-132">String</span></span>|<span data-ttu-id="7939a-133">Id</span><span class="sxs-lookup"><span data-stu-id="7939a-133">Id</span></span>|
|<span data-ttu-id="7939a-134">target</span><span class="sxs-lookup"><span data-stu-id="7939a-134">target</span></span>|[<span data-ttu-id="7939a-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7939a-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7939a-136">Bezeichner für die Bereitstellung einer Gruppe oder App</span><span class="sxs-lookup"><span data-stu-id="7939a-136">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="7939a-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="7939a-137">Response</span></span>
<span data-ttu-id="7939a-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7939a-138">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7939a-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7939a-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="7939a-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7939a-140">Request</span></span>
<span data-ttu-id="7939a-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7939a-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="7939a-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="7939a-142">Response</span></span>
<span data-ttu-id="7939a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7939a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



