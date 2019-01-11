---
title: Erstellen von „windowsUpdateForBusinessConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5166e54fbe7066644b751985b101d1876529ded8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872765"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="d5624-103">Erstellen von „windowsUpdateForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="d5624-103">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="d5624-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d5624-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5624-105">Diese Methode erstellt ein neues Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5624-105">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5624-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d5624-106">Prerequisites</span></span>
<span data-ttu-id="d5624-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5624-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5624-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d5624-109">Permission type</span></span>|<span data-ttu-id="d5624-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d5624-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5624-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d5624-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d5624-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5624-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d5624-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d5624-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5624-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5624-114">Not supported.</span></span>|
|<span data-ttu-id="d5624-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d5624-115">Application</span></span>|<span data-ttu-id="d5624-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5624-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5624-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5624-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d5624-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d5624-118">Request headers</span></span>
|<span data-ttu-id="d5624-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d5624-119">Header</span></span>|<span data-ttu-id="d5624-120">Wert</span><span class="sxs-lookup"><span data-stu-id="d5624-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5624-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5624-121">Authorization</span></span>|<span data-ttu-id="d5624-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d5624-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5624-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d5624-123">Accept</span></span>|<span data-ttu-id="d5624-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d5624-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5624-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d5624-125">Request body</span></span>
<span data-ttu-id="d5624-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsUpdateForBusinessConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="d5624-126">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="d5624-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsUpdateForBusinessConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="d5624-127">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="d5624-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d5624-128">Property</span></span>|<span data-ttu-id="d5624-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d5624-129">Type</span></span>|<span data-ttu-id="d5624-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5624-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5624-131">id</span><span class="sxs-lookup"><span data-stu-id="d5624-131">id</span></span>|<span data-ttu-id="d5624-132">String</span><span class="sxs-lookup"><span data-stu-id="d5624-132">String</span></span>|<span data-ttu-id="d5624-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d5624-133">Key of the entity.</span></span> <span data-ttu-id="d5624-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5624-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5624-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5624-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d5624-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5624-136">DateTimeOffset</span></span>|<span data-ttu-id="d5624-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d5624-137">DateTime the object was last modified.</span></span> <span data-ttu-id="d5624-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5624-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5624-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5624-139">createdDateTime</span></span>|<span data-ttu-id="d5624-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5624-140">DateTimeOffset</span></span>|<span data-ttu-id="d5624-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d5624-141">DateTime the object was created.</span></span> <span data-ttu-id="d5624-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5624-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5624-143">description</span><span class="sxs-lookup"><span data-stu-id="d5624-143">description</span></span>|<span data-ttu-id="d5624-144">String</span><span class="sxs-lookup"><span data-stu-id="d5624-144">String</span></span>|<span data-ttu-id="d5624-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d5624-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d5624-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5624-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5624-147">displayName</span><span class="sxs-lookup"><span data-stu-id="d5624-147">displayName</span></span>|<span data-ttu-id="d5624-148">String</span><span class="sxs-lookup"><span data-stu-id="d5624-148">String</span></span>|<span data-ttu-id="d5624-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d5624-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d5624-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5624-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5624-151">Version</span><span class="sxs-lookup"><span data-stu-id="d5624-151">version</span></span>|<span data-ttu-id="d5624-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d5624-152">Int32</span></span>|<span data-ttu-id="d5624-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d5624-153">Version of the device configuration.</span></span> <span data-ttu-id="d5624-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5624-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5624-155">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="d5624-155">deliveryOptimizationMode</span></span>|[<span data-ttu-id="d5624-156">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="d5624-156">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="d5624-157">Übermittlung Optimierung Modus.</span><span class="sxs-lookup"><span data-stu-id="d5624-157">Delivery Optimization Mode.</span></span> <span data-ttu-id="d5624-158">Mögliche Werte sind: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload` und `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="d5624-158">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="d5624-159">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="d5624-159">prereleaseFeatures</span></span>|[<span data-ttu-id="d5624-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="d5624-160">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="d5624-161">Pre-Release-Funktionen.</span><span class="sxs-lookup"><span data-stu-id="d5624-161">The pre-release features.</span></span> <span data-ttu-id="d5624-162">Mögliche Werte sind: `userDefined`, `settingsOnly`, `settingsAndExperimentations` und `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="d5624-162">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="d5624-163">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="d5624-163">automaticUpdateMode</span></span>|[<span data-ttu-id="d5624-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="d5624-164">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="d5624-165">Modus für automatische Updates.</span><span class="sxs-lookup"><span data-stu-id="d5624-165">Automatic update mode.</span></span> <span data-ttu-id="d5624-166">Mögliche Werte sind: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime` und `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="d5624-166">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="d5624-167">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="d5624-167">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="d5624-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5624-168">Boolean</span></span>|<span data-ttu-id="d5624-169">Legt fest, dass der Microsoft Update Service zugelassen wird.</span><span class="sxs-lookup"><span data-stu-id="d5624-169">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="d5624-170">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="d5624-170">driversExcluded</span></span>|<span data-ttu-id="d5624-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5624-171">Boolean</span></span>|<span data-ttu-id="d5624-172">Legt fest, dass Treiber von Windows-Updates ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="d5624-172">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="d5624-173">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="d5624-173">installationSchedule</span></span>|[<span data-ttu-id="d5624-174">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="d5624-174">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="d5624-175">Installationszeitplan</span><span class="sxs-lookup"><span data-stu-id="d5624-175">Installation schedule</span></span>|
|<span data-ttu-id="d5624-176">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="d5624-176">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="d5624-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d5624-177">Int32</span></span>|<span data-ttu-id="d5624-178">Legt fest, um wie viele Tage Qualitätsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d5624-178">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="d5624-179">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="d5624-179">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="d5624-180">Int32</span><span class="sxs-lookup"><span data-stu-id="d5624-180">Int32</span></span>|<span data-ttu-id="d5624-181">Legt fest, um wie viele Tage Funktionsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d5624-181">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="d5624-182">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="d5624-182">qualityUpdatesPaused</span></span>|<span data-ttu-id="d5624-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5624-183">Boolean</span></span>|<span data-ttu-id="d5624-184">Setzt Qualitätsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="d5624-184">Pause Quality Updates</span></span>|
|<span data-ttu-id="d5624-185">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="d5624-185">featureUpdatesPaused</span></span>|<span data-ttu-id="d5624-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5624-186">Boolean</span></span>|<span data-ttu-id="d5624-187">Setzt Funktionsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="d5624-187">Pause Feature Updates</span></span>|
|<span data-ttu-id="d5624-188">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="d5624-188">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="d5624-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5624-189">DateTimeOffset</span></span>|<span data-ttu-id="d5624-190">Datum und Uhrzeit des Ablaufs der Aussetzung der Qualitätsupdates</span><span class="sxs-lookup"><span data-stu-id="d5624-190">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="d5624-191">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="d5624-191">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="d5624-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5624-192">DateTimeOffset</span></span>|<span data-ttu-id="d5624-193">Datum und Uhrzeit des Ablaufs der Aussetzung der Funktionsupdates</span><span class="sxs-lookup"><span data-stu-id="d5624-193">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="d5624-194">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="d5624-194">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="d5624-195">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="d5624-195">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="d5624-196">Bestimmt, welche Geräte Branch ihre Updates von erhält.</span><span class="sxs-lookup"><span data-stu-id="d5624-196">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="d5624-197">Mögliche Werte sind: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow` und `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="d5624-197">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="d5624-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5624-198">Response</span></span>
<span data-ttu-id="d5624-199">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d5624-199">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5624-200">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d5624-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5624-201">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5624-201">Request</span></span>
<span data-ttu-id="d5624-202">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d5624-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 910

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all"
}
```

### <a name="response"></a><span data-ttu-id="d5624-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5624-203">Response</span></span>
<span data-ttu-id="d5624-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d5624-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1082

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all"
}
```



