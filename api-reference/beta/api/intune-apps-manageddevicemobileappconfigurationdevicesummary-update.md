---
title: Aktualisieren von „managedDeviceMobileAppConfigurationDeviceSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef7e7ef9a7ef41c4fbc00eeff4750e11e5c3cbc1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962869"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="85932-103">Aktualisieren von „managedDeviceMobileAppConfigurationDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="85932-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="85932-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85932-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85932-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="85932-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85932-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="85932-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85932-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="85932-107">Prerequisites</span></span>
<span data-ttu-id="85932-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85932-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85932-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="85932-110">Permission type</span></span>|<span data-ttu-id="85932-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="85932-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85932-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="85932-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85932-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85932-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="85932-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="85932-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85932-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85932-115">Not supported.</span></span>|
|<span data-ttu-id="85932-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="85932-116">Application</span></span>|<span data-ttu-id="85932-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85932-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85932-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85932-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="85932-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85932-119">Request headers</span></span>
|<span data-ttu-id="85932-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="85932-120">Header</span></span>|<span data-ttu-id="85932-121">Wert</span><span class="sxs-lookup"><span data-stu-id="85932-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85932-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85932-122">Authorization</span></span>|<span data-ttu-id="85932-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="85932-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85932-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="85932-124">Accept</span></span>|<span data-ttu-id="85932-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85932-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85932-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85932-126">Request body</span></span>
<span data-ttu-id="85932-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="85932-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="85932-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="85932-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="85932-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85932-129">Property</span></span>|<span data-ttu-id="85932-130">Typ</span><span class="sxs-lookup"><span data-stu-id="85932-130">Type</span></span>|<span data-ttu-id="85932-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85932-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85932-132">id</span><span class="sxs-lookup"><span data-stu-id="85932-132">id</span></span>|<span data-ttu-id="85932-133">String</span><span class="sxs-lookup"><span data-stu-id="85932-133">String</span></span>|<span data-ttu-id="85932-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="85932-134">Key of the entity.</span></span>|
|<span data-ttu-id="85932-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="85932-135">pendingCount</span></span>|<span data-ttu-id="85932-136">Int32</span><span class="sxs-lookup"><span data-stu-id="85932-136">Int32</span></span>|<span data-ttu-id="85932-137">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="85932-137">Number of pending devices</span></span>|
|<span data-ttu-id="85932-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="85932-138">notApplicableCount</span></span>|<span data-ttu-id="85932-139">Int32</span><span class="sxs-lookup"><span data-stu-id="85932-139">Int32</span></span>|<span data-ttu-id="85932-140">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="85932-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="85932-141">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="85932-141">notApplicablePlatformCount</span></span>|<span data-ttu-id="85932-142">Int32</span><span class="sxs-lookup"><span data-stu-id="85932-142">Int32</span></span>|<span data-ttu-id="85932-143">Anzahl der nicht anwendbaren Geräte aufgrund fehlender Platt Form und Richtlinie</span><span class="sxs-lookup"><span data-stu-id="85932-143">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="85932-144">successCount</span><span class="sxs-lookup"><span data-stu-id="85932-144">successCount</span></span>|<span data-ttu-id="85932-145">Int32</span><span class="sxs-lookup"><span data-stu-id="85932-145">Int32</span></span>|<span data-ttu-id="85932-146">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="85932-146">Number of succeeded devices</span></span>|
|<span data-ttu-id="85932-147">errorCount</span><span class="sxs-lookup"><span data-stu-id="85932-147">errorCount</span></span>|<span data-ttu-id="85932-148">Int32</span><span class="sxs-lookup"><span data-stu-id="85932-148">Int32</span></span>|<span data-ttu-id="85932-149">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="85932-149">Number of error devices</span></span>|
|<span data-ttu-id="85932-150">failedCount</span><span class="sxs-lookup"><span data-stu-id="85932-150">failedCount</span></span>|<span data-ttu-id="85932-151">Int32</span><span class="sxs-lookup"><span data-stu-id="85932-151">Int32</span></span>|<span data-ttu-id="85932-152">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="85932-152">Number of failed devices</span></span>|
|<span data-ttu-id="85932-153">Conflictcount zur</span><span class="sxs-lookup"><span data-stu-id="85932-153">conflictCount</span></span>|<span data-ttu-id="85932-154">Int32</span><span class="sxs-lookup"><span data-stu-id="85932-154">Int32</span></span>|<span data-ttu-id="85932-155">Anzahl der in Konflikt stehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="85932-155">Number of devices in conflict</span></span>|
|<span data-ttu-id="85932-156">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="85932-156">lastUpdateDateTime</span></span>|<span data-ttu-id="85932-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85932-157">DateTimeOffset</span></span>|<span data-ttu-id="85932-158">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="85932-158">Last update time</span></span>|
|<span data-ttu-id="85932-159">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="85932-159">configurationVersion</span></span>|<span data-ttu-id="85932-160">Int32</span><span class="sxs-lookup"><span data-stu-id="85932-160">Int32</span></span>|<span data-ttu-id="85932-161">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="85932-161">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="85932-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="85932-162">Response</span></span>
<span data-ttu-id="85932-163">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="85932-163">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85932-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85932-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="85932-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85932-165">Request</span></span>
<span data-ttu-id="85932-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="85932-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
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

### <a name="response"></a><span data-ttu-id="85932-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="85932-167">Response</span></span>
<span data-ttu-id="85932-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85932-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
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




