---
title: Erstellen von „deviceComplianceScheduledActionForRule“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fac03ca9bf037a92bdc36cbadbf1ac7da437e849
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941758"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="8c767-103">Erstellen von „deviceComplianceScheduledActionForRule“</span><span class="sxs-lookup"><span data-stu-id="8c767-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="8c767-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8c767-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c767-105">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="8c767-105">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c767-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8c767-106">Prerequisites</span></span>
<span data-ttu-id="8c767-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c767-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c767-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c767-109">Permission type</span></span>|<span data-ttu-id="8c767-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c767-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c767-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c767-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c767-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c767-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c767-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c767-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c767-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c767-114">Not supported.</span></span>|
|<span data-ttu-id="8c767-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c767-115">Application</span></span>|<span data-ttu-id="8c767-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c767-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c767-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c767-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="8c767-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c767-118">Request headers</span></span>
|<span data-ttu-id="8c767-119">Header</span><span class="sxs-lookup"><span data-stu-id="8c767-119">Header</span></span>|<span data-ttu-id="8c767-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8c767-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c767-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c767-121">Authorization</span></span>|<span data-ttu-id="8c767-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8c767-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c767-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8c767-123">Accept</span></span>|<span data-ttu-id="8c767-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8c767-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c767-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c767-125">Request body</span></span>
<span data-ttu-id="8c767-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceScheduledActionForRule“ an.</span><span class="sxs-lookup"><span data-stu-id="8c767-126">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="8c767-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceScheduledActionForRule“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="8c767-127">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="8c767-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8c767-128">Property</span></span>|<span data-ttu-id="8c767-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8c767-129">Type</span></span>|<span data-ttu-id="8c767-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c767-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c767-131">id</span><span class="sxs-lookup"><span data-stu-id="8c767-131">id</span></span>|<span data-ttu-id="8c767-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8c767-132">String</span></span>|<span data-ttu-id="8c767-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8c767-133">Key of the entity.</span></span>|
|<span data-ttu-id="8c767-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="8c767-134">ruleName</span></span>|<span data-ttu-id="8c767-135">String</span><span class="sxs-lookup"><span data-stu-id="8c767-135">String</span></span>|<span data-ttu-id="8c767-136">Name der Regel, auf die die geplante Aktion angewendet wird</span><span class="sxs-lookup"><span data-stu-id="8c767-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="8c767-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c767-137">Response</span></span>
<span data-ttu-id="8c767-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8c767-138">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c767-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c767-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c767-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c767-140">Request</span></span>
<span data-ttu-id="8c767-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c767-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="8c767-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c767-142">Response</span></span>
<span data-ttu-id="8c767-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c767-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



