---
title: Aktion „assign“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 05ed52b22b6c4709499f5736ab911a565605bcbb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929172"
---
# <a name="assign-action"></a><span data-ttu-id="849e7-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="849e7-103">assign action</span></span>

> <span data-ttu-id="849e7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="849e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="849e7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="849e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="849e7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="849e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="849e7-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="849e7-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="849e7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="849e7-108">Prerequisites</span></span>
<span data-ttu-id="849e7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="849e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="849e7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="849e7-111">Permission type</span></span>|<span data-ttu-id="849e7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="849e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="849e7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="849e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="849e7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="849e7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="849e7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="849e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="849e7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="849e7-116">Not supported.</span></span>|
|<span data-ttu-id="849e7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="849e7-117">Application</span></span>|<span data-ttu-id="849e7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="849e7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="849e7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="849e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="849e7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="849e7-120">Request headers</span></span>
|<span data-ttu-id="849e7-121">Header</span><span class="sxs-lookup"><span data-stu-id="849e7-121">Header</span></span>|<span data-ttu-id="849e7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="849e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="849e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="849e7-123">Authorization</span></span>|<span data-ttu-id="849e7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="849e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="849e7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="849e7-125">Accept</span></span>|<span data-ttu-id="849e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="849e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="849e7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="849e7-127">Request body</span></span>
<span data-ttu-id="849e7-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="849e7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="849e7-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="849e7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="849e7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="849e7-130">Property</span></span>|<span data-ttu-id="849e7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="849e7-131">Type</span></span>|<span data-ttu-id="849e7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="849e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="849e7-133">assignments</span><span class="sxs-lookup"><span data-stu-id="849e7-133">assignments</span></span>|<span data-ttu-id="849e7-134">Collection von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="849e7-134">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="849e7-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="849e7-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="849e7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="849e7-136">Response</span></span>
<span data-ttu-id="849e7-137">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="849e7-137">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="849e7-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="849e7-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="849e7-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="849e7-139">Request</span></span>
<span data-ttu-id="849e7-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="849e7-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="849e7-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="849e7-141">Response</span></span>
<span data-ttu-id="849e7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="849e7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





