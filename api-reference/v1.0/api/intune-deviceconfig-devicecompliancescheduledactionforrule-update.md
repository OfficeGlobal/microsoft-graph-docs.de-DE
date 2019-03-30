---
title: Aktualisieren von „deviceComplianceScheduledActionForRule“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37b53af2128e340450b0bdf5799250660c5ab0a3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988875"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="a3ef3-103">Aktualisieren von „deviceComplianceScheduledActionForRule“</span><span class="sxs-lookup"><span data-stu-id="a3ef3-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="a3ef3-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a3ef3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3ef3-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="a3ef3-105">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3ef3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a3ef3-106">Prerequisites</span></span>
<span data-ttu-id="a3ef3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3ef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3ef3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a3ef3-109">Permission type</span></span>|<span data-ttu-id="a3ef3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a3ef3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3ef3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a3ef3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3ef3-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3ef3-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3ef3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a3ef3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3ef3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3ef3-114">Not supported.</span></span>|
|<span data-ttu-id="a3ef3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a3ef3-115">Application</span></span>|<span data-ttu-id="a3ef3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3ef3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3ef3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3ef3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="a3ef3-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a3ef3-118">Request headers</span></span>
|<span data-ttu-id="a3ef3-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a3ef3-119">Header</span></span>|<span data-ttu-id="a3ef3-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a3ef3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3ef3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3ef3-121">Authorization</span></span>|<span data-ttu-id="a3ef3-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a3ef3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3ef3-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a3ef3-123">Accept</span></span>|<span data-ttu-id="a3ef3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a3ef3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3ef3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a3ef3-125">Request body</span></span>
<span data-ttu-id="a3ef3-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) an.</span><span class="sxs-lookup"><span data-stu-id="a3ef3-126">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="a3ef3-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a3ef3-127">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="a3ef3-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a3ef3-128">Property</span></span>|<span data-ttu-id="a3ef3-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a3ef3-129">Type</span></span>|<span data-ttu-id="a3ef3-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3ef3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3ef3-131">id</span><span class="sxs-lookup"><span data-stu-id="a3ef3-131">id</span></span>|<span data-ttu-id="a3ef3-132">String</span><span class="sxs-lookup"><span data-stu-id="a3ef3-132">String</span></span>|<span data-ttu-id="a3ef3-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a3ef3-133">Key of the entity.</span></span>|
|<span data-ttu-id="a3ef3-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="a3ef3-134">ruleName</span></span>|<span data-ttu-id="a3ef3-135">String</span><span class="sxs-lookup"><span data-stu-id="a3ef3-135">String</span></span>|<span data-ttu-id="a3ef3-136">Name der Regel, auf die die geplante Aktion angewendet wird</span><span class="sxs-lookup"><span data-stu-id="a3ef3-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="a3ef3-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3ef3-137">Response</span></span>
<span data-ttu-id="a3ef3-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a3ef3-138">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3ef3-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a3ef3-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3ef3-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3ef3-140">Request</span></span>
<span data-ttu-id="a3ef3-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a3ef3-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="a3ef3-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3ef3-142">Response</span></span>
<span data-ttu-id="a3ef3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3ef3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



