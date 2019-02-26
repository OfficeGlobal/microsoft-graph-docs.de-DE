---
title: scheduleActionsForRules-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0f4c8d6334d7b4a6634884d892207101c5c1daa
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255311"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="3260b-103">scheduleActionsForRules-Aktion</span><span class="sxs-lookup"><span data-stu-id="3260b-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="3260b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3260b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3260b-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3260b-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3260b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3260b-106">Prerequisites</span></span>
<span data-ttu-id="3260b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3260b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3260b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3260b-109">Permission type</span></span>|<span data-ttu-id="3260b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3260b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3260b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3260b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3260b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3260b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3260b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3260b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3260b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3260b-114">Not supported.</span></span>|
|<span data-ttu-id="3260b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3260b-115">Application</span></span>|<span data-ttu-id="3260b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3260b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3260b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3260b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="3260b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3260b-118">Request headers</span></span>
|<span data-ttu-id="3260b-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3260b-119">Header</span></span>|<span data-ttu-id="3260b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3260b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3260b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3260b-121">Authorization</span></span>|<span data-ttu-id="3260b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3260b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3260b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3260b-123">Accept</span></span>|<span data-ttu-id="3260b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3260b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3260b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3260b-125">Request body</span></span>
<span data-ttu-id="3260b-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="3260b-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3260b-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="3260b-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3260b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3260b-128">Property</span></span>|<span data-ttu-id="3260b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3260b-129">Type</span></span>|<span data-ttu-id="3260b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3260b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3260b-131">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="3260b-131">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="3260b-132">Sammlung von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="3260b-132">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="3260b-133">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="3260b-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3260b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3260b-134">Response</span></span>
<span data-ttu-id="3260b-135">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="3260b-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3260b-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3260b-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="3260b-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3260b-137">Request</span></span>
<span data-ttu-id="3260b-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3260b-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3260b-139">Reaktion</span><span class="sxs-lookup"><span data-stu-id="3260b-139">Response</span></span>
<span data-ttu-id="3260b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3260b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



