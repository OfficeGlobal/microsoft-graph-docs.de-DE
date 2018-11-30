---
title: Aktion „assign“
description: Noch nicht dokumentiert
ms.openlocfilehash: b7d8fe08b041a4486b286ca4690e2f5b6782aa88
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018343"
---
# <a name="assign-action"></a><span data-ttu-id="dee20-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="dee20-103">assign action</span></span>

> <span data-ttu-id="dee20-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dee20-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dee20-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="dee20-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dee20-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dee20-106">Prerequisites</span></span>
<span data-ttu-id="dee20-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dee20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dee20-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dee20-109">Permission type</span></span>|<span data-ttu-id="dee20-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dee20-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dee20-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dee20-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dee20-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dee20-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dee20-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dee20-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dee20-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dee20-114">Not supported.</span></span>|
|<span data-ttu-id="dee20-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dee20-115">Application</span></span>|<span data-ttu-id="dee20-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dee20-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dee20-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dee20-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="dee20-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dee20-118">Request headers</span></span>
|<span data-ttu-id="dee20-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dee20-119">Header</span></span>|<span data-ttu-id="dee20-120">Wert</span><span class="sxs-lookup"><span data-stu-id="dee20-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dee20-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dee20-121">Authorization</span></span>|<span data-ttu-id="dee20-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dee20-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dee20-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dee20-123">Accept</span></span>|<span data-ttu-id="dee20-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dee20-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dee20-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dee20-125">Request body</span></span>
<span data-ttu-id="dee20-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="dee20-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dee20-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="dee20-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dee20-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dee20-128">Property</span></span>|<span data-ttu-id="dee20-129">Typ</span><span class="sxs-lookup"><span data-stu-id="dee20-129">Type</span></span>|<span data-ttu-id="dee20-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dee20-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dee20-131">assignments</span><span class="sxs-lookup"><span data-stu-id="dee20-131">assignments</span></span>|<span data-ttu-id="dee20-132">Collection von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="dee20-132">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="dee20-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="dee20-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dee20-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="dee20-134">Response</span></span>
<span data-ttu-id="dee20-135">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dee20-135">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dee20-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dee20-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="dee20-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dee20-137">Request</span></span>
<span data-ttu-id="dee20-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dee20-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign

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

### <a name="response"></a><span data-ttu-id="dee20-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="dee20-139">Response</span></span>
<span data-ttu-id="dee20-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dee20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



