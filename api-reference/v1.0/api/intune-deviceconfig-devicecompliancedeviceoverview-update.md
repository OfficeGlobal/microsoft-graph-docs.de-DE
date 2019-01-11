---
title: Aktualisieren von „deviceComplianceDeviceOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceComplianceDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 884e8dc786196ff865c4f184a2f20a73926d3855
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876517"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="fa488-103">Aktualisieren von „deviceComplianceDeviceOverview“</span><span class="sxs-lookup"><span data-stu-id="fa488-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="fa488-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fa488-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa488-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="fa488-105">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa488-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa488-106">Prerequisites</span></span>
<span data-ttu-id="fa488-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa488-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa488-109">Permission type</span></span>|<span data-ttu-id="fa488-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa488-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa488-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa488-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa488-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa488-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa488-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa488-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa488-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa488-114">Not supported.</span></span>|
|<span data-ttu-id="fa488-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa488-115">Application</span></span>|<span data-ttu-id="fa488-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa488-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa488-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa488-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="fa488-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa488-118">Request headers</span></span>
|<span data-ttu-id="fa488-119">Header</span><span class="sxs-lookup"><span data-stu-id="fa488-119">Header</span></span>|<span data-ttu-id="fa488-120">Wert</span><span class="sxs-lookup"><span data-stu-id="fa488-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa488-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa488-121">Authorization</span></span>|<span data-ttu-id="fa488-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa488-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa488-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fa488-123">Accept</span></span>|<span data-ttu-id="fa488-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fa488-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa488-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa488-125">Request body</span></span>
<span data-ttu-id="fa488-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="fa488-126">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="fa488-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="fa488-127">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="fa488-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa488-128">Property</span></span>|<span data-ttu-id="fa488-129">Typ</span><span class="sxs-lookup"><span data-stu-id="fa488-129">Type</span></span>|<span data-ttu-id="fa488-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa488-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa488-131">id</span><span class="sxs-lookup"><span data-stu-id="fa488-131">id</span></span>|<span data-ttu-id="fa488-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa488-132">String</span></span>|<span data-ttu-id="fa488-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fa488-133">Key of the entity.</span></span>|
|<span data-ttu-id="fa488-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="fa488-134">pendingCount</span></span>|<span data-ttu-id="fa488-135">Int32</span><span class="sxs-lookup"><span data-stu-id="fa488-135">Int32</span></span>|<span data-ttu-id="fa488-136">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="fa488-136">Number of pending devices</span></span>|
|<span data-ttu-id="fa488-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="fa488-137">notApplicableCount</span></span>|<span data-ttu-id="fa488-138">Int32</span><span class="sxs-lookup"><span data-stu-id="fa488-138">Int32</span></span>|<span data-ttu-id="fa488-139">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="fa488-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="fa488-140">successCount</span><span class="sxs-lookup"><span data-stu-id="fa488-140">successCount</span></span>|<span data-ttu-id="fa488-141">Int32</span><span class="sxs-lookup"><span data-stu-id="fa488-141">Int32</span></span>|<span data-ttu-id="fa488-142">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="fa488-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="fa488-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="fa488-143">errorCount</span></span>|<span data-ttu-id="fa488-144">Int32</span><span class="sxs-lookup"><span data-stu-id="fa488-144">Int32</span></span>|<span data-ttu-id="fa488-145">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="fa488-145">Number of error devices</span></span>|
|<span data-ttu-id="fa488-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="fa488-146">failedCount</span></span>|<span data-ttu-id="fa488-147">Int32</span><span class="sxs-lookup"><span data-stu-id="fa488-147">Int32</span></span>|<span data-ttu-id="fa488-148">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="fa488-148">Number of failed devices</span></span>|
|<span data-ttu-id="fa488-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="fa488-149">lastUpdateDateTime</span></span>|<span data-ttu-id="fa488-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa488-150">DateTimeOffset</span></span>|<span data-ttu-id="fa488-151">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="fa488-151">Last update time</span></span>|
|<span data-ttu-id="fa488-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="fa488-152">configurationVersion</span></span>|<span data-ttu-id="fa488-153">Int32</span><span class="sxs-lookup"><span data-stu-id="fa488-153">Int32</span></span>|<span data-ttu-id="fa488-154">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="fa488-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="fa488-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa488-155">Response</span></span>
<span data-ttu-id="fa488-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fa488-156">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa488-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa488-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa488-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa488-158">Request</span></span>
<span data-ttu-id="fa488-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa488-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="fa488-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa488-160">Response</span></span>
<span data-ttu-id="fa488-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa488-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



