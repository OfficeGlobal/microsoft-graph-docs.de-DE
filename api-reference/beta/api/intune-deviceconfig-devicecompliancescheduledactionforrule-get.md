---
title: Abrufen von „deviceComplianceScheduledActionForRule“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5dd939cfc14dc1da3089e3d36da5885bdcc3608c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148433"
---
# <a name="get-devicecompliancescheduledactionforrule"></a><span data-ttu-id="af164-103">Abrufen von „deviceComplianceScheduledActionForRule“</span><span class="sxs-lookup"><span data-stu-id="af164-103">Get deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="af164-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="af164-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af164-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="af164-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af164-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="af164-106">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af164-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="af164-107">Prerequisites</span></span>
<span data-ttu-id="af164-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="af164-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="af164-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="af164-110">Permission type</span></span>|<span data-ttu-id="af164-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="af164-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af164-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="af164-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af164-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="af164-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="af164-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="af164-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af164-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af164-115">Not supported.</span></span>|
|<span data-ttu-id="af164-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="af164-116">Application</span></span>|<span data-ttu-id="af164-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af164-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af164-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="af164-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af164-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="af164-119">Optional query parameters</span></span>
<span data-ttu-id="af164-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="af164-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af164-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="af164-121">Request headers</span></span>
|<span data-ttu-id="af164-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="af164-122">Header</span></span>|<span data-ttu-id="af164-123">Wert</span><span class="sxs-lookup"><span data-stu-id="af164-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af164-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="af164-124">Authorization</span></span>|<span data-ttu-id="af164-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="af164-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af164-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="af164-126">Accept</span></span>|<span data-ttu-id="af164-127">application/json</span><span class="sxs-lookup"><span data-stu-id="af164-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af164-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="af164-128">Request body</span></span>
<span data-ttu-id="af164-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="af164-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af164-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="af164-130">Response</span></span>
<span data-ttu-id="af164-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="af164-131">If successful, this method returns a `200 OK` response code and [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af164-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="af164-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="af164-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="af164-133">Request</span></span>
<span data-ttu-id="af164-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="af164-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

### <a name="response"></a><span data-ttu-id="af164-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="af164-135">Response</span></span>
<span data-ttu-id="af164-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="af164-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 188

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
    "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
    "ruleName": "Rule Name value"
  }
}
```




