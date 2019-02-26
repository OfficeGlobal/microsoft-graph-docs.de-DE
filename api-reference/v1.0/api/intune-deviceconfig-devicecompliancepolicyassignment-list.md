---
title: Auflisten von „deviceCompliancePolicyAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceCompliancePolicyAssignment auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 047f8b3c6bb1fb5c4ca2113a72abcb32fad84130
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263959"
---
# <a name="list-devicecompliancepolicyassignments"></a><span data-ttu-id="218eb-103">Auflisten von „deviceCompliancePolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="218eb-103">List deviceCompliancePolicyAssignments</span></span>

> <span data-ttu-id="218eb-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="218eb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="218eb-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="218eb-105">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="218eb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="218eb-106">Prerequisites</span></span>
<span data-ttu-id="218eb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="218eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="218eb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="218eb-109">Permission type</span></span>|<span data-ttu-id="218eb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="218eb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="218eb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="218eb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="218eb-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="218eb-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="218eb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="218eb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="218eb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="218eb-114">Not supported.</span></span>|
|<span data-ttu-id="218eb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="218eb-115">Application</span></span>|<span data-ttu-id="218eb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="218eb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="218eb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="218eb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="218eb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="218eb-118">Request headers</span></span>
|<span data-ttu-id="218eb-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="218eb-119">Header</span></span>|<span data-ttu-id="218eb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="218eb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="218eb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="218eb-121">Authorization</span></span>|<span data-ttu-id="218eb-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="218eb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="218eb-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="218eb-123">Accept</span></span>|<span data-ttu-id="218eb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="218eb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="218eb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="218eb-125">Request body</span></span>
<span data-ttu-id="218eb-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="218eb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="218eb-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="218eb-127">Response</span></span>
<span data-ttu-id="218eb-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="218eb-128">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="218eb-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="218eb-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="218eb-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="218eb-130">Request</span></span>
<span data-ttu-id="218eb-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="218eb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="218eb-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="218eb-132">Response</span></span>
<span data-ttu-id="218eb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="218eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



