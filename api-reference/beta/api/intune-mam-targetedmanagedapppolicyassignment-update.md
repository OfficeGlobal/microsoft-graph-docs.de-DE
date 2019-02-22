---
title: targetedManagedAppPolicyAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines targetedManagedAppPolicyAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3864da7ce775e9dc37b44ac9f491bc1f6b917110
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169111"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="cacbd-103">targetedManagedAppPolicyAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="cacbd-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="cacbd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cacbd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cacbd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cacbd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cacbd-106">Aktualisieren der Eigenschaften eines [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cacbd-106">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cacbd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cacbd-107">Prerequisites</span></span>
<span data-ttu-id="cacbd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cacbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cacbd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cacbd-110">Permission type</span></span>|<span data-ttu-id="cacbd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cacbd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cacbd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cacbd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cacbd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cacbd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cacbd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cacbd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cacbd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cacbd-115">Not supported.</span></span>|
|<span data-ttu-id="cacbd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cacbd-116">Application</span></span>|<span data-ttu-id="cacbd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cacbd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cacbd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cacbd-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="cacbd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cacbd-119">Request headers</span></span>
|<span data-ttu-id="cacbd-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cacbd-120">Header</span></span>|<span data-ttu-id="cacbd-121">Wert</span><span class="sxs-lookup"><span data-stu-id="cacbd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cacbd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cacbd-122">Authorization</span></span>|<span data-ttu-id="cacbd-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cacbd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cacbd-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cacbd-124">Accept</span></span>|<span data-ttu-id="cacbd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cacbd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cacbd-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cacbd-126">Request body</span></span>
<span data-ttu-id="cacbd-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="cacbd-127">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="cacbd-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="cacbd-128">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="cacbd-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cacbd-129">Property</span></span>|<span data-ttu-id="cacbd-130">Typ</span><span class="sxs-lookup"><span data-stu-id="cacbd-130">Type</span></span>|<span data-ttu-id="cacbd-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cacbd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cacbd-132">id</span><span class="sxs-lookup"><span data-stu-id="cacbd-132">id</span></span>|<span data-ttu-id="cacbd-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cacbd-133">String</span></span>|<span data-ttu-id="cacbd-134">Id</span><span class="sxs-lookup"><span data-stu-id="cacbd-134">Id</span></span>|
|<span data-ttu-id="cacbd-135">target</span><span class="sxs-lookup"><span data-stu-id="cacbd-135">target</span></span>|[<span data-ttu-id="cacbd-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cacbd-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cacbd-137">Bezeichner für die Bereitstellung einer Gruppe oder App</span><span class="sxs-lookup"><span data-stu-id="cacbd-137">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="cacbd-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="cacbd-138">Response</span></span>
<span data-ttu-id="cacbd-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cacbd-139">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cacbd-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cacbd-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="cacbd-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cacbd-141">Request</span></span>
<span data-ttu-id="cacbd-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cacbd-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cacbd-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="cacbd-143">Response</span></span>
<span data-ttu-id="cacbd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cacbd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




