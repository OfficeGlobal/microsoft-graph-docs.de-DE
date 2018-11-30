---
title: Aktualisieren von „deviceCompliancePolicyDeviceStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCompliancePolicyDeviceStateSummary.
ms.openlocfilehash: 0cf0fe68f87bfe92536a5e13684818dabad1b2bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017773"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="588a4-103">Aktualisieren von „deviceCompliancePolicyDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="588a4-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="588a4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="588a4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="588a4-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="588a4-105">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="588a4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="588a4-106">Prerequisites</span></span>
<span data-ttu-id="588a4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="588a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="588a4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="588a4-109">Permission type</span></span>|<span data-ttu-id="588a4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="588a4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="588a4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="588a4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="588a4-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="588a4-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="588a4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="588a4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="588a4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="588a4-114">Not supported.</span></span>|
|<span data-ttu-id="588a4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="588a4-115">Application</span></span>|<span data-ttu-id="588a4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="588a4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="588a4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="588a4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="588a4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="588a4-118">Request headers</span></span>
|<span data-ttu-id="588a4-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="588a4-119">Header</span></span>|<span data-ttu-id="588a4-120">Wert</span><span class="sxs-lookup"><span data-stu-id="588a4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="588a4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="588a4-121">Authorization</span></span>|<span data-ttu-id="588a4-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="588a4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="588a4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="588a4-123">Accept</span></span>|<span data-ttu-id="588a4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="588a4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="588a4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="588a4-125">Request body</span></span>
<span data-ttu-id="588a4-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="588a4-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="588a4-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="588a4-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="588a4-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="588a4-128">Property</span></span>|<span data-ttu-id="588a4-129">Typ</span><span class="sxs-lookup"><span data-stu-id="588a4-129">Type</span></span>|<span data-ttu-id="588a4-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="588a4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="588a4-131">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="588a4-131">inGracePeriodCount</span></span>|<span data-ttu-id="588a4-132">Int32</span><span class="sxs-lookup"><span data-stu-id="588a4-132">Int32</span></span>|<span data-ttu-id="588a4-133">Anzahl von Geräten, die sich in der Toleranzperiode befinden</span><span class="sxs-lookup"><span data-stu-id="588a4-133">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="588a4-134">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="588a4-134">configManagerCount</span></span>|<span data-ttu-id="588a4-135">Int32</span><span class="sxs-lookup"><span data-stu-id="588a4-135">Int32</span></span>|<span data-ttu-id="588a4-136">Anzahl von Geräten, deren Konformität mit System Center Configuration Manager verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="588a4-136">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="588a4-137">id</span><span class="sxs-lookup"><span data-stu-id="588a4-137">id</span></span>|<span data-ttu-id="588a4-138">String</span><span class="sxs-lookup"><span data-stu-id="588a4-138">String</span></span>|<span data-ttu-id="588a4-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="588a4-139">Key of the entity.</span></span>|
|<span data-ttu-id="588a4-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="588a4-140">unknownDeviceCount</span></span>|<span data-ttu-id="588a4-141">Int32</span><span class="sxs-lookup"><span data-stu-id="588a4-141">Int32</span></span>|<span data-ttu-id="588a4-142">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="588a4-142">Number of unknown devices</span></span>|
|<span data-ttu-id="588a4-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="588a4-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="588a4-144">Int32</span><span class="sxs-lookup"><span data-stu-id="588a4-144">Int32</span></span>|<span data-ttu-id="588a4-145">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="588a4-145">Number of not applicable devices</span></span>|
|<span data-ttu-id="588a4-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="588a4-146">compliantDeviceCount</span></span>|<span data-ttu-id="588a4-147">Int32</span><span class="sxs-lookup"><span data-stu-id="588a4-147">Int32</span></span>|<span data-ttu-id="588a4-148">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="588a4-148">Number of compliant devices</span></span>|
|<span data-ttu-id="588a4-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="588a4-149">remediatedDeviceCount</span></span>|<span data-ttu-id="588a4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="588a4-150">Int32</span></span>|<span data-ttu-id="588a4-151">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="588a4-151">Number of remediated devices</span></span>|
|<span data-ttu-id="588a4-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="588a4-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="588a4-153">Int32</span><span class="sxs-lookup"><span data-stu-id="588a4-153">Int32</span></span>|<span data-ttu-id="588a4-154">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="588a4-154">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="588a4-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="588a4-155">errorDeviceCount</span></span>|<span data-ttu-id="588a4-156">Int32</span><span class="sxs-lookup"><span data-stu-id="588a4-156">Int32</span></span>|<span data-ttu-id="588a4-157">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="588a4-157">Number of error devices</span></span>|
|<span data-ttu-id="588a4-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="588a4-158">conflictDeviceCount</span></span>|<span data-ttu-id="588a4-159">Int32</span><span class="sxs-lookup"><span data-stu-id="588a4-159">Int32</span></span>|<span data-ttu-id="588a4-160">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="588a4-160">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="588a4-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="588a4-161">Response</span></span>
<span data-ttu-id="588a4-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="588a4-162">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="588a4-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="588a4-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="588a4-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="588a4-164">Request</span></span>
<span data-ttu-id="588a4-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="588a4-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="588a4-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="588a4-166">Response</span></span>
<span data-ttu-id="588a4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="588a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



