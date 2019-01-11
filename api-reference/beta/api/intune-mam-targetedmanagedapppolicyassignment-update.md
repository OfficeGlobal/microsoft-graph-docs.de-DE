---
title: targetedManagedAppPolicyAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines targetedManagedAppPolicyAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 09e2d3685bdfd9fde586612294a386b79bb58f0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858828"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="a9a52-103">targetedManagedAppPolicyAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a9a52-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="a9a52-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a9a52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9a52-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a9a52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9a52-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a9a52-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9a52-107">Aktualisieren der Eigenschaften eines [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a9a52-107">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9a52-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a9a52-108">Prerequisites</span></span>
<span data-ttu-id="a9a52-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9a52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9a52-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a9a52-111">Permission type</span></span>|<span data-ttu-id="a9a52-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a9a52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9a52-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a9a52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9a52-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9a52-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a9a52-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a9a52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9a52-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9a52-116">Not supported.</span></span>|
|<span data-ttu-id="a9a52-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a9a52-117">Application</span></span>|<span data-ttu-id="a9a52-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9a52-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9a52-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9a52-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a9a52-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a9a52-120">Request headers</span></span>
|<span data-ttu-id="a9a52-121">Header</span><span class="sxs-lookup"><span data-stu-id="a9a52-121">Header</span></span>|<span data-ttu-id="a9a52-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a9a52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9a52-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9a52-123">Authorization</span></span>|<span data-ttu-id="a9a52-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a9a52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9a52-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a9a52-125">Accept</span></span>|<span data-ttu-id="a9a52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9a52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9a52-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a9a52-127">Request body</span></span>
<span data-ttu-id="a9a52-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a9a52-128">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="a9a52-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a9a52-129">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="a9a52-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a9a52-130">Property</span></span>|<span data-ttu-id="a9a52-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a9a52-131">Type</span></span>|<span data-ttu-id="a9a52-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a9a52-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9a52-133">id</span><span class="sxs-lookup"><span data-stu-id="a9a52-133">id</span></span>|<span data-ttu-id="a9a52-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9a52-134">String</span></span>|<span data-ttu-id="a9a52-135">Id</span><span class="sxs-lookup"><span data-stu-id="a9a52-135">Id</span></span>|
|<span data-ttu-id="a9a52-136">target</span><span class="sxs-lookup"><span data-stu-id="a9a52-136">target</span></span>|[<span data-ttu-id="a9a52-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a9a52-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a9a52-138">Bezeichner für die Bereitstellung einer Gruppe oder App</span><span class="sxs-lookup"><span data-stu-id="a9a52-138">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="a9a52-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9a52-139">Response</span></span>
<span data-ttu-id="a9a52-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a9a52-140">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9a52-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a9a52-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9a52-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9a52-142">Request</span></span>
<span data-ttu-id="a9a52-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a9a52-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a9a52-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9a52-144">Response</span></span>
<span data-ttu-id="a9a52-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a9a52-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





