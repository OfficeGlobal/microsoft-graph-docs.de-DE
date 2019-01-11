---
title: Aktualisieren von „deviceComplianceDeviceOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceComplianceDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1bcbcd81d70eb01613d33a9acf44737ae9519583
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882103"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="004f6-103">Aktualisieren von „deviceComplianceDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="004f6-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="004f6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="004f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="004f6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="004f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="004f6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="004f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="004f6-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="004f6-107">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="004f6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="004f6-108">Prerequisites</span></span>
<span data-ttu-id="004f6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="004f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="004f6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="004f6-111">Permission type</span></span>|<span data-ttu-id="004f6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="004f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="004f6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="004f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="004f6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="004f6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="004f6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="004f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="004f6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="004f6-116">Not supported.</span></span>|
|<span data-ttu-id="004f6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="004f6-117">Application</span></span>|<span data-ttu-id="004f6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="004f6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="004f6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="004f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="004f6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="004f6-120">Request headers</span></span>
|<span data-ttu-id="004f6-121">Header</span><span class="sxs-lookup"><span data-stu-id="004f6-121">Header</span></span>|<span data-ttu-id="004f6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="004f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="004f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="004f6-123">Authorization</span></span>|<span data-ttu-id="004f6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="004f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="004f6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="004f6-125">Accept</span></span>|<span data-ttu-id="004f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="004f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="004f6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="004f6-127">Request body</span></span>
<span data-ttu-id="004f6-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="004f6-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="004f6-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="004f6-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="004f6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="004f6-130">Property</span></span>|<span data-ttu-id="004f6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="004f6-131">Type</span></span>|<span data-ttu-id="004f6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="004f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="004f6-133">id</span><span class="sxs-lookup"><span data-stu-id="004f6-133">id</span></span>|<span data-ttu-id="004f6-134">String</span><span class="sxs-lookup"><span data-stu-id="004f6-134">String</span></span>|<span data-ttu-id="004f6-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="004f6-135">Key of the entity.</span></span>|
|<span data-ttu-id="004f6-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="004f6-136">pendingCount</span></span>|<span data-ttu-id="004f6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="004f6-137">Int32</span></span>|<span data-ttu-id="004f6-138">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="004f6-138">Number of pending devices</span></span>|
|<span data-ttu-id="004f6-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="004f6-139">notApplicableCount</span></span>|<span data-ttu-id="004f6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="004f6-140">Int32</span></span>|<span data-ttu-id="004f6-141">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="004f6-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="004f6-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="004f6-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="004f6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="004f6-143">Int32</span></span>|<span data-ttu-id="004f6-144">Anzahl der Geräte, die aufgrund von Konflikt Plattform und Richtlinie nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="004f6-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="004f6-145">successCount</span><span class="sxs-lookup"><span data-stu-id="004f6-145">successCount</span></span>|<span data-ttu-id="004f6-146">Int32</span><span class="sxs-lookup"><span data-stu-id="004f6-146">Int32</span></span>|<span data-ttu-id="004f6-147">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="004f6-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="004f6-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="004f6-148">errorCount</span></span>|<span data-ttu-id="004f6-149">Int32</span><span class="sxs-lookup"><span data-stu-id="004f6-149">Int32</span></span>|<span data-ttu-id="004f6-150">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="004f6-150">Number of error devices</span></span>|
|<span data-ttu-id="004f6-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="004f6-151">failedCount</span></span>|<span data-ttu-id="004f6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="004f6-152">Int32</span></span>|<span data-ttu-id="004f6-153">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="004f6-153">Number of failed devices</span></span>|
|<span data-ttu-id="004f6-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="004f6-154">conflictCount</span></span>|<span data-ttu-id="004f6-155">Int32</span><span class="sxs-lookup"><span data-stu-id="004f6-155">Int32</span></span>|<span data-ttu-id="004f6-156">Anzahl der Geräte in Konflikt</span><span class="sxs-lookup"><span data-stu-id="004f6-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="004f6-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="004f6-157">lastUpdateDateTime</span></span>|<span data-ttu-id="004f6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="004f6-158">DateTimeOffset</span></span>|<span data-ttu-id="004f6-159">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="004f6-159">Last update time</span></span>|
|<span data-ttu-id="004f6-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="004f6-160">configurationVersion</span></span>|<span data-ttu-id="004f6-161">Int32</span><span class="sxs-lookup"><span data-stu-id="004f6-161">Int32</span></span>|<span data-ttu-id="004f6-162">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="004f6-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="004f6-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="004f6-163">Response</span></span>
<span data-ttu-id="004f6-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="004f6-164">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="004f6-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="004f6-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="004f6-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="004f6-166">Request</span></span>
<span data-ttu-id="004f6-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="004f6-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 273

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="004f6-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="004f6-168">Response</span></span>
<span data-ttu-id="004f6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="004f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





