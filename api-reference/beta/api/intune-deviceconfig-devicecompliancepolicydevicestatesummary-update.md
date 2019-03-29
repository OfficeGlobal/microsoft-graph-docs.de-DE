---
title: Aktualisieren von „deviceCompliancePolicyDeviceStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceCompliancePolicyDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0ebfa288def2c43c5d6b5491a525f704dc401b9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984121"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="86cd7-103">Aktualisieren von „deviceCompliancePolicyDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="86cd7-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="86cd7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="86cd7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86cd7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="86cd7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86cd7-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="86cd7-106">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86cd7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="86cd7-107">Prerequisites</span></span>
<span data-ttu-id="86cd7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86cd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86cd7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86cd7-110">Permission type</span></span>|<span data-ttu-id="86cd7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86cd7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86cd7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86cd7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86cd7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86cd7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86cd7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="86cd7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86cd7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86cd7-115">Not supported.</span></span>|
|<span data-ttu-id="86cd7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86cd7-116">Application</span></span>|<span data-ttu-id="86cd7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86cd7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86cd7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86cd7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="86cd7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86cd7-119">Request headers</span></span>
|<span data-ttu-id="86cd7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="86cd7-120">Header</span></span>|<span data-ttu-id="86cd7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="86cd7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86cd7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86cd7-122">Authorization</span></span>|<span data-ttu-id="86cd7-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="86cd7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86cd7-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="86cd7-124">Accept</span></span>|<span data-ttu-id="86cd7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86cd7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86cd7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="86cd7-126">Request body</span></span>
<span data-ttu-id="86cd7-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="86cd7-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="86cd7-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="86cd7-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="86cd7-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86cd7-129">Property</span></span>|<span data-ttu-id="86cd7-130">Typ</span><span class="sxs-lookup"><span data-stu-id="86cd7-130">Type</span></span>|<span data-ttu-id="86cd7-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86cd7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86cd7-132">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="86cd7-132">inGracePeriodCount</span></span>|<span data-ttu-id="86cd7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd7-133">Int32</span></span>|<span data-ttu-id="86cd7-134">Anzahl von Geräten, die sich in der Toleranzperiode befinden</span><span class="sxs-lookup"><span data-stu-id="86cd7-134">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="86cd7-135">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="86cd7-135">configManagerCount</span></span>|<span data-ttu-id="86cd7-136">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd7-136">Int32</span></span>|<span data-ttu-id="86cd7-137">Anzahl von Geräten, deren Konformität mit System Center Configuration Manager verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="86cd7-137">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="86cd7-138">id</span><span class="sxs-lookup"><span data-stu-id="86cd7-138">id</span></span>|<span data-ttu-id="86cd7-139">String</span><span class="sxs-lookup"><span data-stu-id="86cd7-139">String</span></span>|<span data-ttu-id="86cd7-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="86cd7-140">Key of the entity.</span></span>|
|<span data-ttu-id="86cd7-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86cd7-141">unknownDeviceCount</span></span>|<span data-ttu-id="86cd7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd7-142">Int32</span></span>|<span data-ttu-id="86cd7-143">Anzahl der unbekannten Geräte</span><span class="sxs-lookup"><span data-stu-id="86cd7-143">Number of unknown devices</span></span>|
|<span data-ttu-id="86cd7-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86cd7-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="86cd7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd7-145">Int32</span></span>|<span data-ttu-id="86cd7-146">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="86cd7-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="86cd7-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86cd7-147">compliantDeviceCount</span></span>|<span data-ttu-id="86cd7-148">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd7-148">Int32</span></span>|<span data-ttu-id="86cd7-149">Anzahl der konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="86cd7-149">Number of compliant devices</span></span>|
|<span data-ttu-id="86cd7-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86cd7-150">remediatedDeviceCount</span></span>|<span data-ttu-id="86cd7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd7-151">Int32</span></span>|<span data-ttu-id="86cd7-152">Anzahl der korrigierten Geräte</span><span class="sxs-lookup"><span data-stu-id="86cd7-152">Number of remediated devices</span></span>|
|<span data-ttu-id="86cd7-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86cd7-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="86cd7-154">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd7-154">Int32</span></span>|<span data-ttu-id="86cd7-155">Anzahl der nicht konformen Geräte</span><span class="sxs-lookup"><span data-stu-id="86cd7-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="86cd7-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86cd7-156">errorDeviceCount</span></span>|<span data-ttu-id="86cd7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd7-157">Int32</span></span>|<span data-ttu-id="86cd7-158">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="86cd7-158">Number of error devices</span></span>|
|<span data-ttu-id="86cd7-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86cd7-159">conflictDeviceCount</span></span>|<span data-ttu-id="86cd7-160">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd7-160">Int32</span></span>|<span data-ttu-id="86cd7-161">Anzahl der Geräte mit Konflikten</span><span class="sxs-lookup"><span data-stu-id="86cd7-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="86cd7-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="86cd7-162">Response</span></span>
<span data-ttu-id="86cd7-163">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="86cd7-163">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86cd7-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86cd7-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="86cd7-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="86cd7-165">Request</span></span>
<span data-ttu-id="86cd7-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86cd7-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
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

### <a name="response"></a><span data-ttu-id="86cd7-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="86cd7-167">Response</span></span>
<span data-ttu-id="86cd7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86cd7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




