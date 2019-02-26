---
title: Erstellen von „deviceComplianceScheduledActionForRule“
description: Diese Methode erstellt ein neues Objekt des Typs deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89309a44a0246d74064942bb340140f1c5923ca0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264127"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="fe0f7-103">Erstellen von „deviceComplianceScheduledActionForRule“</span><span class="sxs-lookup"><span data-stu-id="fe0f7-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="fe0f7-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fe0f7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe0f7-105">Diese Methode erstellt ein neues Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="fe0f7-105">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe0f7-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fe0f7-106">Prerequisites</span></span>
<span data-ttu-id="fe0f7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe0f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fe0f7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fe0f7-109">Permission type</span></span>|<span data-ttu-id="fe0f7-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fe0f7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe0f7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fe0f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fe0f7-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe0f7-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe0f7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fe0f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe0f7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe0f7-114">Not supported.</span></span>|
|<span data-ttu-id="fe0f7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fe0f7-115">Application</span></span>|<span data-ttu-id="fe0f7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe0f7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe0f7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe0f7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="fe0f7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fe0f7-118">Request headers</span></span>
|<span data-ttu-id="fe0f7-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fe0f7-119">Header</span></span>|<span data-ttu-id="fe0f7-120">Wert</span><span class="sxs-lookup"><span data-stu-id="fe0f7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe0f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe0f7-121">Authorization</span></span>|<span data-ttu-id="fe0f7-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fe0f7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe0f7-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fe0f7-123">Accept</span></span>|<span data-ttu-id="fe0f7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fe0f7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe0f7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fe0f7-125">Request body</span></span>
<span data-ttu-id="fe0f7-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceComplianceScheduledActionForRule“ an.</span><span class="sxs-lookup"><span data-stu-id="fe0f7-126">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="fe0f7-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceComplianceScheduledActionForRule“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="fe0f7-127">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="fe0f7-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fe0f7-128">Property</span></span>|<span data-ttu-id="fe0f7-129">Typ</span><span class="sxs-lookup"><span data-stu-id="fe0f7-129">Type</span></span>|<span data-ttu-id="fe0f7-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe0f7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe0f7-131">id</span><span class="sxs-lookup"><span data-stu-id="fe0f7-131">id</span></span>|<span data-ttu-id="fe0f7-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fe0f7-132">String</span></span>|<span data-ttu-id="fe0f7-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fe0f7-133">Key of the entity.</span></span>|
|<span data-ttu-id="fe0f7-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="fe0f7-134">ruleName</span></span>|<span data-ttu-id="fe0f7-135">String</span><span class="sxs-lookup"><span data-stu-id="fe0f7-135">String</span></span>|<span data-ttu-id="fe0f7-136">Name der Regel, auf die die geplante Aktion angewendet wird</span><span class="sxs-lookup"><span data-stu-id="fe0f7-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="fe0f7-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe0f7-137">Response</span></span>
<span data-ttu-id="fe0f7-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fe0f7-138">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe0f7-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fe0f7-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe0f7-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe0f7-140">Request</span></span>
<span data-ttu-id="fe0f7-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fe0f7-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="fe0f7-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe0f7-142">Response</span></span>
<span data-ttu-id="fe0f7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe0f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



