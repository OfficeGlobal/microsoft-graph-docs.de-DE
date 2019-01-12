---
title: targetedManagedAppPolicyAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines targetedManagedAppPolicyAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5d20413017c9a1063204273574bb9b24e8ba31b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927765"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="949f7-103">targetedManagedAppPolicyAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="949f7-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="949f7-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="949f7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="949f7-105">Aktualisieren der Eigenschaften eines [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="949f7-105">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="949f7-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="949f7-106">Prerequisites</span></span>
<span data-ttu-id="949f7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="949f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="949f7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="949f7-109">Permission type</span></span>|<span data-ttu-id="949f7-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="949f7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="949f7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="949f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="949f7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="949f7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="949f7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="949f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="949f7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="949f7-114">Not supported.</span></span>|
|<span data-ttu-id="949f7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="949f7-115">Application</span></span>|<span data-ttu-id="949f7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="949f7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="949f7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="949f7-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="949f7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="949f7-118">Request headers</span></span>
|<span data-ttu-id="949f7-119">Header</span><span class="sxs-lookup"><span data-stu-id="949f7-119">Header</span></span>|<span data-ttu-id="949f7-120">Wert</span><span class="sxs-lookup"><span data-stu-id="949f7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="949f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="949f7-121">Authorization</span></span>|<span data-ttu-id="949f7-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="949f7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="949f7-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="949f7-123">Accept</span></span>|<span data-ttu-id="949f7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="949f7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="949f7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="949f7-125">Request body</span></span>
<span data-ttu-id="949f7-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="949f7-126">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="949f7-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="949f7-127">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="949f7-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="949f7-128">Property</span></span>|<span data-ttu-id="949f7-129">Typ</span><span class="sxs-lookup"><span data-stu-id="949f7-129">Type</span></span>|<span data-ttu-id="949f7-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="949f7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="949f7-131">id</span><span class="sxs-lookup"><span data-stu-id="949f7-131">id</span></span>|<span data-ttu-id="949f7-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="949f7-132">String</span></span>|<span data-ttu-id="949f7-133">Id</span><span class="sxs-lookup"><span data-stu-id="949f7-133">Id</span></span>|
|<span data-ttu-id="949f7-134">target</span><span class="sxs-lookup"><span data-stu-id="949f7-134">target</span></span>|[<span data-ttu-id="949f7-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="949f7-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="949f7-136">Bezeichner für die Bereitstellung einer Gruppe oder App</span><span class="sxs-lookup"><span data-stu-id="949f7-136">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="949f7-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="949f7-137">Response</span></span>
<span data-ttu-id="949f7-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="949f7-138">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="949f7-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="949f7-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="949f7-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="949f7-140">Request</span></span>
<span data-ttu-id="949f7-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="949f7-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="949f7-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="949f7-142">Response</span></span>
<span data-ttu-id="949f7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="949f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



