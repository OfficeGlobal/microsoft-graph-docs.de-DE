---
title: targetedManagedAppPolicyAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines targetedManagedAppPolicyAssignment-Objekts.
ms.openlocfilehash: f165b66b016080d3461d8a512812373615e16a27
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059330"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="766e6-103">targetedManagedAppPolicyAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="766e6-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="766e6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="766e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="766e6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="766e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="766e6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="766e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="766e6-107">Aktualisieren der Eigenschaften eines [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="766e6-107">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="766e6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="766e6-108">Prerequisites</span></span>
<span data-ttu-id="766e6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="766e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="766e6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="766e6-111">Permission type</span></span>|<span data-ttu-id="766e6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="766e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="766e6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="766e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="766e6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="766e6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="766e6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="766e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="766e6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="766e6-116">Not supported.</span></span>|
|<span data-ttu-id="766e6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="766e6-117">Application</span></span>|<span data-ttu-id="766e6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="766e6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="766e6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="766e6-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="766e6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="766e6-120">Request headers</span></span>
|<span data-ttu-id="766e6-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="766e6-121">Header</span></span>|<span data-ttu-id="766e6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="766e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="766e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="766e6-123">Authorization</span></span>|<span data-ttu-id="766e6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="766e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="766e6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="766e6-125">Accept</span></span>|<span data-ttu-id="766e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="766e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="766e6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="766e6-127">Request body</span></span>
<span data-ttu-id="766e6-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="766e6-128">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="766e6-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="766e6-129">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="766e6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="766e6-130">Property</span></span>|<span data-ttu-id="766e6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="766e6-131">Type</span></span>|<span data-ttu-id="766e6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="766e6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="766e6-133">id</span><span class="sxs-lookup"><span data-stu-id="766e6-133">id</span></span>|<span data-ttu-id="766e6-134">String</span><span class="sxs-lookup"><span data-stu-id="766e6-134">String</span></span>|<span data-ttu-id="766e6-135">Id</span><span class="sxs-lookup"><span data-stu-id="766e6-135">Id</span></span>|
|<span data-ttu-id="766e6-136">target</span><span class="sxs-lookup"><span data-stu-id="766e6-136">target</span></span>|[<span data-ttu-id="766e6-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="766e6-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="766e6-138">Bezeichner für die Bereitstellung einer Gruppe oder App</span><span class="sxs-lookup"><span data-stu-id="766e6-138">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="766e6-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="766e6-139">Response</span></span>
<span data-ttu-id="766e6-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="766e6-140">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="766e6-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="766e6-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="766e6-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="766e6-142">Request</span></span>
<span data-ttu-id="766e6-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="766e6-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="766e6-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="766e6-144">Response</span></span>
<span data-ttu-id="766e6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="766e6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




