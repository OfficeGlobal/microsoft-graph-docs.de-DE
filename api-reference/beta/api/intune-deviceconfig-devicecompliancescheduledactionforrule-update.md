---
title: Aktualisieren von „deviceComplianceScheduledActionForRule“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceComplianceScheduledActionForRule.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d2ae868b5c11220423c4f1ee496c77f8cd0482c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414641"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="2e639-103">Aktualisieren von „deviceComplianceScheduledActionForRule“</span><span class="sxs-lookup"><span data-stu-id="2e639-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="2e639-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2e639-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2e639-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2e639-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e639-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2e639-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e639-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="2e639-107">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e639-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2e639-108">Prerequisites</span></span>
<span data-ttu-id="2e639-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e639-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2e639-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e639-111">Permission type</span></span>|<span data-ttu-id="2e639-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e639-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e639-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e639-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e639-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e639-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2e639-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e639-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e639-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e639-116">Not supported.</span></span>|
|<span data-ttu-id="2e639-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e639-117">Application</span></span>|<span data-ttu-id="2e639-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e639-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e639-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e639-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="2e639-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e639-120">Request headers</span></span>
|<span data-ttu-id="2e639-121">Header</span><span class="sxs-lookup"><span data-stu-id="2e639-121">Header</span></span>|<span data-ttu-id="2e639-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2e639-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e639-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2e639-123">Authorization</span></span>|<span data-ttu-id="2e639-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2e639-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e639-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2e639-125">Accept</span></span>|<span data-ttu-id="2e639-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e639-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e639-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e639-127">Request body</span></span>
<span data-ttu-id="2e639-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) an.</span><span class="sxs-lookup"><span data-stu-id="2e639-128">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="2e639-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2e639-129">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="2e639-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e639-130">Property</span></span>|<span data-ttu-id="2e639-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2e639-131">Type</span></span>|<span data-ttu-id="2e639-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e639-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e639-133">id</span><span class="sxs-lookup"><span data-stu-id="2e639-133">id</span></span>|<span data-ttu-id="2e639-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2e639-134">String</span></span>|<span data-ttu-id="2e639-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2e639-135">Key of the entity.</span></span>|
|<span data-ttu-id="2e639-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="2e639-136">ruleName</span></span>|<span data-ttu-id="2e639-137">String</span><span class="sxs-lookup"><span data-stu-id="2e639-137">String</span></span>|<span data-ttu-id="2e639-138">Name der Regel, auf die die geplante Aktion angewendet wird</span><span class="sxs-lookup"><span data-stu-id="2e639-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="2e639-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e639-139">Response</span></span>
<span data-ttu-id="2e639-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2e639-140">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e639-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e639-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e639-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e639-142">Request</span></span>
<span data-ttu-id="2e639-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e639-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="2e639-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e639-144">Response</span></span>
<span data-ttu-id="2e639-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e639-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




