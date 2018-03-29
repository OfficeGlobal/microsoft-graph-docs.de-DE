# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="af2c8-101">Erstellen von „windowsUpdateForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="af2c8-101">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="af2c8-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="af2c8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af2c8-103">Diese Methode erstellt ein neues Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af2c8-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af2c8-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="af2c8-104">Prerequisites</span></span>
<span data-ttu-id="af2c8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="af2c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="af2c8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="af2c8-107">Permission type</span></span>|<span data-ttu-id="af2c8-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="af2c8-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af2c8-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="af2c8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="af2c8-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af2c8-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af2c8-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="af2c8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af2c8-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af2c8-112">Not supported.</span></span>|
|<span data-ttu-id="af2c8-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="af2c8-113">Application</span></span>|<span data-ttu-id="af2c8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af2c8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af2c8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="af2c8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="af2c8-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="af2c8-116">Request headers</span></span>
|<span data-ttu-id="af2c8-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="af2c8-117">Header</span></span>|<span data-ttu-id="af2c8-118">Wert</span><span class="sxs-lookup"><span data-stu-id="af2c8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af2c8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="af2c8-119">Authorization</span></span>|<span data-ttu-id="af2c8-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="af2c8-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="af2c8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="af2c8-121">Accept</span></span>|<span data-ttu-id="af2c8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="af2c8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af2c8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="af2c8-123">Request body</span></span>
<span data-ttu-id="af2c8-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsUpdateForBusinessConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="af2c8-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="af2c8-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsUpdateForBusinessConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="af2c8-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="af2c8-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="af2c8-126">Property</span></span>|<span data-ttu-id="af2c8-127">Typ</span><span class="sxs-lookup"><span data-stu-id="af2c8-127">Type</span></span>|<span data-ttu-id="af2c8-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af2c8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af2c8-129">id</span><span class="sxs-lookup"><span data-stu-id="af2c8-129">id</span></span>|<span data-ttu-id="af2c8-130">String</span><span class="sxs-lookup"><span data-stu-id="af2c8-130">String</span></span>|<span data-ttu-id="af2c8-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="af2c8-131">Key of the setting.</span></span> <span data-ttu-id="af2c8-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af2c8-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af2c8-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af2c8-133">lastModifiedDateTime</span></span>|<span data-ttu-id="af2c8-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af2c8-134">DateTimeOffset</span></span>|<span data-ttu-id="af2c8-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="af2c8-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="af2c8-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af2c8-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af2c8-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af2c8-137">createdDateTime</span></span>|<span data-ttu-id="af2c8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af2c8-138">DateTimeOffset</span></span>|<span data-ttu-id="af2c8-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="af2c8-139">DateTime the object was created.</span></span> <span data-ttu-id="af2c8-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af2c8-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af2c8-141">description</span><span class="sxs-lookup"><span data-stu-id="af2c8-141">description</span></span>|<span data-ttu-id="af2c8-142">String</span><span class="sxs-lookup"><span data-stu-id="af2c8-142">String</span></span>|<span data-ttu-id="af2c8-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="af2c8-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="af2c8-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af2c8-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af2c8-145">displayName</span><span class="sxs-lookup"><span data-stu-id="af2c8-145">displayName</span></span>|<span data-ttu-id="af2c8-146">String</span><span class="sxs-lookup"><span data-stu-id="af2c8-146">String</span></span>|<span data-ttu-id="af2c8-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="af2c8-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="af2c8-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af2c8-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af2c8-149">version</span><span class="sxs-lookup"><span data-stu-id="af2c8-149">version</span></span>|<span data-ttu-id="af2c8-150">Int32</span><span class="sxs-lookup"><span data-stu-id="af2c8-150">Int32</span></span>|<span data-ttu-id="af2c8-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="af2c8-151">Version of the device configuration.</span></span> <span data-ttu-id="af2c8-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af2c8-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af2c8-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="af2c8-153">deliveryOptimizationMode</span></span>|<span data-ttu-id="af2c8-154">String</span><span class="sxs-lookup"><span data-stu-id="af2c8-154">String</span></span>|<span data-ttu-id="af2c8-155">Delivery Optimization Mode. Mögliche Werte sind: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload` und `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="af2c8-155">Delivery Optimization Mode Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="af2c8-156">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="af2c8-156">prereleaseFeatures</span></span>|<span data-ttu-id="af2c8-157">String</span><span class="sxs-lookup"><span data-stu-id="af2c8-157">String</span></span>|<span data-ttu-id="af2c8-158">Pre-Release-Funktionen.</span><span class="sxs-lookup"><span data-stu-id="af2c8-158">The pre-release features.</span></span> <span data-ttu-id="af2c8-159">Mögliche Werte sind: `userDefined`, `settingsOnly`, `settingsAndExperimentations` und `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="af2c8-159">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="af2c8-160">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="af2c8-160">automaticUpdateMode</span></span>|<span data-ttu-id="af2c8-161">String</span><span class="sxs-lookup"><span data-stu-id="af2c8-161">String</span></span>|<span data-ttu-id="af2c8-162">Modus für automatische Updates.</span><span class="sxs-lookup"><span data-stu-id="af2c8-162">Automatic update mode.</span></span> <span data-ttu-id="af2c8-163">Mögliche Werte sind: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime` und `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="af2c8-163">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="af2c8-164">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="af2c8-164">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="af2c8-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="af2c8-165">Boolean</span></span>|<span data-ttu-id="af2c8-166">Legt fest, dass der Microsoft Update Service zugelassen wird.</span><span class="sxs-lookup"><span data-stu-id="af2c8-166">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="af2c8-167">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="af2c8-167">driversExcluded</span></span>|<span data-ttu-id="af2c8-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="af2c8-168">Boolean</span></span>|<span data-ttu-id="af2c8-169">Legt fest, dass Treiber von Windows-Updates ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="af2c8-169">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="af2c8-170">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="af2c8-170">installationSchedule</span></span>|[<span data-ttu-id="af2c8-171">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="af2c8-171">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="af2c8-172">Installationszeitplan</span><span class="sxs-lookup"><span data-stu-id="af2c8-172">Installation schedule</span></span>|
|<span data-ttu-id="af2c8-173">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="af2c8-173">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="af2c8-174">Int32</span><span class="sxs-lookup"><span data-stu-id="af2c8-174">Int32</span></span>|<span data-ttu-id="af2c8-175">Legt fest, um wie viele Tage Qualitätsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="af2c8-175">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="af2c8-176">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="af2c8-176">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="af2c8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="af2c8-177">Int32</span></span>|<span data-ttu-id="af2c8-178">Legt fest, um wie viele Tage Funktionsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="af2c8-178">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="af2c8-179">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="af2c8-179">qualityUpdatesPaused</span></span>|<span data-ttu-id="af2c8-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="af2c8-180">Boolean</span></span>|<span data-ttu-id="af2c8-181">Setzt Qualitätsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="af2c8-181">Pause Quality Updates</span></span>|
|<span data-ttu-id="af2c8-182">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="af2c8-182">featureUpdatesPaused</span></span>|<span data-ttu-id="af2c8-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="af2c8-183">Boolean</span></span>|<span data-ttu-id="af2c8-184">Setzt Funktionsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="af2c8-184">Pause Feature Updates</span></span>|
|<span data-ttu-id="af2c8-185">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="af2c8-185">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="af2c8-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af2c8-186">DateTimeOffset</span></span>|<span data-ttu-id="af2c8-187">Datum und Uhrzeit des Ablaufs der Aussetzung der Qualitätsupdates</span><span class="sxs-lookup"><span data-stu-id="af2c8-187">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="af2c8-188">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="af2c8-188">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="af2c8-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af2c8-189">DateTimeOffset</span></span>|<span data-ttu-id="af2c8-190">Datum und Uhrzeit des Ablaufs der Aussetzung der Funktionsupdates</span><span class="sxs-lookup"><span data-stu-id="af2c8-190">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="af2c8-191">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="af2c8-191">businessReadyUpdatesOnly</span></span>|<span data-ttu-id="af2c8-192">String</span><span class="sxs-lookup"><span data-stu-id="af2c8-192">String</span></span>|<span data-ttu-id="af2c8-193">Legt fest, aus welchem Branch Geräte Updates erhalten sollen. Mögliche Werte sind: `userDefined`, `all` und `businessReadyOnly`.</span><span class="sxs-lookup"><span data-stu-id="af2c8-193">Determines which branch devices will receive their updates from Possible values are: `userDefined`, `all`, `businessReadyOnly`.</span></span>|



## <a name="response"></a><span data-ttu-id="af2c8-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="af2c8-194">Response</span></span>
<span data-ttu-id="af2c8-195">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="af2c8-195">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af2c8-196">Beispiel</span><span class="sxs-lookup"><span data-stu-id="af2c8-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="af2c8-197">Anforderung</span><span class="sxs-lookup"><span data-stu-id="af2c8-197">Request</span></span>
<span data-ttu-id="af2c8-198">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="af2c8-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="af2c8-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="af2c8-199">Response</span></span>
<span data-ttu-id="af2c8-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="af2c8-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



