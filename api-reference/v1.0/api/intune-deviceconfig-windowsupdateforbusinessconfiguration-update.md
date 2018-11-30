---
title: Aktualisieren von „windowsUpdateForBusinessConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windowsUpdateForBusinessConfiguration.
ms.openlocfilehash: 17538d2fb06af92e8b8f5ec63a023d6fe2c0bdbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019740"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="f6eb6-103">Aktualisieren von „windowsUpdateForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="f6eb6-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="f6eb6-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6eb6-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6eb6-105">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f6eb6-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f6eb6-106">Prerequisites</span></span>
<span data-ttu-id="f6eb6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6eb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6eb6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6eb6-109">Permission type</span></span>|<span data-ttu-id="f6eb6-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6eb6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6eb6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6eb6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f6eb6-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6eb6-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6eb6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6eb6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6eb6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6eb6-114">Not supported.</span></span>|
|<span data-ttu-id="f6eb6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6eb6-115">Application</span></span>|<span data-ttu-id="f6eb6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6eb6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6eb6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6eb6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f6eb6-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6eb6-118">Request headers</span></span>
|<span data-ttu-id="f6eb6-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f6eb6-119">Header</span></span>|<span data-ttu-id="f6eb6-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f6eb6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6eb6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6eb6-121">Authorization</span></span>|<span data-ttu-id="f6eb6-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f6eb6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6eb6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f6eb6-123">Accept</span></span>|<span data-ttu-id="f6eb6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f6eb6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6eb6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6eb6-125">Request body</span></span>
<span data-ttu-id="f6eb6-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-126">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="f6eb6-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-127">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="f6eb6-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f6eb6-128">Property</span></span>|<span data-ttu-id="f6eb6-129">Typ</span><span class="sxs-lookup"><span data-stu-id="f6eb6-129">Type</span></span>|<span data-ttu-id="f6eb6-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6eb6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6eb6-131">id</span><span class="sxs-lookup"><span data-stu-id="f6eb6-131">id</span></span>|<span data-ttu-id="f6eb6-132">String</span><span class="sxs-lookup"><span data-stu-id="f6eb6-132">String</span></span>|<span data-ttu-id="f6eb6-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f6eb6-133">Key of the entity.</span></span> <span data-ttu-id="f6eb6-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6eb6-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6eb6-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6eb6-135">lastModifiedDateTime</span></span>|<span data-ttu-id="f6eb6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6eb6-136">DateTimeOffset</span></span>|<span data-ttu-id="f6eb6-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-137">DateTime the object was last modified.</span></span> <span data-ttu-id="f6eb6-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6eb6-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6eb6-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6eb6-139">createdDateTime</span></span>|<span data-ttu-id="f6eb6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6eb6-140">DateTimeOffset</span></span>|<span data-ttu-id="f6eb6-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-141">DateTime the object was created.</span></span> <span data-ttu-id="f6eb6-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6eb6-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6eb6-143">description</span><span class="sxs-lookup"><span data-stu-id="f6eb6-143">description</span></span>|<span data-ttu-id="f6eb6-144">String</span><span class="sxs-lookup"><span data-stu-id="f6eb6-144">String</span></span>|<span data-ttu-id="f6eb6-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f6eb6-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f6eb6-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6eb6-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6eb6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="f6eb6-147">displayName</span></span>|<span data-ttu-id="f6eb6-148">String</span><span class="sxs-lookup"><span data-stu-id="f6eb6-148">String</span></span>|<span data-ttu-id="f6eb6-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f6eb6-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f6eb6-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6eb6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6eb6-151">Version</span><span class="sxs-lookup"><span data-stu-id="f6eb6-151">version</span></span>|<span data-ttu-id="f6eb6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f6eb6-152">Int32</span></span>|<span data-ttu-id="f6eb6-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-153">Version of the device configuration.</span></span> <span data-ttu-id="f6eb6-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f6eb6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f6eb6-155">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f6eb6-155">deliveryOptimizationMode</span></span>|[<span data-ttu-id="f6eb6-156">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f6eb6-156">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="f6eb6-157">Übermittlung Optimierung Modus.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-157">Delivery Optimization Mode.</span></span> <span data-ttu-id="f6eb6-158">Mögliche Werte sind: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload` und `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-158">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="f6eb6-159">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="f6eb6-159">prereleaseFeatures</span></span>|[<span data-ttu-id="f6eb6-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="f6eb6-160">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="f6eb6-161">Pre-Release-Funktionen.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-161">The pre-release features.</span></span> <span data-ttu-id="f6eb6-162">Mögliche Werte sind: `userDefined`, `settingsOnly`, `settingsAndExperimentations` und `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-162">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="f6eb6-163">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="f6eb6-163">automaticUpdateMode</span></span>|[<span data-ttu-id="f6eb6-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="f6eb6-164">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="f6eb6-165">Modus für automatische Updates.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-165">Automatic update mode.</span></span> <span data-ttu-id="f6eb6-166">Mögliche Werte sind: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime` und `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-166">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="f6eb6-167">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="f6eb6-167">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="f6eb6-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6eb6-168">Boolean</span></span>|<span data-ttu-id="f6eb6-169">Legt fest, dass der Microsoft Update Service zugelassen wird.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-169">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="f6eb6-170">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="f6eb6-170">driversExcluded</span></span>|<span data-ttu-id="f6eb6-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6eb6-171">Boolean</span></span>|<span data-ttu-id="f6eb6-172">Legt fest, dass Treiber von Windows-Updates ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-172">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="f6eb6-173">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="f6eb6-173">installationSchedule</span></span>|[<span data-ttu-id="f6eb6-174">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="f6eb6-174">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="f6eb6-175">Installationszeitplan</span><span class="sxs-lookup"><span data-stu-id="f6eb6-175">Installation schedule</span></span>|
|<span data-ttu-id="f6eb6-176">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="f6eb6-176">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="f6eb6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f6eb6-177">Int32</span></span>|<span data-ttu-id="f6eb6-178">Legt fest, um wie viele Tage Qualitätsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-178">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="f6eb6-179">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="f6eb6-179">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="f6eb6-180">Int32</span><span class="sxs-lookup"><span data-stu-id="f6eb6-180">Int32</span></span>|<span data-ttu-id="f6eb6-181">Legt fest, um wie viele Tage Funktionsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-181">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="f6eb6-182">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="f6eb6-182">qualityUpdatesPaused</span></span>|<span data-ttu-id="f6eb6-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6eb6-183">Boolean</span></span>|<span data-ttu-id="f6eb6-184">Setzt Qualitätsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-184">Pause Quality Updates</span></span>|
|<span data-ttu-id="f6eb6-185">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="f6eb6-185">featureUpdatesPaused</span></span>|<span data-ttu-id="f6eb6-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6eb6-186">Boolean</span></span>|<span data-ttu-id="f6eb6-187">Setzt Funktionsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-187">Pause Feature Updates</span></span>|
|<span data-ttu-id="f6eb6-188">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="f6eb6-188">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="f6eb6-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6eb6-189">DateTimeOffset</span></span>|<span data-ttu-id="f6eb6-190">Datum und Uhrzeit des Ablaufs der Aussetzung der Qualitätsupdates</span><span class="sxs-lookup"><span data-stu-id="f6eb6-190">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="f6eb6-191">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="f6eb6-191">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="f6eb6-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6eb6-192">DateTimeOffset</span></span>|<span data-ttu-id="f6eb6-193">Datum und Uhrzeit des Ablaufs der Aussetzung der Funktionsupdates</span><span class="sxs-lookup"><span data-stu-id="f6eb6-193">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="f6eb6-194">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="f6eb6-194">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="f6eb6-195">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="f6eb6-195">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="f6eb6-196">Bestimmt, welche Geräte Branch ihre Updates von erhält.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-196">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="f6eb6-197">Mögliche Werte sind: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow` und `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-197">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="f6eb6-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6eb6-198">Response</span></span>
<span data-ttu-id="f6eb6-199">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-199">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6eb6-200">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6eb6-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="f6eb6-201">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6eb6-201">Request</span></span>
<span data-ttu-id="f6eb6-202">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="f6eb6-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6eb6-203">Response</span></span>
<span data-ttu-id="f6eb6-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6eb6-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



