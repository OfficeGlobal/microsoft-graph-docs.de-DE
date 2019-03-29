---
title: targetedManagedAppPolicyAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines targetedManagedAppPolicyAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0683f21d4a3d657936bc14a93e36a217bc2fa3b5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980761"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="c16c1-103">targetedManagedAppPolicyAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c16c1-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="c16c1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c16c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c16c1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c16c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c16c1-106">Aktualisieren der Eigenschaften eines [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c16c1-106">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c16c1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c16c1-107">Prerequisites</span></span>
<span data-ttu-id="c16c1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c16c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c16c1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c16c1-110">Permission type</span></span>|<span data-ttu-id="c16c1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c16c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c16c1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c16c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c16c1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c16c1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c16c1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c16c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c16c1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c16c1-115">Not supported.</span></span>|
|<span data-ttu-id="c16c1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c16c1-116">Application</span></span>|<span data-ttu-id="c16c1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c16c1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c16c1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c16c1-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c16c1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c16c1-119">Request headers</span></span>
|<span data-ttu-id="c16c1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c16c1-120">Header</span></span>|<span data-ttu-id="c16c1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c16c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c16c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c16c1-122">Authorization</span></span>|<span data-ttu-id="c16c1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c16c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c16c1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c16c1-124">Accept</span></span>|<span data-ttu-id="c16c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c16c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c16c1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c16c1-126">Request body</span></span>
<span data-ttu-id="c16c1-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c16c1-127">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="c16c1-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="c16c1-128">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="c16c1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c16c1-129">Property</span></span>|<span data-ttu-id="c16c1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c16c1-130">Type</span></span>|<span data-ttu-id="c16c1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c16c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c16c1-132">id</span><span class="sxs-lookup"><span data-stu-id="c16c1-132">id</span></span>|<span data-ttu-id="c16c1-133">String</span><span class="sxs-lookup"><span data-stu-id="c16c1-133">String</span></span>|<span data-ttu-id="c16c1-134">Id</span><span class="sxs-lookup"><span data-stu-id="c16c1-134">Id</span></span>|
|<span data-ttu-id="c16c1-135">target</span><span class="sxs-lookup"><span data-stu-id="c16c1-135">target</span></span>|[<span data-ttu-id="c16c1-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c16c1-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c16c1-137">Bezeichner für die Bereitstellung einer Gruppe oder App</span><span class="sxs-lookup"><span data-stu-id="c16c1-137">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="c16c1-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="c16c1-138">Response</span></span>
<span data-ttu-id="c16c1-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c16c1-139">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c16c1-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c16c1-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="c16c1-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c16c1-141">Request</span></span>
<span data-ttu-id="c16c1-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c16c1-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="c16c1-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c16c1-143">Response</span></span>
<span data-ttu-id="c16c1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c16c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




