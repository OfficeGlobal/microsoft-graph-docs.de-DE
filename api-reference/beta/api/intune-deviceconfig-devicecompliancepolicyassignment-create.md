---
title: Erstellen von „deviceCompliancePolicyAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs deviceCompliancePolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3c181e7362528fe0231e2e744f59ac82d7ee333e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847957"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="02a75-103">Erstellen von „deviceCompliancePolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="02a75-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="02a75-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="02a75-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02a75-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02a75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02a75-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="02a75-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02a75-107">Diese Methode erstellt ein neues Objekt des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="02a75-107">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02a75-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="02a75-108">Prerequisites</span></span>
<span data-ttu-id="02a75-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02a75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a75-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02a75-111">Permission type</span></span>|<span data-ttu-id="02a75-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02a75-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02a75-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02a75-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02a75-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a75-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02a75-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02a75-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02a75-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02a75-116">Not supported.</span></span>|
|<span data-ttu-id="02a75-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02a75-117">Application</span></span>|<span data-ttu-id="02a75-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02a75-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02a75-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02a75-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="02a75-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="02a75-120">Request headers</span></span>
|<span data-ttu-id="02a75-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="02a75-121">Header</span></span>|<span data-ttu-id="02a75-122">Wert</span><span class="sxs-lookup"><span data-stu-id="02a75-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02a75-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02a75-123">Authorization</span></span>|<span data-ttu-id="02a75-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="02a75-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02a75-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="02a75-125">Accept</span></span>|<span data-ttu-id="02a75-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02a75-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02a75-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="02a75-127">Request body</span></span>
<span data-ttu-id="02a75-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceCompliancePolicyAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="02a75-128">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="02a75-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceCompliancePolicyAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="02a75-129">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="02a75-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02a75-130">Property</span></span>|<span data-ttu-id="02a75-131">Typ</span><span class="sxs-lookup"><span data-stu-id="02a75-131">Type</span></span>|<span data-ttu-id="02a75-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02a75-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02a75-133">id</span><span class="sxs-lookup"><span data-stu-id="02a75-133">id</span></span>|<span data-ttu-id="02a75-134">String</span><span class="sxs-lookup"><span data-stu-id="02a75-134">String</span></span>|<span data-ttu-id="02a75-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="02a75-135">Key of the entity.</span></span>|
|<span data-ttu-id="02a75-136">target</span><span class="sxs-lookup"><span data-stu-id="02a75-136">target</span></span>|[<span data-ttu-id="02a75-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="02a75-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="02a75-138">Ziel der Zuweisung der Konformitätsrichtlinie</span><span class="sxs-lookup"><span data-stu-id="02a75-138">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="02a75-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="02a75-139">Response</span></span>
<span data-ttu-id="02a75-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="02a75-140">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02a75-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="02a75-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="02a75-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02a75-142">Request</span></span>
<span data-ttu-id="02a75-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="02a75-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="02a75-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="02a75-144">Response</span></span>
<span data-ttu-id="02a75-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02a75-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





