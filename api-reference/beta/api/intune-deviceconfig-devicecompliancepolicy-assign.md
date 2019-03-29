---
title: Aktion zuweisen
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bc193a057534c13e169eab6d0558cb0a752b8c2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962939"
---
# <a name="assign-action"></a><span data-ttu-id="14a3e-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="14a3e-103">assign action</span></span>

> <span data-ttu-id="14a3e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="14a3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14a3e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="14a3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14a3e-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="14a3e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14a3e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="14a3e-107">Prerequisites</span></span>
<span data-ttu-id="14a3e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14a3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14a3e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="14a3e-110">Permission type</span></span>|<span data-ttu-id="14a3e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="14a3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14a3e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="14a3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14a3e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a3e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14a3e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="14a3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14a3e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="14a3e-115">Not supported.</span></span>|
|<span data-ttu-id="14a3e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="14a3e-116">Application</span></span>|<span data-ttu-id="14a3e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="14a3e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14a3e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="14a3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="14a3e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="14a3e-119">Request headers</span></span>
|<span data-ttu-id="14a3e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="14a3e-120">Header</span></span>|<span data-ttu-id="14a3e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="14a3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14a3e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="14a3e-122">Authorization</span></span>|<span data-ttu-id="14a3e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="14a3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14a3e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="14a3e-124">Accept</span></span>|<span data-ttu-id="14a3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14a3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14a3e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="14a3e-126">Request body</span></span>
<span data-ttu-id="14a3e-127">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="14a3e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="14a3e-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="14a3e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="14a3e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="14a3e-129">Property</span></span>|<span data-ttu-id="14a3e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="14a3e-130">Type</span></span>|<span data-ttu-id="14a3e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14a3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14a3e-132">assignments</span><span class="sxs-lookup"><span data-stu-id="14a3e-132">assignments</span></span>|<span data-ttu-id="14a3e-133">Sammlung von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="14a3e-133">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="14a3e-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="14a3e-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="14a3e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="14a3e-135">Response</span></span>
<span data-ttu-id="14a3e-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="14a3e-136">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14a3e-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="14a3e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="14a3e-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="14a3e-138">Request</span></span>
<span data-ttu-id="14a3e-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="14a3e-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign

Content-type: application/json
Content-length: 280

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="14a3e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="14a3e-140">Response</span></span>
<span data-ttu-id="14a3e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="14a3e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




