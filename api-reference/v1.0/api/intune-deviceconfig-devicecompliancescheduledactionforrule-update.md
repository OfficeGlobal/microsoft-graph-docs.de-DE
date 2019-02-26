---
title: Aktualisieren von „deviceComplianceScheduledActionForRule“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: adfd70118ba57210b5ac743e6b664b2fe276f98d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257015"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="94205-103">Aktualisieren von „deviceComplianceScheduledActionForRule“</span><span class="sxs-lookup"><span data-stu-id="94205-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="94205-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="94205-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94205-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="94205-105">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94205-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="94205-106">Prerequisites</span></span>
<span data-ttu-id="94205-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="94205-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="94205-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="94205-109">Permission type</span></span>|<span data-ttu-id="94205-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="94205-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94205-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="94205-111">Delegated (work or school account)</span></span>|<span data-ttu-id="94205-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94205-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="94205-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="94205-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94205-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94205-114">Not supported.</span></span>|
|<span data-ttu-id="94205-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="94205-115">Application</span></span>|<span data-ttu-id="94205-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94205-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94205-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="94205-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="94205-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="94205-118">Request headers</span></span>
|<span data-ttu-id="94205-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="94205-119">Header</span></span>|<span data-ttu-id="94205-120">Wert</span><span class="sxs-lookup"><span data-stu-id="94205-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94205-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="94205-121">Authorization</span></span>|<span data-ttu-id="94205-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="94205-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94205-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="94205-123">Accept</span></span>|<span data-ttu-id="94205-124">application/json</span><span class="sxs-lookup"><span data-stu-id="94205-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94205-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="94205-125">Request body</span></span>
<span data-ttu-id="94205-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) an.</span><span class="sxs-lookup"><span data-stu-id="94205-126">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="94205-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="94205-127">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="94205-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="94205-128">Property</span></span>|<span data-ttu-id="94205-129">Typ</span><span class="sxs-lookup"><span data-stu-id="94205-129">Type</span></span>|<span data-ttu-id="94205-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94205-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94205-131">id</span><span class="sxs-lookup"><span data-stu-id="94205-131">id</span></span>|<span data-ttu-id="94205-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="94205-132">String</span></span>|<span data-ttu-id="94205-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="94205-133">Key of the entity.</span></span>|
|<span data-ttu-id="94205-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="94205-134">ruleName</span></span>|<span data-ttu-id="94205-135">String</span><span class="sxs-lookup"><span data-stu-id="94205-135">String</span></span>|<span data-ttu-id="94205-136">Name der Regel, auf die die geplante Aktion angewendet wird</span><span class="sxs-lookup"><span data-stu-id="94205-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="94205-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="94205-137">Response</span></span>
<span data-ttu-id="94205-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="94205-138">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94205-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="94205-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="94205-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="94205-140">Request</span></span>
<span data-ttu-id="94205-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="94205-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="94205-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="94205-142">Response</span></span>
<span data-ttu-id="94205-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94205-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



