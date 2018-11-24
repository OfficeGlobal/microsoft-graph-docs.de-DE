# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="faed4-101">Erstellen von „windowsUpdateForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="faed4-101">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="faed4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="faed4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="faed4-103">Diese Methode erstellt ein neues Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faed4-103">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="faed4-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="faed4-104">Prerequisites</span></span>
<span data-ttu-id="faed4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="faed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="faed4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="faed4-107">Permission type</span></span>|<span data-ttu-id="faed4-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="faed4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faed4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="faed4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="faed4-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faed4-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="faed4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="faed4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faed4-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="faed4-112">Not supported.</span></span>|
|<span data-ttu-id="faed4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="faed4-113">Application</span></span>|<span data-ttu-id="faed4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="faed4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="faed4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="faed4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="faed4-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="faed4-116">Request headers</span></span>
|<span data-ttu-id="faed4-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="faed4-117">Header</span></span>|<span data-ttu-id="faed4-118">Wert</span><span class="sxs-lookup"><span data-stu-id="faed4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faed4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="faed4-119">Authorization</span></span>|<span data-ttu-id="faed4-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="faed4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faed4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="faed4-121">Accept</span></span>|<span data-ttu-id="faed4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="faed4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faed4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="faed4-123">Request body</span></span>
<span data-ttu-id="faed4-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsUpdateForBusinessConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="faed4-124">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="faed4-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsUpdateForBusinessConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="faed4-125">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="faed4-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="faed4-126">Property</span></span>|<span data-ttu-id="faed4-127">Typ</span><span class="sxs-lookup"><span data-stu-id="faed4-127">Type</span></span>|<span data-ttu-id="faed4-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="faed4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faed4-129">id</span><span class="sxs-lookup"><span data-stu-id="faed4-129">id</span></span>|<span data-ttu-id="faed4-130">String</span><span class="sxs-lookup"><span data-stu-id="faed4-130">String</span></span>|<span data-ttu-id="faed4-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="faed4-131">Key of the entity.</span></span> <span data-ttu-id="faed4-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faed4-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faed4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="faed4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="faed4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faed4-134">DateTimeOffset</span></span>|<span data-ttu-id="faed4-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="faed4-135">DateTime the object was last modified.</span></span> <span data-ttu-id="faed4-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faed4-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faed4-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="faed4-137">createdDateTime</span></span>|<span data-ttu-id="faed4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faed4-138">DateTimeOffset</span></span>|<span data-ttu-id="faed4-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="faed4-139">DateTime the object was created.</span></span> <span data-ttu-id="faed4-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faed4-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faed4-141">description</span><span class="sxs-lookup"><span data-stu-id="faed4-141">description</span></span>|<span data-ttu-id="faed4-142">String</span><span class="sxs-lookup"><span data-stu-id="faed4-142">String</span></span>|<span data-ttu-id="faed4-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="faed4-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="faed4-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faed4-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faed4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="faed4-145">displayName</span></span>|<span data-ttu-id="faed4-146">String</span><span class="sxs-lookup"><span data-stu-id="faed4-146">String</span></span>|<span data-ttu-id="faed4-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="faed4-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="faed4-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faed4-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faed4-149">version</span><span class="sxs-lookup"><span data-stu-id="faed4-149">version</span></span>|<span data-ttu-id="faed4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="faed4-150">Int32</span></span>|<span data-ttu-id="faed4-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="faed4-151">Version of the device configuration.</span></span> <span data-ttu-id="faed4-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="faed4-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faed4-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="faed4-153">deliveryOptimizationMode</span></span>|[<span data-ttu-id="faed4-154">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="faed4-154">windowsDeliveryOptimizationMode</span></span>](../resources/intune_deviceconfig_windowsdeliveryoptimizationmode.md)|<span data-ttu-id="faed4-155">Übermittlung Optimierung Modus.</span><span class="sxs-lookup"><span data-stu-id="faed4-155">Delivery Optimization Mode.</span></span> <span data-ttu-id="faed4-156">Mögliche Werte sind: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload` und `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="faed4-156">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="faed4-157">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="faed4-157">prereleaseFeatures</span></span>|[<span data-ttu-id="faed4-158">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="faed4-158">prereleaseFeatures</span></span>](../resources/intune_deviceconfig_prereleasefeatures.md)|<span data-ttu-id="faed4-159">Pre-Release-Funktionen.</span><span class="sxs-lookup"><span data-stu-id="faed4-159">The pre-release features.</span></span> <span data-ttu-id="faed4-160">Mögliche Werte sind: `userDefined`, `settingsOnly`, `settingsAndExperimentations` und `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="faed4-160">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="faed4-161">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="faed4-161">automaticUpdateMode</span></span>|[<span data-ttu-id="faed4-162">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="faed4-162">automaticUpdateMode</span></span>](../resources/intune_deviceconfig_automaticupdatemode.md)|<span data-ttu-id="faed4-163">Modus für automatische Updates.</span><span class="sxs-lookup"><span data-stu-id="faed4-163">Automatic update mode.</span></span> <span data-ttu-id="faed4-164">Mögliche Werte sind: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime` und `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="faed4-164">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="faed4-165">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="faed4-165">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="faed4-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="faed4-166">Boolean</span></span>|<span data-ttu-id="faed4-167">Legt fest, dass der Microsoft Update Service zugelassen wird.</span><span class="sxs-lookup"><span data-stu-id="faed4-167">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="faed4-168">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="faed4-168">driversExcluded</span></span>|<span data-ttu-id="faed4-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="faed4-169">Boolean</span></span>|<span data-ttu-id="faed4-170">Legt fest, dass Treiber von Windows-Updates ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="faed4-170">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="faed4-171">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="faed4-171">installationSchedule</span></span>|[<span data-ttu-id="faed4-172">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="faed4-172">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="faed4-173">Installationszeitplan</span><span class="sxs-lookup"><span data-stu-id="faed4-173">Installation schedule</span></span>|
|<span data-ttu-id="faed4-174">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="faed4-174">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="faed4-175">Int32</span><span class="sxs-lookup"><span data-stu-id="faed4-175">Int32</span></span>|<span data-ttu-id="faed4-176">Legt fest, um wie viele Tage Qualitätsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="faed4-176">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="faed4-177">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="faed4-177">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="faed4-178">Int32</span><span class="sxs-lookup"><span data-stu-id="faed4-178">Int32</span></span>|<span data-ttu-id="faed4-179">Legt fest, um wie viele Tage Funktionsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="faed4-179">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="faed4-180">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="faed4-180">qualityUpdatesPaused</span></span>|<span data-ttu-id="faed4-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="faed4-181">Boolean</span></span>|<span data-ttu-id="faed4-182">Setzt Qualitätsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="faed4-182">Pause Quality Updates</span></span>|
|<span data-ttu-id="faed4-183">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="faed4-183">featureUpdatesPaused</span></span>|<span data-ttu-id="faed4-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="faed4-184">Boolean</span></span>|<span data-ttu-id="faed4-185">Setzt Funktionsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="faed4-185">Pause Feature Updates</span></span>|
|<span data-ttu-id="faed4-186">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="faed4-186">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="faed4-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faed4-187">DateTimeOffset</span></span>|<span data-ttu-id="faed4-188">Datum und Uhrzeit des Ablaufs der Aussetzung der Qualitätsupdates</span><span class="sxs-lookup"><span data-stu-id="faed4-188">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="faed4-189">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="faed4-189">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="faed4-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faed4-190">DateTimeOffset</span></span>|<span data-ttu-id="faed4-191">Datum und Uhrzeit des Ablaufs der Aussetzung der Funktionsupdates</span><span class="sxs-lookup"><span data-stu-id="faed4-191">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="faed4-192">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="faed4-192">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="faed4-193">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="faed4-193">windowsUpdateType</span></span>](../resources/intune_deviceconfig_windowsupdatetype.md)|<span data-ttu-id="faed4-194">Bestimmt, welche Geräte Branch ihre Updates von erhält.</span><span class="sxs-lookup"><span data-stu-id="faed4-194">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="faed4-195">Mögliche Werte sind: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow` und `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="faed4-195">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="faed4-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="faed4-196">Response</span></span>
<span data-ttu-id="faed4-197">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="faed4-197">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faed4-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="faed4-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="faed4-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="faed4-199">Request</span></span>
<span data-ttu-id="faed4-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="faed4-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="faed4-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="faed4-201">Response</span></span>
<span data-ttu-id="faed4-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="faed4-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



