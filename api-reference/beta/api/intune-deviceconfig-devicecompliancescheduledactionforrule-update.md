---
title: Aktualisieren von „deviceComplianceScheduledActionForRule“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceComplianceScheduledActionForRule.
author: tfitzmac
ms.openlocfilehash: 811029446591b33ac38dad5e4a9aaca045d6e9dc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330842"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="6db5a-103">Aktualisieren von „deviceComplianceScheduledActionForRule“</span><span class="sxs-lookup"><span data-stu-id="6db5a-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="6db5a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6db5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6db5a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6db5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6db5a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6db5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6db5a-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="6db5a-107">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6db5a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6db5a-108">Prerequisites</span></span>
<span data-ttu-id="6db5a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6db5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6db5a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6db5a-111">Permission type</span></span>|<span data-ttu-id="6db5a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6db5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6db5a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6db5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6db5a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6db5a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6db5a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6db5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6db5a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6db5a-116">Not supported.</span></span>|
|<span data-ttu-id="6db5a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6db5a-117">Application</span></span>|<span data-ttu-id="6db5a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6db5a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6db5a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6db5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="6db5a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6db5a-120">Request headers</span></span>
|<span data-ttu-id="6db5a-121">Header</span><span class="sxs-lookup"><span data-stu-id="6db5a-121">Header</span></span>|<span data-ttu-id="6db5a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6db5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6db5a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6db5a-123">Authorization</span></span>|<span data-ttu-id="6db5a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6db5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6db5a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6db5a-125">Accept</span></span>|<span data-ttu-id="6db5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6db5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6db5a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6db5a-127">Request body</span></span>
<span data-ttu-id="6db5a-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) an.</span><span class="sxs-lookup"><span data-stu-id="6db5a-128">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="6db5a-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="6db5a-129">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="6db5a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6db5a-130">Property</span></span>|<span data-ttu-id="6db5a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6db5a-131">Type</span></span>|<span data-ttu-id="6db5a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6db5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6db5a-133">id</span><span class="sxs-lookup"><span data-stu-id="6db5a-133">id</span></span>|<span data-ttu-id="6db5a-134">String</span><span class="sxs-lookup"><span data-stu-id="6db5a-134">String</span></span>|<span data-ttu-id="6db5a-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6db5a-135">Key of the entity.</span></span>|
|<span data-ttu-id="6db5a-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="6db5a-136">ruleName</span></span>|<span data-ttu-id="6db5a-137">String</span><span class="sxs-lookup"><span data-stu-id="6db5a-137">String</span></span>|<span data-ttu-id="6db5a-138">Name der Regel, auf die die geplante Aktion angewendet wird</span><span class="sxs-lookup"><span data-stu-id="6db5a-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="6db5a-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="6db5a-139">Response</span></span>
<span data-ttu-id="6db5a-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6db5a-140">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6db5a-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6db5a-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="6db5a-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6db5a-142">Request</span></span>
<span data-ttu-id="6db5a-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6db5a-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 37

{
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="6db5a-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="6db5a-144">Response</span></span>
<span data-ttu-id="6db5a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6db5a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```





