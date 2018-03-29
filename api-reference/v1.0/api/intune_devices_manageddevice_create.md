# <a name="create-manageddevice"></a><span data-ttu-id="0c5b8-101">Erstellen von „managedDevice“</span><span class="sxs-lookup"><span data-stu-id="0c5b8-101">Create managedDevice</span></span>

> <span data-ttu-id="0c5b8-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c5b8-103">Diese Methode erstellt ein neues Objekt des Typs [managedDevice](../resources/intune_devices_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="0c5b8-103">Create a new [plannerBucket](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c5b8-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0c5b8-104">Prerequisites</span></span>
<span data-ttu-id="0c5b8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0c5b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0c5b8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0c5b8-107">Permission type</span></span>|<span data-ttu-id="0c5b8-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0c5b8-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c5b8-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0c5b8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0c5b8-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c5b8-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0c5b8-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0c5b8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c5b8-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c5b8-112">Not supported.</span></span>|
|<span data-ttu-id="0c5b8-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0c5b8-113">Application</span></span>|<span data-ttu-id="0c5b8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c5b8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c5b8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c5b8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="0c5b8-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0c5b8-116">Request headers</span></span>
|<span data-ttu-id="0c5b8-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0c5b8-117">Header</span></span>|<span data-ttu-id="0c5b8-118">Wert</span><span class="sxs-lookup"><span data-stu-id="0c5b8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c5b8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c5b8-119">Authorization</span></span>|<span data-ttu-id="0c5b8-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0c5b8-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0c5b8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0c5b8-121">Accept</span></span>|<span data-ttu-id="0c5b8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0c5b8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c5b8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0c5b8-123">Request body</span></span>
<span data-ttu-id="0c5b8-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedDevice“ an.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="0c5b8-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedDevice“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="0c5b8-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0c5b8-126">Property</span></span>|<span data-ttu-id="0c5b8-127">Typ</span><span class="sxs-lookup"><span data-stu-id="0c5b8-127">Type</span></span>|<span data-ttu-id="0c5b8-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c5b8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c5b8-129">id</span><span class="sxs-lookup"><span data-stu-id="0c5b8-129">id</span></span>|<span data-ttu-id="0c5b8-130">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-130">String</span></span>|<span data-ttu-id="0c5b8-131">Eindeutiger Bezeichner für das Gerät</span><span class="sxs-lookup"><span data-stu-id="0c5b8-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="0c5b8-132">userId</span><span class="sxs-lookup"><span data-stu-id="0c5b8-132">userID</span></span>|<span data-ttu-id="0c5b8-133">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-133">String</span></span>|<span data-ttu-id="0c5b8-134">Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="0c5b8-134">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="0c5b8-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="0c5b8-135">deviceName</span></span>|<span data-ttu-id="0c5b8-136">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-136">String</span></span>|<span data-ttu-id="0c5b8-137">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="0c5b8-137">Name of the device</span></span>|
|<span data-ttu-id="0c5b8-138">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="0c5b8-138">deviceActionResults</span></span>|<span data-ttu-id="0c5b8-139">Collection von Objekten des Typs [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0c5b8-139">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) collection</span></span>|<span data-ttu-id="0c5b8-140">Liste von Objekten des Typs „ComplexType deviceActionResult“</span><span class="sxs-lookup"><span data-stu-id="0c5b8-140">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="0c5b8-141">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="0c5b8-141">enrolledDateTime</span></span>|<span data-ttu-id="0c5b8-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c5b8-142">DateTimeOffset</span></span>|<span data-ttu-id="0c5b8-143">Datum und Uhrzeit der Geräteregistrierung</span><span class="sxs-lookup"><span data-stu-id="0c5b8-143">Enrollment time of the device.</span></span>|
|<span data-ttu-id="0c5b8-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0c5b8-144">lastSyncDateTime</span></span>|<span data-ttu-id="0c5b8-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c5b8-145">DateTimeOffset</span></span>|<span data-ttu-id="0c5b8-146">Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune</span><span class="sxs-lookup"><span data-stu-id="0c5b8-146">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="0c5b8-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0c5b8-147">operatingSystem</span></span>|<span data-ttu-id="0c5b8-148">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-148">String</span></span>|<span data-ttu-id="0c5b8-149">Betriebssystem des Geräts.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-149">Operating system of the device.</span></span> <span data-ttu-id="0c5b8-150">Windows, iOS usw.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-150">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="0c5b8-151">complianceState</span><span class="sxs-lookup"><span data-stu-id="0c5b8-151">complianceState</span></span>|<span data-ttu-id="0c5b8-152">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-152">String</span></span>|<span data-ttu-id="0c5b8-153">Konformitätsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-153">Compliance state of the device.</span></span> <span data-ttu-id="0c5b8-154">Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-154">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="0c5b8-155">jailBroken</span><span class="sxs-lookup"><span data-stu-id="0c5b8-155">jailBroken</span></span>|<span data-ttu-id="0c5b8-156">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-156">String</span></span>|<span data-ttu-id="0c5b8-157">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-157">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="0c5b8-158">managementAgent</span><span class="sxs-lookup"><span data-stu-id="0c5b8-158">managementAgent</span></span>|<span data-ttu-id="0c5b8-159">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-159">String</span></span>|<span data-ttu-id="0c5b8-160">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-160">Management channel of the device.</span></span> <span data-ttu-id="0c5b8-161">Intune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf` und `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-161">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="0c5b8-162">osVersion</span><span class="sxs-lookup"><span data-stu-id="0c5b8-162">osVersion</span></span>|<span data-ttu-id="0c5b8-163">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-163">String</span></span>|<span data-ttu-id="0c5b8-164">Auf dem Gerät installierte Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="0c5b8-164">Operating system version of the device.</span></span>|
|<span data-ttu-id="0c5b8-165">easActivated</span><span class="sxs-lookup"><span data-stu-id="0c5b8-165">easActivated</span></span>|<span data-ttu-id="0c5b8-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c5b8-166">Boolean</span></span>|<span data-ttu-id="0c5b8-167">Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-167">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="0c5b8-168">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="0c5b8-168">easDeviceId</span></span>|<span data-ttu-id="0c5b8-169">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-169">String</span></span>|<span data-ttu-id="0c5b8-170">Exchange ActiveSync-ID des Geräts</span><span class="sxs-lookup"><span data-stu-id="0c5b8-170">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="0c5b8-171">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="0c5b8-171">easActivationDateTime</span></span>|<span data-ttu-id="0c5b8-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c5b8-172">DateTimeOffset</span></span>|<span data-ttu-id="0c5b8-173">Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät</span><span class="sxs-lookup"><span data-stu-id="0c5b8-173">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="0c5b8-174">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="0c5b8-174">azureADRegistered</span></span>|<span data-ttu-id="0c5b8-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c5b8-175">Boolean</span></span>|<span data-ttu-id="0c5b8-176">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-176">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="0c5b8-177">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="0c5b8-177">deviceEnrollmentType</span></span>|<span data-ttu-id="0c5b8-178">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-178">String</span></span>|<span data-ttu-id="0c5b8-179">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-179">Enrollment type of the device.</span></span> <span data-ttu-id="0c5b8-180">Mögliche Werte sind: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin` und `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-180">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="0c5b8-181">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="0c5b8-181">activationLockBypassCode</span></span>|<span data-ttu-id="0c5b8-182">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-182">String</span></span>|<span data-ttu-id="0c5b8-183">Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht</span><span class="sxs-lookup"><span data-stu-id="0c5b8-183">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="0c5b8-184">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0c5b8-184">emailAddress</span></span>|<span data-ttu-id="0c5b8-185">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-185">String</span></span>|<span data-ttu-id="0c5b8-186">E-Mail-Adressen des Benutzers, der dem Gerät zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="0c5b8-186">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="0c5b8-187">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="0c5b8-187">azureADDeviceId</span></span>|<span data-ttu-id="0c5b8-188">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-188">String</span></span>|<span data-ttu-id="0c5b8-189">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-189">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="0c5b8-190">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-190">Read only.</span></span>|
|<span data-ttu-id="0c5b8-191">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0c5b8-191">deviceRegistrationState</span></span>|<span data-ttu-id="0c5b8-192">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-192">String</span></span>|<span data-ttu-id="0c5b8-193">Registrierungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-193">Device registration state.</span></span> <span data-ttu-id="0c5b8-194">Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-194">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`.</span></span>|
|<span data-ttu-id="0c5b8-195">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="0c5b8-195">deviceCategoryDisplayName</span></span>|<span data-ttu-id="0c5b8-196">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-196">String</span></span>|<span data-ttu-id="0c5b8-197">Anzeigename der Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="0c5b8-197">Device category display name</span></span>|
|<span data-ttu-id="0c5b8-198">isSupervised</span><span class="sxs-lookup"><span data-stu-id="0c5b8-198">isSupervised</span></span>|<span data-ttu-id="0c5b8-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c5b8-199">Boolean</span></span>|<span data-ttu-id="0c5b8-200">Überwachungsstatus des Geräts</span><span class="sxs-lookup"><span data-stu-id="0c5b8-200">Device supervised status</span></span>|
|<span data-ttu-id="0c5b8-201">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0c5b8-201">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="0c5b8-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c5b8-202">DateTimeOffset</span></span>|<span data-ttu-id="0c5b8-203">Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange</span><span class="sxs-lookup"><span data-stu-id="0c5b8-203">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="0c5b8-204">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="0c5b8-204">exchangeAccessState</span></span>|<span data-ttu-id="0c5b8-205">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-205">String</span></span>|<span data-ttu-id="0c5b8-206">Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-206">The Access State of the device in Exchange.</span></span> <span data-ttu-id="0c5b8-207">Mögliche Werte sind: `none`, `unknown`, `allowed`, `blocked` und `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-207">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="0c5b8-208">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="0c5b8-208">exchangeAccessStateReason</span></span>|<span data-ttu-id="0c5b8-209">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-209">String</span></span>|<span data-ttu-id="0c5b8-210">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-210">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="0c5b8-211">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-211">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="0c5b8-212">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="0c5b8-212">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="0c5b8-213">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-213">String</span></span>|<span data-ttu-id="0c5b8-214">URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät</span><span class="sxs-lookup"><span data-stu-id="0c5b8-214">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="0c5b8-215">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0c5b8-215">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="0c5b8-216">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-216">String</span></span>|<span data-ttu-id="0c5b8-217">Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen</span><span class="sxs-lookup"><span data-stu-id="0c5b8-217">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="0c5b8-218">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="0c5b8-218">isEncrypted</span></span>|<span data-ttu-id="0c5b8-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c5b8-219">Boolean</span></span>|<span data-ttu-id="0c5b8-220">Verschlüsselungsstatus des Geräts</span><span class="sxs-lookup"><span data-stu-id="0c5b8-220">Device encryption status</span></span>|
|<span data-ttu-id="0c5b8-221">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0c5b8-221">userPrincipalName</span></span>|<span data-ttu-id="0c5b8-222">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-222">String</span></span>|<span data-ttu-id="0c5b8-223">Benutzerprinzipalname für das Gerät</span><span class="sxs-lookup"><span data-stu-id="0c5b8-223">Device user principal name</span></span>|
|<span data-ttu-id="0c5b8-224">model</span><span class="sxs-lookup"><span data-stu-id="0c5b8-224">model</span></span>|<span data-ttu-id="0c5b8-225">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-225">String</span></span>|<span data-ttu-id="0c5b8-226">Modell des Geräts</span><span class="sxs-lookup"><span data-stu-id="0c5b8-226">Model of the device</span></span>|
|<span data-ttu-id="0c5b8-227">manufacturer</span><span class="sxs-lookup"><span data-stu-id="0c5b8-227">Camera manufacturer.</span></span>|<span data-ttu-id="0c5b8-228">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-228">String</span></span>|<span data-ttu-id="0c5b8-229">Hersteller des Geräts</span><span class="sxs-lookup"><span data-stu-id="0c5b8-229">Manufacturer of the device</span></span>|
|<span data-ttu-id="0c5b8-230">imei</span><span class="sxs-lookup"><span data-stu-id="0c5b8-230">imei</span></span>|<span data-ttu-id="0c5b8-231">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-231">String</span></span>|<span data-ttu-id="0c5b8-232">IMEI</span><span class="sxs-lookup"><span data-stu-id="0c5b8-232">IMEI</span></span>|
|<span data-ttu-id="0c5b8-233">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0c5b8-233">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="0c5b8-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c5b8-234">DateTimeOffset</span></span>|<span data-ttu-id="0c5b8-235">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="0c5b8-235">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="0c5b8-236">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0c5b8-236">serialNumber</span></span>|<span data-ttu-id="0c5b8-237">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-237">String</span></span>|<span data-ttu-id="0c5b8-238">Seriennummer</span><span class="sxs-lookup"><span data-stu-id="0c5b8-238">SerialNumber Property</span></span>|
|<span data-ttu-id="0c5b8-239">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="0c5b8-239">PhoneNumber</span></span>|<span data-ttu-id="0c5b8-240">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-240">String</span></span>|<span data-ttu-id="0c5b8-241">Telefonnummer des Geräts</span><span class="sxs-lookup"><span data-stu-id="0c5b8-241">Phone number of the device</span></span>|
|<span data-ttu-id="0c5b8-242">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="0c5b8-242">androidSecurityPatchLevel</span></span>|<span data-ttu-id="0c5b8-243">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-243">String</span></span>|<span data-ttu-id="0c5b8-244">Android-Sicherheitspatchlevel</span><span class="sxs-lookup"><span data-stu-id="0c5b8-244">Android security patch level</span></span>|
|<span data-ttu-id="0c5b8-245">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0c5b8-245">userDisplayName</span></span>|<span data-ttu-id="0c5b8-246">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-246">String</span></span>|<span data-ttu-id="0c5b8-247">Anzeigename des Benutzers</span><span class="sxs-lookup"><span data-stu-id="0c5b8-247">user display name</span></span>|
|<span data-ttu-id="0c5b8-248">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0c5b8-248">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="0c5b8-249">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0c5b8-249">configurationManagerClientEnabledFeatures</span></span>](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="0c5b8-250">Aktivierte Funktionen des Konfigurations-Manager-Clients</span><span class="sxs-lookup"><span data-stu-id="0c5b8-250">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="0c5b8-251">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="0c5b8-251">wiFiMacAddress</span></span>|<span data-ttu-id="0c5b8-252">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-252">String</span></span>|<span data-ttu-id="0c5b8-253">WLAN-MAC</span><span class="sxs-lookup"><span data-stu-id="0c5b8-253">Wi-Fi MAC</span></span>|
|<span data-ttu-id="0c5b8-254">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0c5b8-254">deviceHealthAttestationState</span></span>|[<span data-ttu-id="0c5b8-255">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0c5b8-255">deviceHealthAttestationState</span></span>](../resources/intune_devices_devicehealthattestationstate.md)|<span data-ttu-id="0c5b8-256">Status des Integritätsnachweises für Geräte</span><span class="sxs-lookup"><span data-stu-id="0c5b8-256">The device health attestation state.</span></span>|
|<span data-ttu-id="0c5b8-257">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="0c5b8-257">subscriberCarrier</span></span>|<span data-ttu-id="0c5b8-258">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-258">String</span></span>|<span data-ttu-id="0c5b8-259">Netzbetreiber des Abonnenten</span><span class="sxs-lookup"><span data-stu-id="0c5b8-259">Subscriber Carrier</span></span>|
|<span data-ttu-id="0c5b8-260">meid</span><span class="sxs-lookup"><span data-stu-id="0c5b8-260">meid</span></span>|<span data-ttu-id="0c5b8-261">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-261">String</span></span>|<span data-ttu-id="0c5b8-262">MEID</span><span class="sxs-lookup"><span data-stu-id="0c5b8-262">MEID</span></span>|
|<span data-ttu-id="0c5b8-263">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0c5b8-263">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="0c5b8-264">Int64</span><span class="sxs-lookup"><span data-stu-id="0c5b8-264">Int64</span></span>|<span data-ttu-id="0c5b8-265">Gesamtspeicher in Byte</span><span class="sxs-lookup"><span data-stu-id="0c5b8-265">Total Storage in Bytes</span></span>|
|<span data-ttu-id="0c5b8-266">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="0c5b8-266">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="0c5b8-267">Int64</span><span class="sxs-lookup"><span data-stu-id="0c5b8-267">Int64</span></span>|<span data-ttu-id="0c5b8-268">Freier Speicher in Byte</span><span class="sxs-lookup"><span data-stu-id="0c5b8-268">Free Storage in Bytes</span></span>|
|<span data-ttu-id="0c5b8-269">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="0c5b8-269">managedDeviceName</span></span>|<span data-ttu-id="0c5b8-270">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-270">String</span></span>|<span data-ttu-id="0c5b8-271">Automatisch generierter Name zur Identifizierung des Geräts.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-271">Automatically generated name to identify a device.</span></span> <span data-ttu-id="0c5b8-272">Kann mit einem benutzerfreundlichen Namen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-272">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="0c5b8-273">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="0c5b8-273">partnerReportedThreatState</span></span>|<span data-ttu-id="0c5b8-274">String</span><span class="sxs-lookup"><span data-stu-id="0c5b8-274">String</span></span>|<span data-ttu-id="0c5b8-275">Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-275">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="0c5b8-276">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-276">Read Only</span></span> <span data-ttu-id="0c5b8-277">Mögliche Werte sind: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-277">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`.</span></span>|



## <a name="response"></a><span data-ttu-id="0c5b8-278">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c5b8-278">Response</span></span>
<span data-ttu-id="0c5b8-279">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedDevice](../resources/intune_devices_manageddevice.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-279">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c5b8-280">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0c5b8-280">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c5b8-281">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c5b8-281">Request</span></span>
<span data-ttu-id="0c5b8-282">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-282">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 4616

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated"
}
```

### <a name="response"></a><span data-ttu-id="0c5b8-283">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c5b8-283">Response</span></span>
<span data-ttu-id="0c5b8-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4665

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated"
}
```



