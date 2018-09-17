# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="cfe8b-101">Aktualisieren von „windowsUpdateForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="cfe8b-101">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="cfe8b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cfe8b-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfe8b-103">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cfe8b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cfe8b-104">Prerequisites</span></span>
<span data-ttu-id="cfe8b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cfe8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cfe8b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cfe8b-107">Permission type</span></span>|<span data-ttu-id="cfe8b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cfe8b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfe8b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cfe8b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cfe8b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfe8b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cfe8b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cfe8b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfe8b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cfe8b-112">Not supported.</span></span>|
|<span data-ttu-id="cfe8b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cfe8b-113">Application</span></span>|<span data-ttu-id="cfe8b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cfe8b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfe8b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cfe8b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cfe8b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cfe8b-116">Request headers</span></span>
|<span data-ttu-id="cfe8b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cfe8b-117">Header</span></span>|<span data-ttu-id="cfe8b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="cfe8b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfe8b-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cfe8b-119">Authorization</span></span>|<span data-ttu-id="cfe8b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cfe8b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfe8b-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="cfe8b-121">Accept</span></span>|<span data-ttu-id="cfe8b-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="cfe8b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfe8b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cfe8b-123">Request body</span></span>
<span data-ttu-id="cfe8b-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-124">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="cfe8b-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-125">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="cfe8b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cfe8b-126">Property</span></span>|<span data-ttu-id="cfe8b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="cfe8b-127">Type</span></span>|<span data-ttu-id="cfe8b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cfe8b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfe8b-129">ID</span><span class="sxs-lookup"><span data-stu-id="cfe8b-129">id</span></span>|<span data-ttu-id="cfe8b-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cfe8b-130">String</span></span>|<span data-ttu-id="cfe8b-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cfe8b-131">Key of the entity.</span></span> <span data-ttu-id="cfe8b-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfe8b-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfe8b-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfe8b-133">lastModifiedDateTime</span></span>|<span data-ttu-id="cfe8b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe8b-134">DateTimeOffset</span></span>|<span data-ttu-id="cfe8b-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-135">DateTime the object was last modified.</span></span> <span data-ttu-id="cfe8b-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfe8b-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfe8b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfe8b-137">createdDateTime</span></span>|<span data-ttu-id="cfe8b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe8b-138">DateTimeOffset</span></span>|<span data-ttu-id="cfe8b-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-139">DateTime the object was created.</span></span> <span data-ttu-id="cfe8b-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfe8b-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfe8b-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cfe8b-141">description</span></span>|<span data-ttu-id="cfe8b-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cfe8b-142">String</span></span>|<span data-ttu-id="cfe8b-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="cfe8b-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cfe8b-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfe8b-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfe8b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="cfe8b-145">displayName</span></span>|<span data-ttu-id="cfe8b-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cfe8b-146">String</span></span>|<span data-ttu-id="cfe8b-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="cfe8b-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cfe8b-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfe8b-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfe8b-149">Version</span><span class="sxs-lookup"><span data-stu-id="cfe8b-149">version</span></span>|<span data-ttu-id="cfe8b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe8b-150">Int32</span></span>|<span data-ttu-id="cfe8b-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-151">Version of the device configuration.</span></span> <span data-ttu-id="cfe8b-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfe8b-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfe8b-153">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="cfe8b-153">deliveryOptimizationMode</span></span>|[<span data-ttu-id="cfe8b-154">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="cfe8b-154">windowsDeliveryOptimizationMode</span></span>](../resources/intune_deviceconfig_windowsdeliveryoptimizationmode.md)|<span data-ttu-id="cfe8b-p108">Zustellungsoptimierungsmodus. Mögliche Werte: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload` und `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-p108">Delivery Optimization Mode Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="cfe8b-157">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="cfe8b-157">prereleaseFeatures</span></span>|[<span data-ttu-id="cfe8b-158">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="cfe8b-158">prereleaseFeatures</span></span>](../resources/intune_deviceconfig_prereleasefeatures.md)|<span data-ttu-id="cfe8b-p109">Die Vorabversion-Features. Mögliche Werte: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-p109">The pre-release features. The possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="cfe8b-161">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="cfe8b-161">automaticUpdateMode</span></span>|[<span data-ttu-id="cfe8b-162">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="cfe8b-162">automaticUpdateMode</span></span>](../resources/intune_deviceconfig_automaticupdatemode.md)|<span data-ttu-id="cfe8b-p110">Modus für automatische Updates. Mögliche Werte: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-p110">Automatic update mode. The possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="cfe8b-165">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="cfe8b-165">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="cfe8b-166">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cfe8b-166">Boolean</span></span>|<span data-ttu-id="cfe8b-167">Legt fest, dass der Microsoft Update Service zugelassen wird.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-167">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="cfe8b-168">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="cfe8b-168">driversExcluded</span></span>|<span data-ttu-id="cfe8b-169">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cfe8b-169">Boolean</span></span>|<span data-ttu-id="cfe8b-170">Legt fest, dass Treiber von Windows-Updates ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-170">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="cfe8b-171">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="cfe8b-171">installationSchedule</span></span>|[<span data-ttu-id="cfe8b-172">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="cfe8b-172">windowsUpdateInstallScheduleType</span></span>](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)|<span data-ttu-id="cfe8b-173">Installationszeitplan</span><span class="sxs-lookup"><span data-stu-id="cfe8b-173">Installation schedule</span></span>|
|<span data-ttu-id="cfe8b-174">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="cfe8b-174">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="cfe8b-175">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe8b-175">Int32</span></span>|<span data-ttu-id="cfe8b-176">Legt fest, um wie viele Tage Qualitätsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-176">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="cfe8b-177">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="cfe8b-177">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="cfe8b-178">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe8b-178">Int32</span></span>|<span data-ttu-id="cfe8b-179">Legt fest, um wie viele Tage Funktionsupdates zurückgestellt werden sollen.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-179">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="cfe8b-180">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="cfe8b-180">qualityUpdatesPaused</span></span>|<span data-ttu-id="cfe8b-181">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cfe8b-181">Boolean</span></span>|<span data-ttu-id="cfe8b-182">Setzt Qualitätsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-182">Pause Quality Updates</span></span>|
|<span data-ttu-id="cfe8b-183">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="cfe8b-183">featureUpdatesPaused</span></span>|<span data-ttu-id="cfe8b-184">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cfe8b-184">Boolean</span></span>|<span data-ttu-id="cfe8b-185">Setzt Funktionsupdates aus.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-185">Pause Feature Updates</span></span>|
|<span data-ttu-id="cfe8b-186">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="cfe8b-186">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="cfe8b-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe8b-187">DateTimeOffset</span></span>|<span data-ttu-id="cfe8b-188">Datum und Uhrzeit des Ablaufs der Aussetzung der Qualitätsupdates</span><span class="sxs-lookup"><span data-stu-id="cfe8b-188">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="cfe8b-189">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="cfe8b-189">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="cfe8b-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe8b-190">DateTimeOffset</span></span>|<span data-ttu-id="cfe8b-191">Datum und Uhrzeit des Ablaufs der Aussetzung der Funktionsupdates</span><span class="sxs-lookup"><span data-stu-id="cfe8b-191">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="cfe8b-192">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="cfe8b-192">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="cfe8b-193">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="cfe8b-193">windowsUpdateType</span></span>](../resources/intune_deviceconfig_windowsupdatetype.md)|<span data-ttu-id="cfe8b-p111">Bestimmt, welche Branch-Geräte ihre Updates erhalten von. Mögliche Werte: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-p111">Determines which branch devices will receive their updates from. The possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="cfe8b-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="cfe8b-196">Response</span></span>
<span data-ttu-id="cfe8b-197">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-197">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfe8b-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cfe8b-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="cfe8b-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cfe8b-199">Request</span></span>
<span data-ttu-id="cfe8b-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 898

{
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

### <a name="response"></a><span data-ttu-id="cfe8b-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="cfe8b-201">Response</span></span>
<span data-ttu-id="cfe8b-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cfe8b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








