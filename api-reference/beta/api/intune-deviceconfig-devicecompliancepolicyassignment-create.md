---
title: Erstellen von „deviceCompliancePolicyAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs deviceCompliancePolicyAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3fb7372bf769366ef83999a82461ce0cc6563066
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414907"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="9c2c0-103">Erstellen von „deviceCompliancePolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="9c2c0-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="9c2c0-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9c2c0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9c2c0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9c2c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c2c0-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9c2c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c2c0-107">Diese Methode erstellt ein neues Objekt des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9c2c0-107">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c2c0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9c2c0-108">Prerequisites</span></span>
<span data-ttu-id="9c2c0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9c2c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9c2c0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c2c0-111">Permission type</span></span>|<span data-ttu-id="9c2c0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c2c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c2c0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c2c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c2c0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c2c0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c2c0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c2c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c2c0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c2c0-116">Not supported.</span></span>|
|<span data-ttu-id="9c2c0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c2c0-117">Application</span></span>|<span data-ttu-id="9c2c0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c2c0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c2c0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c2c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9c2c0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c2c0-120">Request headers</span></span>
|<span data-ttu-id="9c2c0-121">Header</span><span class="sxs-lookup"><span data-stu-id="9c2c0-121">Header</span></span>|<span data-ttu-id="9c2c0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9c2c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c2c0-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9c2c0-123">Authorization</span></span>|<span data-ttu-id="9c2c0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9c2c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c2c0-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9c2c0-125">Accept</span></span>|<span data-ttu-id="9c2c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c2c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c2c0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c2c0-127">Request body</span></span>
<span data-ttu-id="9c2c0-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceCompliancePolicyAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="9c2c0-128">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="9c2c0-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceCompliancePolicyAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="9c2c0-129">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="9c2c0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9c2c0-130">Property</span></span>|<span data-ttu-id="9c2c0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9c2c0-131">Type</span></span>|<span data-ttu-id="9c2c0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c2c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c2c0-133">id</span><span class="sxs-lookup"><span data-stu-id="9c2c0-133">id</span></span>|<span data-ttu-id="9c2c0-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9c2c0-134">String</span></span>|<span data-ttu-id="9c2c0-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9c2c0-135">Key of the entity.</span></span>|
|<span data-ttu-id="9c2c0-136">target</span><span class="sxs-lookup"><span data-stu-id="9c2c0-136">target</span></span>|[<span data-ttu-id="9c2c0-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9c2c0-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9c2c0-138">Ziel der Zuweisung der Konformitätsrichtlinie</span><span class="sxs-lookup"><span data-stu-id="9c2c0-138">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="9c2c0-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c2c0-139">Response</span></span>
<span data-ttu-id="9c2c0-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9c2c0-140">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c2c0-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c2c0-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c2c0-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c2c0-142">Request</span></span>
<span data-ttu-id="9c2c0-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9c2c0-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9c2c0-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c2c0-144">Response</span></span>
<span data-ttu-id="9c2c0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c2c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




