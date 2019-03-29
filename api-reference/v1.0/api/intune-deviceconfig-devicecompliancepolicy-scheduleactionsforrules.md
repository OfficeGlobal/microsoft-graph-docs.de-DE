---
title: scheduleActionsForRules-Aktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ced79558b7a106e57468cacd7db2e2bd5ae97bc5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963107"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="04f4f-103">scheduleActionsForRules-Aktion</span><span class="sxs-lookup"><span data-stu-id="04f4f-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="04f4f-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="04f4f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04f4f-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="04f4f-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04f4f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="04f4f-106">Prerequisites</span></span>
<span data-ttu-id="04f4f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04f4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04f4f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04f4f-109">Permission type</span></span>|<span data-ttu-id="04f4f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04f4f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04f4f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04f4f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="04f4f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04f4f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="04f4f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04f4f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04f4f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04f4f-114">Not supported.</span></span>|
|<span data-ttu-id="04f4f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04f4f-115">Application</span></span>|<span data-ttu-id="04f4f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04f4f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04f4f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04f4f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="04f4f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04f4f-118">Request headers</span></span>
|<span data-ttu-id="04f4f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="04f4f-119">Header</span></span>|<span data-ttu-id="04f4f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="04f4f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04f4f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="04f4f-121">Authorization</span></span>|<span data-ttu-id="04f4f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="04f4f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04f4f-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="04f4f-123">Accept</span></span>|<span data-ttu-id="04f4f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="04f4f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04f4f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04f4f-125">Request body</span></span>
<span data-ttu-id="04f4f-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="04f4f-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="04f4f-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="04f4f-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="04f4f-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="04f4f-128">Property</span></span>|<span data-ttu-id="04f4f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="04f4f-129">Type</span></span>|<span data-ttu-id="04f4f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04f4f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04f4f-131">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="04f4f-131">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="04f4f-132">Sammlung von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="04f4f-132">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="04f4f-133">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="04f4f-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="04f4f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="04f4f-134">Response</span></span>
<span data-ttu-id="04f4f-135">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04f4f-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04f4f-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04f4f-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="04f4f-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04f4f-137">Request</span></span>
<span data-ttu-id="04f4f-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04f4f-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04f4f-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="04f4f-139">Response</span></span>
<span data-ttu-id="04f4f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04f4f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



