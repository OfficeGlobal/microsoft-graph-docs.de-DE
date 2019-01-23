---
title: Auflisten von „deviceCompliancePolicyAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceCompliancePolicyAssignment auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 93b976a73ab7878c3e4198a90ef14392e2d486dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422138"
---
# <a name="list-devicecompliancepolicyassignments"></a><span data-ttu-id="40290-103">Auflisten von „deviceCompliancePolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="40290-103">List deviceCompliancePolicyAssignments</span></span>

> <span data-ttu-id="40290-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="40290-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="40290-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40290-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40290-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="40290-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40290-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="40290-107">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40290-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="40290-108">Prerequisites</span></span>
<span data-ttu-id="40290-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="40290-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="40290-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40290-111">Permission type</span></span>|<span data-ttu-id="40290-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40290-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40290-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40290-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40290-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="40290-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="40290-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40290-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40290-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40290-116">Not supported.</span></span>|
|<span data-ttu-id="40290-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40290-117">Application</span></span>|<span data-ttu-id="40290-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40290-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40290-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40290-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="40290-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40290-120">Request headers</span></span>
|<span data-ttu-id="40290-121">Header</span><span class="sxs-lookup"><span data-stu-id="40290-121">Header</span></span>|<span data-ttu-id="40290-122">Wert</span><span class="sxs-lookup"><span data-stu-id="40290-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40290-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="40290-123">Authorization</span></span>|<span data-ttu-id="40290-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="40290-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40290-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="40290-125">Accept</span></span>|<span data-ttu-id="40290-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40290-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40290-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40290-127">Request body</span></span>
<span data-ttu-id="40290-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="40290-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40290-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="40290-129">Response</span></span>
<span data-ttu-id="40290-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="40290-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40290-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40290-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="40290-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40290-132">Request</span></span>
<span data-ttu-id="40290-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40290-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="40290-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="40290-134">Response</span></span>
<span data-ttu-id="40290-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40290-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




