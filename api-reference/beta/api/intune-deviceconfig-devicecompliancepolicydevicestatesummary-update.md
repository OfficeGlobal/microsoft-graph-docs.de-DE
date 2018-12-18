---
title: Aktualisieren von „deviceCompliancePolicyDeviceStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCompliancePolicyDeviceStateSummary.
author: tfitzmac
ms.openlocfilehash: d7955abf7919259c52f6f709a18a654efe6703d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321847"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="e0ef1-103">Aktualisieren von „deviceCompliancePolicyDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="e0ef1-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="e0ef1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e0ef1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0ef1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e0ef1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0ef1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e0ef1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0ef1-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e0ef1-107">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0ef1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e0ef1-108">Prerequisites</span></span>
<span data-ttu-id="e0ef1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0ef1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0ef1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e0ef1-111">Permission type</span></span>|<span data-ttu-id="e0ef1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e0ef1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0ef1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e0ef1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0ef1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ef1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0ef1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e0ef1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0ef1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0ef1-116">Not supported.</span></span>|
|<span data-ttu-id="e0ef1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e0ef1-117">Application</span></span>|<span data-ttu-id="e0ef1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0ef1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0ef1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0ef1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="e0ef1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0ef1-120">Request headers</span></span>
|<span data-ttu-id="e0ef1-121">Header</span><span class="sxs-lookup"><span data-stu-id="e0ef1-121">Header</span></span>|<span data-ttu-id="e0ef1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e0ef1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0ef1-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e0ef1-123">Authorization</span></span>|<span data-ttu-id="e0ef1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e0ef1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0ef1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0ef1-125">Accept</span></span>|<span data-ttu-id="e0ef1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0ef1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0ef1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e0ef1-127">Request body</span></span>
<span data-ttu-id="e0ef1-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="e0ef1-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="e0ef1-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="e0ef1-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="e0ef1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e0ef1-130">Property</span></span>|<span data-ttu-id="e0ef1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e0ef1-131">Type</span></span>|<span data-ttu-id="e0ef1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0ef1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0ef1-133">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="e0ef1-133">inGracePeriodCount</span></span>|<span data-ttu-id="e0ef1-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ef1-134">Int32</span></span>|<span data-ttu-id="e0ef1-135">Anzahl von Geräten, die sich in der Toleranzperiode befinden</span><span class="sxs-lookup"><span data-stu-id="e0ef1-135">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="e0ef1-136">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="e0ef1-136">configManagerCount</span></span>|<span data-ttu-id="e0ef1-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ef1-137">Int32</span></span>|<span data-ttu-id="e0ef1-138">Anzahl von Geräten, deren Konformität mit System Center Configuration Manager verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="e0ef1-138">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="e0ef1-139">id</span><span class="sxs-lookup"><span data-stu-id="e0ef1-139">id</span></span>|<span data-ttu-id="e0ef1-140">String</span><span class="sxs-lookup"><span data-stu-id="e0ef1-140">String</span></span>|<span data-ttu-id="e0ef1-141">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e0ef1-141">Key of the entity.</span></span>|
|<span data-ttu-id="e0ef1-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0ef1-142">unknownDeviceCount</span></span>|<span data-ttu-id="e0ef1-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ef1-143">Int32</span></span>|<span data-ttu-id="e0ef1-144">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="e0ef1-144">Number of unknown devices</span></span>|
|<span data-ttu-id="e0ef1-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0ef1-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="e0ef1-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ef1-146">Int32</span></span>|<span data-ttu-id="e0ef1-147">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="e0ef1-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="e0ef1-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0ef1-148">compliantDeviceCount</span></span>|<span data-ttu-id="e0ef1-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ef1-149">Int32</span></span>|<span data-ttu-id="e0ef1-150">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="e0ef1-150">Number of compliant devices</span></span>|
|<span data-ttu-id="e0ef1-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0ef1-151">remediatedDeviceCount</span></span>|<span data-ttu-id="e0ef1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ef1-152">Int32</span></span>|<span data-ttu-id="e0ef1-153">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="e0ef1-153">Number of remediated devices</span></span>|
|<span data-ttu-id="e0ef1-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0ef1-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e0ef1-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ef1-155">Int32</span></span>|<span data-ttu-id="e0ef1-156">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="e0ef1-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e0ef1-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0ef1-157">errorDeviceCount</span></span>|<span data-ttu-id="e0ef1-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ef1-158">Int32</span></span>|<span data-ttu-id="e0ef1-159">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="e0ef1-159">Number of error devices</span></span>|
|<span data-ttu-id="e0ef1-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0ef1-160">conflictDeviceCount</span></span>|<span data-ttu-id="e0ef1-161">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ef1-161">Int32</span></span>|<span data-ttu-id="e0ef1-162">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="e0ef1-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="e0ef1-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0ef1-163">Response</span></span>
<span data-ttu-id="e0ef1-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e0ef1-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0ef1-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0ef1-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0ef1-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0ef1-166">Request</span></span>
<span data-ttu-id="e0ef1-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0ef1-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 270

{
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

### <a name="response"></a><span data-ttu-id="e0ef1-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0ef1-168">Response</span></span>
<span data-ttu-id="e0ef1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0ef1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





