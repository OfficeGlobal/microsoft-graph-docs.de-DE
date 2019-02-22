---
title: Erstellen von „deviceComplianceScheduledActionForRule“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 40a72428b64f5d99d12cf16175dc4765d7664008
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140355"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="08728-103">Erstellen von „deviceComplianceScheduledActionForRule“</span><span class="sxs-lookup"><span data-stu-id="08728-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="08728-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08728-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08728-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="08728-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08728-106">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="08728-106">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08728-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="08728-107">Prerequisites</span></span>
<span data-ttu-id="08728-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="08728-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="08728-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="08728-110">Permission type</span></span>|<span data-ttu-id="08728-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="08728-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08728-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="08728-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08728-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08728-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08728-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="08728-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08728-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08728-115">Not supported.</span></span>|
|<span data-ttu-id="08728-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="08728-116">Application</span></span>|<span data-ttu-id="08728-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08728-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08728-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08728-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="08728-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="08728-119">Request headers</span></span>
|<span data-ttu-id="08728-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="08728-120">Header</span></span>|<span data-ttu-id="08728-121">Wert</span><span class="sxs-lookup"><span data-stu-id="08728-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08728-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08728-122">Authorization</span></span>|<span data-ttu-id="08728-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="08728-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08728-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="08728-124">Accept</span></span>|<span data-ttu-id="08728-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08728-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08728-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="08728-126">Request body</span></span>
<span data-ttu-id="08728-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceScheduledActionForRule“ an.</span><span class="sxs-lookup"><span data-stu-id="08728-127">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="08728-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceScheduledActionForRule“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="08728-128">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="08728-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08728-129">Property</span></span>|<span data-ttu-id="08728-130">Typ</span><span class="sxs-lookup"><span data-stu-id="08728-130">Type</span></span>|<span data-ttu-id="08728-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08728-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08728-132">id</span><span class="sxs-lookup"><span data-stu-id="08728-132">id</span></span>|<span data-ttu-id="08728-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08728-133">String</span></span>|<span data-ttu-id="08728-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="08728-134">Key of the entity.</span></span>|
|<span data-ttu-id="08728-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="08728-135">ruleName</span></span>|<span data-ttu-id="08728-136">String</span><span class="sxs-lookup"><span data-stu-id="08728-136">String</span></span>|<span data-ttu-id="08728-137">Name der Regel, auf die die geplante Aktion angewendet wird</span><span class="sxs-lookup"><span data-stu-id="08728-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="08728-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="08728-138">Response</span></span>
<span data-ttu-id="08728-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="08728-139">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08728-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="08728-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="08728-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08728-141">Request</span></span>
<span data-ttu-id="08728-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="08728-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="08728-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="08728-143">Response</span></span>
<span data-ttu-id="08728-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08728-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




