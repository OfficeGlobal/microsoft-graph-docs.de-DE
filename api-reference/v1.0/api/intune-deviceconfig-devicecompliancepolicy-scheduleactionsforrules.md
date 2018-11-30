---
title: scheduleActionsForRules-Aktion
description: Noch nicht dokumentiert
ms.openlocfilehash: 7df79c4428834cda8a739a9afb1919282c9e1dbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019401"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="4b1a2-103">scheduleActionsForRules-Aktion</span><span class="sxs-lookup"><span data-stu-id="4b1a2-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="4b1a2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4b1a2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b1a2-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4b1a2-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b1a2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4b1a2-106">Prerequisites</span></span>
<span data-ttu-id="4b1a2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b1a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b1a2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b1a2-109">Permission type</span></span>|<span data-ttu-id="4b1a2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b1a2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b1a2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b1a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4b1a2-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b1a2-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b1a2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b1a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b1a2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b1a2-114">Not supported.</span></span>|
|<span data-ttu-id="4b1a2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b1a2-115">Application</span></span>|<span data-ttu-id="4b1a2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b1a2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b1a2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b1a2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="4b1a2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b1a2-118">Request headers</span></span>
|<span data-ttu-id="4b1a2-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4b1a2-119">Header</span></span>|<span data-ttu-id="4b1a2-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4b1a2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b1a2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b1a2-121">Authorization</span></span>|<span data-ttu-id="4b1a2-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4b1a2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b1a2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4b1a2-123">Accept</span></span>|<span data-ttu-id="4b1a2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4b1a2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b1a2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b1a2-125">Request body</span></span>
<span data-ttu-id="4b1a2-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="4b1a2-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4b1a2-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="4b1a2-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4b1a2-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b1a2-128">Property</span></span>|<span data-ttu-id="4b1a2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4b1a2-129">Type</span></span>|<span data-ttu-id="4b1a2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b1a2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b1a2-131">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="4b1a2-131">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="4b1a2-132">Sammlung von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="4b1a2-132">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="4b1a2-133">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="4b1a2-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4b1a2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b1a2-134">Response</span></span>
<span data-ttu-id="4b1a2-135">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="4b1a2-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4b1a2-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b1a2-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b1a2-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b1a2-137">Request</span></span>
<span data-ttu-id="4b1a2-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b1a2-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules

Content-type: application/json
Content-length: 242

{
  "deviceComplianceScheduledActionForRules": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
      "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
      "ruleName": "Rule Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4b1a2-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b1a2-139">Response</span></span>
<span data-ttu-id="4b1a2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b1a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



