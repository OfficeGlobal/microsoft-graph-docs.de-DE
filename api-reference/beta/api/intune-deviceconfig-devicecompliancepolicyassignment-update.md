---
title: Aktualisieren von „deviceCompliancePolicyAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCompliancePolicyAssignment.
ms.openlocfilehash: f472403ff97d2cce4fa7f24f9f75028652d56171
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063009"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="21d24-103">Aktualisieren von „deviceCompliancePolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="21d24-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="21d24-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="21d24-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21d24-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21d24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21d24-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="21d24-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21d24-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="21d24-107">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21d24-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="21d24-108">Prerequisites</span></span>
<span data-ttu-id="21d24-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21d24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21d24-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21d24-111">Permission type</span></span>|<span data-ttu-id="21d24-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21d24-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21d24-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21d24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21d24-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21d24-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21d24-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21d24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21d24-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21d24-116">Not supported.</span></span>|
|<span data-ttu-id="21d24-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21d24-117">Application</span></span>|<span data-ttu-id="21d24-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21d24-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21d24-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21d24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="21d24-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21d24-120">Request headers</span></span>
|<span data-ttu-id="21d24-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="21d24-121">Header</span></span>|<span data-ttu-id="21d24-122">Wert</span><span class="sxs-lookup"><span data-stu-id="21d24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21d24-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21d24-123">Authorization</span></span>|<span data-ttu-id="21d24-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="21d24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21d24-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21d24-125">Accept</span></span>|<span data-ttu-id="21d24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21d24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21d24-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21d24-127">Request body</span></span>
<span data-ttu-id="21d24-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="21d24-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="21d24-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="21d24-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="21d24-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21d24-130">Property</span></span>|<span data-ttu-id="21d24-131">Typ</span><span class="sxs-lookup"><span data-stu-id="21d24-131">Type</span></span>|<span data-ttu-id="21d24-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21d24-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21d24-133">id</span><span class="sxs-lookup"><span data-stu-id="21d24-133">id</span></span>|<span data-ttu-id="21d24-134">String</span><span class="sxs-lookup"><span data-stu-id="21d24-134">String</span></span>|<span data-ttu-id="21d24-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="21d24-135">Key of the entity.</span></span>|
|<span data-ttu-id="21d24-136">target</span><span class="sxs-lookup"><span data-stu-id="21d24-136">target</span></span>|[<span data-ttu-id="21d24-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="21d24-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="21d24-138">Ziel der Zuweisung der Konformitätsrichtlinie</span><span class="sxs-lookup"><span data-stu-id="21d24-138">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="21d24-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="21d24-139">Response</span></span>
<span data-ttu-id="21d24-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="21d24-140">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21d24-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21d24-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="21d24-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21d24-142">Request</span></span>
<span data-ttu-id="21d24-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21d24-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="21d24-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="21d24-144">Response</span></span>
<span data-ttu-id="21d24-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21d24-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





