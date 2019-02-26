---
title: Aktualisieren von „deviceCompliancePolicyDeviceStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCompliancePolicyDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b4d943ea1e4686f7c1b4e6cbf3e3036625ea5f7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260648"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="a78bc-103">Aktualisieren von „deviceCompliancePolicyDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="a78bc-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="a78bc-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a78bc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a78bc-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a78bc-105">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a78bc-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a78bc-106">Prerequisites</span></span>
<span data-ttu-id="a78bc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a78bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a78bc-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a78bc-109">Permission type</span></span>|<span data-ttu-id="a78bc-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a78bc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a78bc-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a78bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a78bc-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a78bc-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a78bc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a78bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a78bc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a78bc-114">Not supported.</span></span>|
|<span data-ttu-id="a78bc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a78bc-115">Application</span></span>|<span data-ttu-id="a78bc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a78bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a78bc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a78bc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="a78bc-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a78bc-118">Request headers</span></span>
|<span data-ttu-id="a78bc-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a78bc-119">Header</span></span>|<span data-ttu-id="a78bc-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a78bc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a78bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a78bc-121">Authorization</span></span>|<span data-ttu-id="a78bc-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a78bc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a78bc-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a78bc-123">Accept</span></span>|<span data-ttu-id="a78bc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a78bc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a78bc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a78bc-125">Request body</span></span>
<span data-ttu-id="a78bc-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="a78bc-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="a78bc-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a78bc-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="a78bc-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a78bc-128">Property</span></span>|<span data-ttu-id="a78bc-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a78bc-129">Type</span></span>|<span data-ttu-id="a78bc-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a78bc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a78bc-131">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="a78bc-131">inGracePeriodCount</span></span>|<span data-ttu-id="a78bc-132">Int32</span><span class="sxs-lookup"><span data-stu-id="a78bc-132">Int32</span></span>|<span data-ttu-id="a78bc-133">Anzahl von Geräten, die sich in der Toleranzperiode befinden</span><span class="sxs-lookup"><span data-stu-id="a78bc-133">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="a78bc-134">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="a78bc-134">configManagerCount</span></span>|<span data-ttu-id="a78bc-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a78bc-135">Int32</span></span>|<span data-ttu-id="a78bc-136">Anzahl von Geräten, deren Konformität mit System Center Configuration Manager verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="a78bc-136">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="a78bc-137">id</span><span class="sxs-lookup"><span data-stu-id="a78bc-137">id</span></span>|<span data-ttu-id="a78bc-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a78bc-138">String</span></span>|<span data-ttu-id="a78bc-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a78bc-139">Key of the entity.</span></span>|
|<span data-ttu-id="a78bc-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a78bc-140">unknownDeviceCount</span></span>|<span data-ttu-id="a78bc-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a78bc-141">Int32</span></span>|<span data-ttu-id="a78bc-142">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="a78bc-142">Number of unknown devices</span></span>|
|<span data-ttu-id="a78bc-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a78bc-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="a78bc-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a78bc-144">Int32</span></span>|<span data-ttu-id="a78bc-145">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="a78bc-145">Number of not applicable devices</span></span>|
|<span data-ttu-id="a78bc-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a78bc-146">compliantDeviceCount</span></span>|<span data-ttu-id="a78bc-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a78bc-147">Int32</span></span>|<span data-ttu-id="a78bc-148">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="a78bc-148">Number of compliant devices</span></span>|
|<span data-ttu-id="a78bc-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a78bc-149">remediatedDeviceCount</span></span>|<span data-ttu-id="a78bc-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a78bc-150">Int32</span></span>|<span data-ttu-id="a78bc-151">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="a78bc-151">Number of remediated devices</span></span>|
|<span data-ttu-id="a78bc-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a78bc-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a78bc-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a78bc-153">Int32</span></span>|<span data-ttu-id="a78bc-154">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="a78bc-154">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="a78bc-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a78bc-155">errorDeviceCount</span></span>|<span data-ttu-id="a78bc-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a78bc-156">Int32</span></span>|<span data-ttu-id="a78bc-157">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="a78bc-157">Number of error devices</span></span>|
|<span data-ttu-id="a78bc-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a78bc-158">conflictDeviceCount</span></span>|<span data-ttu-id="a78bc-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a78bc-159">Int32</span></span>|<span data-ttu-id="a78bc-160">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="a78bc-160">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="a78bc-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="a78bc-161">Response</span></span>
<span data-ttu-id="a78bc-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a78bc-162">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a78bc-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a78bc-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="a78bc-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a78bc-164">Request</span></span>
<span data-ttu-id="a78bc-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a78bc-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 349

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="a78bc-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="a78bc-166">Response</span></span>
<span data-ttu-id="a78bc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a78bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



