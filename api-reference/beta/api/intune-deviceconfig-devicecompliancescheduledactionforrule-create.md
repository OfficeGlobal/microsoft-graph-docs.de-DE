---
title: Erstellen von „deviceComplianceScheduledActionForRule“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceScheduledActionForRule.
author: tfitzmac
ms.openlocfilehash: adc4e488d387c5f5087ded96e585a882ee424707
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345829"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="b32d6-103">Erstellen von „deviceComplianceScheduledActionForRule“</span><span class="sxs-lookup"><span data-stu-id="b32d6-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="b32d6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b32d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b32d6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b32d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b32d6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b32d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b32d6-107">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="b32d6-107">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b32d6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b32d6-108">Prerequisites</span></span>
<span data-ttu-id="b32d6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b32d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b32d6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b32d6-111">Permission type</span></span>|<span data-ttu-id="b32d6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b32d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b32d6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b32d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b32d6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b32d6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b32d6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b32d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b32d6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b32d6-116">Not supported.</span></span>|
|<span data-ttu-id="b32d6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b32d6-117">Application</span></span>|<span data-ttu-id="b32d6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b32d6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b32d6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b32d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="b32d6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b32d6-120">Request headers</span></span>
|<span data-ttu-id="b32d6-121">Header</span><span class="sxs-lookup"><span data-stu-id="b32d6-121">Header</span></span>|<span data-ttu-id="b32d6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b32d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b32d6-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b32d6-123">Authorization</span></span>|<span data-ttu-id="b32d6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b32d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b32d6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b32d6-125">Accept</span></span>|<span data-ttu-id="b32d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b32d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b32d6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b32d6-127">Request body</span></span>
<span data-ttu-id="b32d6-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceScheduledActionForRule“ an.</span><span class="sxs-lookup"><span data-stu-id="b32d6-128">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="b32d6-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceScheduledActionForRule“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="b32d6-129">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="b32d6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b32d6-130">Property</span></span>|<span data-ttu-id="b32d6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b32d6-131">Type</span></span>|<span data-ttu-id="b32d6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b32d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b32d6-133">id</span><span class="sxs-lookup"><span data-stu-id="b32d6-133">id</span></span>|<span data-ttu-id="b32d6-134">String</span><span class="sxs-lookup"><span data-stu-id="b32d6-134">String</span></span>|<span data-ttu-id="b32d6-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b32d6-135">Key of the entity.</span></span>|
|<span data-ttu-id="b32d6-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="b32d6-136">ruleName</span></span>|<span data-ttu-id="b32d6-137">String</span><span class="sxs-lookup"><span data-stu-id="b32d6-137">String</span></span>|<span data-ttu-id="b32d6-138">Name der Regel, auf die die geplante Aktion angewendet wird</span><span class="sxs-lookup"><span data-stu-id="b32d6-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="b32d6-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b32d6-139">Response</span></span>
<span data-ttu-id="b32d6-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b32d6-140">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b32d6-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b32d6-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b32d6-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b32d6-142">Request</span></span>
<span data-ttu-id="b32d6-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b32d6-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="b32d6-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b32d6-144">Response</span></span>
<span data-ttu-id="b32d6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b32d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```





