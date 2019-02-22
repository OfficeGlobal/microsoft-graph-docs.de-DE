---
title: Erstellen von „deviceCompliancePolicyAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs deviceCompliancePolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34004c6529958994a372e8e665f95999e0f624ab
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145332"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="c5c0f-103">Erstellen von „deviceCompliancePolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="c5c0f-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="c5c0f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5c0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5c0f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c5c0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5c0f-106">Diese Methode erstellt ein neues Objekt des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c5c0f-106">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5c0f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c5c0f-107">Prerequisites</span></span>
<span data-ttu-id="c5c0f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5c0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c5c0f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c5c0f-110">Permission type</span></span>|<span data-ttu-id="c5c0f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c5c0f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5c0f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c5c0f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5c0f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5c0f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5c0f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c5c0f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5c0f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5c0f-115">Not supported.</span></span>|
|<span data-ttu-id="c5c0f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c5c0f-116">Application</span></span>|<span data-ttu-id="c5c0f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5c0f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5c0f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5c0f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c5c0f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5c0f-119">Request headers</span></span>
|<span data-ttu-id="c5c0f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c5c0f-120">Header</span></span>|<span data-ttu-id="c5c0f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c5c0f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5c0f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5c0f-122">Authorization</span></span>|<span data-ttu-id="c5c0f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c5c0f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5c0f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c5c0f-124">Accept</span></span>|<span data-ttu-id="c5c0f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5c0f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5c0f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c5c0f-126">Request body</span></span>
<span data-ttu-id="c5c0f-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceCompliancePolicyAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="c5c0f-127">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="c5c0f-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceCompliancePolicyAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="c5c0f-128">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="c5c0f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5c0f-129">Property</span></span>|<span data-ttu-id="c5c0f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c5c0f-130">Type</span></span>|<span data-ttu-id="c5c0f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5c0f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5c0f-132">id</span><span class="sxs-lookup"><span data-stu-id="c5c0f-132">id</span></span>|<span data-ttu-id="c5c0f-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5c0f-133">String</span></span>|<span data-ttu-id="c5c0f-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c5c0f-134">Key of the entity.</span></span>|
|<span data-ttu-id="c5c0f-135">target</span><span class="sxs-lookup"><span data-stu-id="c5c0f-135">target</span></span>|[<span data-ttu-id="c5c0f-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c5c0f-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c5c0f-137">Ziel der Zuweisung der Konformitätsrichtlinie</span><span class="sxs-lookup"><span data-stu-id="c5c0f-137">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="c5c0f-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5c0f-138">Response</span></span>
<span data-ttu-id="c5c0f-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c5c0f-139">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5c0f-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5c0f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5c0f-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5c0f-141">Request</span></span>
<span data-ttu-id="c5c0f-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5c0f-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c5c0f-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5c0f-143">Response</span></span>
<span data-ttu-id="c5c0f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5c0f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




