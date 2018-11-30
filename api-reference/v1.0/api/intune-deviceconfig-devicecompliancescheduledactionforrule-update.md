---
title: Aktualisieren von „deviceComplianceScheduledActionForRule“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceComplianceScheduledActionForRule.
ms.openlocfilehash: d4b6df2d36bfe1852c32e146bb1a553166620a39
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017495"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="88aa5-103">Aktualisieren von „deviceComplianceScheduledActionForRule“</span><span class="sxs-lookup"><span data-stu-id="88aa5-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="88aa5-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="88aa5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88aa5-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="88aa5-105">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88aa5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="88aa5-106">Prerequisites</span></span>
<span data-ttu-id="88aa5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88aa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88aa5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="88aa5-109">Permission type</span></span>|<span data-ttu-id="88aa5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="88aa5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88aa5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="88aa5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88aa5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88aa5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88aa5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="88aa5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88aa5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88aa5-114">Not supported.</span></span>|
|<span data-ttu-id="88aa5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="88aa5-115">Application</span></span>|<span data-ttu-id="88aa5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88aa5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88aa5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="88aa5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="88aa5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="88aa5-118">Request headers</span></span>
|<span data-ttu-id="88aa5-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="88aa5-119">Header</span></span>|<span data-ttu-id="88aa5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="88aa5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88aa5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="88aa5-121">Authorization</span></span>|<span data-ttu-id="88aa5-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="88aa5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88aa5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="88aa5-123">Accept</span></span>|<span data-ttu-id="88aa5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="88aa5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88aa5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="88aa5-125">Request body</span></span>
<span data-ttu-id="88aa5-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) an.</span><span class="sxs-lookup"><span data-stu-id="88aa5-126">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="88aa5-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="88aa5-127">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="88aa5-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88aa5-128">Property</span></span>|<span data-ttu-id="88aa5-129">Typ</span><span class="sxs-lookup"><span data-stu-id="88aa5-129">Type</span></span>|<span data-ttu-id="88aa5-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88aa5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88aa5-131">id</span><span class="sxs-lookup"><span data-stu-id="88aa5-131">id</span></span>|<span data-ttu-id="88aa5-132">String</span><span class="sxs-lookup"><span data-stu-id="88aa5-132">String</span></span>|<span data-ttu-id="88aa5-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="88aa5-133">Key of the entity.</span></span>|
|<span data-ttu-id="88aa5-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="88aa5-134">ruleName</span></span>|<span data-ttu-id="88aa5-135">String</span><span class="sxs-lookup"><span data-stu-id="88aa5-135">String</span></span>|<span data-ttu-id="88aa5-136">Name der Regel, auf die die geplante Aktion angewendet wird</span><span class="sxs-lookup"><span data-stu-id="88aa5-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="88aa5-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="88aa5-137">Response</span></span>
<span data-ttu-id="88aa5-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="88aa5-138">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88aa5-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="88aa5-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="88aa5-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="88aa5-140">Request</span></span>
<span data-ttu-id="88aa5-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="88aa5-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="88aa5-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="88aa5-142">Response</span></span>
<span data-ttu-id="88aa5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="88aa5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



