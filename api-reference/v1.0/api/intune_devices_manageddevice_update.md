# <a name="update-manageddevice"></a><span data-ttu-id="4d996-101">Aktualisieren von „managedDevice“</span><span class="sxs-lookup"><span data-stu-id="4d996-101">Update managedDevice</span></span>

> <span data-ttu-id="4d996-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4d996-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d996-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDevice](../resources/intune_devices_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4d996-103">Update the properties of a [calendar](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d996-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4d996-104">Prerequisites</span></span>
<span data-ttu-id="4d996-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d996-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4d996-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d996-107">Permission type</span></span>|<span data-ttu-id="4d996-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d996-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d996-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d996-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4d996-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d996-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4d996-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d996-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d996-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d996-112">Not supported.</span></span>|
|<span data-ttu-id="4d996-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d996-113">Application</span></span>|<span data-ttu-id="4d996-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d996-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d996-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d996-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="4d996-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d996-116">Request headers</span></span>
|<span data-ttu-id="4d996-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4d996-117">Header</span></span>|<span data-ttu-id="4d996-118">Wert</span><span class="sxs-lookup"><span data-stu-id="4d996-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d996-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d996-119">Authorization</span></span>|<span data-ttu-id="4d996-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d996-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4d996-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4d996-121">Accept</span></span>|<span data-ttu-id="4d996-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4d996-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d996-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d996-123">Request body</span></span>
<span data-ttu-id="4d996-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDevice](../resources/intune_devices_manageddevice.md) an.</span><span class="sxs-lookup"><span data-stu-id="4d996-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_devices_manageddevice.md) object.</span></span>

<span data-ttu-id="4d996-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDevice](../resources/intune_devices_manageddevice.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="4d996-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="4d996-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d996-126">Property</span></span>|<span data-ttu-id="4d996-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4d996-127">Type</span></span>|<span data-ttu-id="4d996-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d996-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d996-129">id</span><span class="sxs-lookup"><span data-stu-id="4d996-129">id</span></span>|<span data-ttu-id="4d996-130">String</span><span class="sxs-lookup"><span data-stu-id="4d996-130">String</span></span>|<span data-ttu-id="4d996-131">Eindeutiger Bezeichner für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="4d996-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="4d996-132">userId</span><span class="sxs-lookup"><span data-stu-id="4d996-132">userID</span></span>|<span data-ttu-id="4d996-133">String</span><span class="sxs-lookup"><span data-stu-id="4d996-133">String</span></span>|<span data-ttu-id="4d996-134">Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="4d996-134">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="4d996-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="4d996-135">deviceName</span></span>|<span data-ttu-id="4d996-136">String</span><span class="sxs-lookup"><span data-stu-id="4d996-136">String</span></span>|<span data-ttu-id="4d996-137">Name des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="4d996-137">Name of the device</span></span>|
|<span data-ttu-id="4d996-138">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="4d996-138">deviceActionResults</span></span>|<span data-ttu-id="4d996-139">Collection von Objekten des Typs [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4d996-139">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) collection</span></span>|<span data-ttu-id="4d996-140">Liste von Objekten des Typs „ComplexType deviceActionResult“.
</span><span class="sxs-lookup"><span data-stu-id="4d996-140">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="4d996-141">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="4d996-141">enrolledDateTime</span></span>|<span data-ttu-id="4d996-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d996-142">DateTimeOffset</span></span>|<span data-ttu-id="4d996-143">Datum und Uhrzeit der Geräteregistrierung.
</span><span class="sxs-lookup"><span data-stu-id="4d996-143">Enrollment time of the device.</span></span>|
|<span data-ttu-id="4d996-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4d996-144">lastSyncDateTime</span></span>|<span data-ttu-id="4d996-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d996-145">DateTimeOffset</span></span>|<span data-ttu-id="4d996-146">Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
</span><span class="sxs-lookup"><span data-stu-id="4d996-146">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="4d996-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="4d996-147">operatingSystem</span></span>|<span data-ttu-id="4d996-148">String</span><span class="sxs-lookup"><span data-stu-id="4d996-148">String</span></span>|<span data-ttu-id="4d996-149">Betriebssystem des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4d996-149">Operating system of the device.</span></span> <span data-ttu-id="4d996-150">Windows, iOS usw.</span><span class="sxs-lookup"><span data-stu-id="4d996-150">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="4d996-151">complianceState</span><span class="sxs-lookup"><span data-stu-id="4d996-151">complianceState</span></span>|<span data-ttu-id="4d996-152">String</span><span class="sxs-lookup"><span data-stu-id="4d996-152">String</span></span>|<span data-ttu-id="4d996-153">Konformitätsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4d996-153">Compliance state of the device.</span></span> <span data-ttu-id="4d996-154">Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.</span><span class="sxs-lookup"><span data-stu-id="4d996-154">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="4d996-155">jailBroken</span><span class="sxs-lookup"><span data-stu-id="4d996-155">jailBroken</span></span>|<span data-ttu-id="4d996-156">String</span><span class="sxs-lookup"><span data-stu-id="4d996-156">String</span></span>|<span data-ttu-id="4d996-157">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="4d996-157">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="4d996-158">managementAgent</span><span class="sxs-lookup"><span data-stu-id="4d996-158">managementAgent</span></span>|<span data-ttu-id="4d996-159">String</span><span class="sxs-lookup"><span data-stu-id="4d996-159">String</span></span>|<span data-ttu-id="4d996-160">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4d996-160">Management channel of the device.</span></span> <span data-ttu-id="4d996-161">Intune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf` und `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="4d996-161">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="4d996-162">osVersion</span><span class="sxs-lookup"><span data-stu-id="4d996-162">osVersion</span></span>|<span data-ttu-id="4d996-163">String</span><span class="sxs-lookup"><span data-stu-id="4d996-163">String</span></span>|<span data-ttu-id="4d996-164">Auf dem Gerät installierte Betriebssystemversion.
</span><span class="sxs-lookup"><span data-stu-id="4d996-164">Operating system version of the device.</span></span>|
|<span data-ttu-id="4d996-165">easActivated</span><span class="sxs-lookup"><span data-stu-id="4d996-165">easActivated</span></span>|<span data-ttu-id="4d996-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d996-166">Boolean</span></span>|<span data-ttu-id="4d996-167">Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="4d996-167">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="4d996-168">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="4d996-168">easDeviceId</span></span>|<span data-ttu-id="4d996-169">String</span><span class="sxs-lookup"><span data-stu-id="4d996-169">String</span></span>|<span data-ttu-id="4d996-170">Exchange ActiveSync-ID des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="4d996-170">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="4d996-171">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="4d996-171">easActivationDateTime</span></span>|<span data-ttu-id="4d996-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d996-172">DateTimeOffset</span></span>|<span data-ttu-id="4d996-173">Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="4d996-173">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="4d996-174">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="4d996-174">azureADRegistered</span></span>|<span data-ttu-id="4d996-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d996-175">Boolean</span></span>|<span data-ttu-id="4d996-176">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="4d996-176">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="4d996-177">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="4d996-177">deviceEnrollmentType</span></span>|<span data-ttu-id="4d996-178">String</span><span class="sxs-lookup"><span data-stu-id="4d996-178">String</span></span>|<span data-ttu-id="4d996-179">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4d996-179">Enrollment type of the device.</span></span> <span data-ttu-id="4d996-180">Mögliche Werte sind: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin` und `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="4d996-180">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="4d996-181">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="4d996-181">activationLockBypassCode</span></span>|<span data-ttu-id="4d996-182">String</span><span class="sxs-lookup"><span data-stu-id="4d996-182">String</span></span>|<span data-ttu-id="4d996-183">Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht</span><span class="sxs-lookup"><span data-stu-id="4d996-183">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="4d996-184">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4d996-184">emailAddress</span></span>|<span data-ttu-id="4d996-185">String</span><span class="sxs-lookup"><span data-stu-id="4d996-185">String</span></span>|<span data-ttu-id="4d996-186">E-Mail-Adressen des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="4d996-186">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="4d996-187">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="4d996-187">azureADDeviceId</span></span>|<span data-ttu-id="4d996-188">String</span><span class="sxs-lookup"><span data-stu-id="4d996-188">String</span></span>|<span data-ttu-id="4d996-189">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="4d996-189">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="4d996-190">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4d996-190">Read only.</span></span>|
|<span data-ttu-id="4d996-191">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="4d996-191">deviceRegistrationState</span></span>|<span data-ttu-id="4d996-192">String</span><span class="sxs-lookup"><span data-stu-id="4d996-192">String</span></span>|<span data-ttu-id="4d996-193">Registrierungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4d996-193">Device registration state.</span></span> <span data-ttu-id="4d996-194">Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4d996-194">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`.</span></span>|
|<span data-ttu-id="4d996-195">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="4d996-195">deviceCategoryDisplayName</span></span>|<span data-ttu-id="4d996-196">String</span><span class="sxs-lookup"><span data-stu-id="4d996-196">String</span></span>|<span data-ttu-id="4d996-197">Anzeigename der Gerätekategorie.
</span><span class="sxs-lookup"><span data-stu-id="4d996-197">Device category display name</span></span>|
|<span data-ttu-id="4d996-198">isSupervised</span><span class="sxs-lookup"><span data-stu-id="4d996-198">isSupervised</span></span>|<span data-ttu-id="4d996-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d996-199">Boolean</span></span>|<span data-ttu-id="4d996-200">Überwachungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="4d996-200">Device supervised status</span></span>|
|<span data-ttu-id="4d996-201">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4d996-201">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="4d996-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d996-202">DateTimeOffset</span></span>|<span data-ttu-id="4d996-203">Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange</span><span class="sxs-lookup"><span data-stu-id="4d996-203">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="4d996-204">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="4d996-204">exchangeAccessState</span></span>|<span data-ttu-id="4d996-205">String</span><span class="sxs-lookup"><span data-stu-id="4d996-205">String</span></span>|<span data-ttu-id="4d996-206">Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d996-206">The Access State of the device in Exchange.</span></span> <span data-ttu-id="4d996-207">Mögliche Werte sind: `none`, `unknown`, `allowed`, `blocked` und `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="4d996-207">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="4d996-208">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="4d996-208">exchangeAccessStateReason</span></span>|<span data-ttu-id="4d996-209">String</span><span class="sxs-lookup"><span data-stu-id="4d996-209">String</span></span>|<span data-ttu-id="4d996-210">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d996-210">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="4d996-211">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="4d996-211">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="4d996-212">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="4d996-212">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="4d996-213">String</span><span class="sxs-lookup"><span data-stu-id="4d996-213">String</span></span>|<span data-ttu-id="4d996-214">URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
</span><span class="sxs-lookup"><span data-stu-id="4d996-214">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="4d996-215">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="4d996-215">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="4d996-216">String</span><span class="sxs-lookup"><span data-stu-id="4d996-216">String</span></span>|<span data-ttu-id="4d996-217">Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
</span><span class="sxs-lookup"><span data-stu-id="4d996-217">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="4d996-218">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="4d996-218">isEncrypted</span></span>|<span data-ttu-id="4d996-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d996-219">Boolean</span></span>|<span data-ttu-id="4d996-220">Verschlüsselungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="4d996-220">Device encryption status</span></span>|
|<span data-ttu-id="4d996-221">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4d996-221">userPrincipalName</span></span>|<span data-ttu-id="4d996-222">String</span><span class="sxs-lookup"><span data-stu-id="4d996-222">String</span></span>|<span data-ttu-id="4d996-223">Benutzerprinzipalname für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="4d996-223">Device user principal name</span></span>|
|<span data-ttu-id="4d996-224">model</span><span class="sxs-lookup"><span data-stu-id="4d996-224">model</span></span>|<span data-ttu-id="4d996-225">String</span><span class="sxs-lookup"><span data-stu-id="4d996-225">String</span></span>|<span data-ttu-id="4d996-226">Modell des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="4d996-226">Model of the device</span></span>|
|<span data-ttu-id="4d996-227">manufacturer</span><span class="sxs-lookup"><span data-stu-id="4d996-227">Camera manufacturer.</span></span>|<span data-ttu-id="4d996-228">String</span><span class="sxs-lookup"><span data-stu-id="4d996-228">String</span></span>|<span data-ttu-id="4d996-229">Hersteller des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="4d996-229">Manufacturer of the device</span></span>|
|<span data-ttu-id="4d996-230">imei</span><span class="sxs-lookup"><span data-stu-id="4d996-230">imei</span></span>|<span data-ttu-id="4d996-231">String</span><span class="sxs-lookup"><span data-stu-id="4d996-231">String</span></span>|<span data-ttu-id="4d996-232">IMEI</span><span class="sxs-lookup"><span data-stu-id="4d996-232">IMEI</span></span>|
|<span data-ttu-id="4d996-233">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4d996-233">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="4d996-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d996-234">DateTimeOffset</span></span>|<span data-ttu-id="4d996-235">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität.
</span><span class="sxs-lookup"><span data-stu-id="4d996-235">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="4d996-236">serialNumber</span><span class="sxs-lookup"><span data-stu-id="4d996-236">serialNumber</span></span>|<span data-ttu-id="4d996-237">String</span><span class="sxs-lookup"><span data-stu-id="4d996-237">String</span></span>|<span data-ttu-id="4d996-238">Seriennummer.
</span><span class="sxs-lookup"><span data-stu-id="4d996-238">SerialNumber Property</span></span>|
|<span data-ttu-id="4d996-239">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="4d996-239">PhoneNumber</span></span>|<span data-ttu-id="4d996-240">String</span><span class="sxs-lookup"><span data-stu-id="4d996-240">String</span></span>|<span data-ttu-id="4d996-241">Telefonnummer des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="4d996-241">Phone number of the device</span></span>|
|<span data-ttu-id="4d996-242">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="4d996-242">androidSecurityPatchLevel</span></span>|<span data-ttu-id="4d996-243">String</span><span class="sxs-lookup"><span data-stu-id="4d996-243">String</span></span>|<span data-ttu-id="4d996-244">Android-Sicherheitspatchlevel.
</span><span class="sxs-lookup"><span data-stu-id="4d996-244">Android security patch level</span></span>|
|<span data-ttu-id="4d996-245">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4d996-245">userDisplayName</span></span>|<span data-ttu-id="4d996-246">String</span><span class="sxs-lookup"><span data-stu-id="4d996-246">String</span></span>|<span data-ttu-id="4d996-247">Anzeigename des Benutzers.
</span><span class="sxs-lookup"><span data-stu-id="4d996-247">user display name</span></span>|
|<span data-ttu-id="4d996-248">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="4d996-248">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="4d996-249">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="4d996-249">configurationManagerClientEnabledFeatures</span></span>](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="4d996-250">Aktivierte Funktionen des Konfigurations-Manager-Clients.
</span><span class="sxs-lookup"><span data-stu-id="4d996-250">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="4d996-251">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="4d996-251">wiFiMacAddress</span></span>|<span data-ttu-id="4d996-252">String</span><span class="sxs-lookup"><span data-stu-id="4d996-252">String</span></span>|<span data-ttu-id="4d996-253">WLAN-MAC</span><span class="sxs-lookup"><span data-stu-id="4d996-253">Wi-Fi MAC</span></span>|
|<span data-ttu-id="4d996-254">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="4d996-254">deviceHealthAttestationState</span></span>|[<span data-ttu-id="4d996-255">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="4d996-255">deviceHealthAttestationState</span></span>](../resources/intune_devices_devicehealthattestationstate.md)|<span data-ttu-id="4d996-256">Status des Integritätsnachweises für Geräte.
</span><span class="sxs-lookup"><span data-stu-id="4d996-256">The device health attestation state.</span></span>|
|<span data-ttu-id="4d996-257">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="4d996-257">subscriberCarrier</span></span>|<span data-ttu-id="4d996-258">String</span><span class="sxs-lookup"><span data-stu-id="4d996-258">String</span></span>|<span data-ttu-id="4d996-259">Netzbetreiber des Abonnenten.
</span><span class="sxs-lookup"><span data-stu-id="4d996-259">Subscriber Carrier</span></span>|
|<span data-ttu-id="4d996-260">meid</span><span class="sxs-lookup"><span data-stu-id="4d996-260">meid</span></span>|<span data-ttu-id="4d996-261">String</span><span class="sxs-lookup"><span data-stu-id="4d996-261">String</span></span>|<span data-ttu-id="4d996-262">MEID</span><span class="sxs-lookup"><span data-stu-id="4d996-262">MEID</span></span>|
|<span data-ttu-id="4d996-263">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="4d996-263">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="4d996-264">Int64</span><span class="sxs-lookup"><span data-stu-id="4d996-264">Int64</span></span>|<span data-ttu-id="4d996-265">Gesamtspeicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="4d996-265">Total Storage in Bytes</span></span>|
|<span data-ttu-id="4d996-266">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="4d996-266">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="4d996-267">Int64</span><span class="sxs-lookup"><span data-stu-id="4d996-267">Int64</span></span>|<span data-ttu-id="4d996-268">Freier Speicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="4d996-268">Free Storage in Bytes</span></span>|
|<span data-ttu-id="4d996-269">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="4d996-269">managedDeviceName</span></span>|<span data-ttu-id="4d996-270">String</span><span class="sxs-lookup"><span data-stu-id="4d996-270">String</span></span>|<span data-ttu-id="4d996-271">Automatisch generierter Name zur Identifizierung des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4d996-271">Automatically generated name to identify a device.</span></span> <span data-ttu-id="4d996-272">Kann mit einem benutzerfreundlichen Namen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="4d996-272">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="4d996-273">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="4d996-273">partnerReportedThreatState</span></span>|<span data-ttu-id="4d996-274">String</span><span class="sxs-lookup"><span data-stu-id="4d996-274">String</span></span>|<span data-ttu-id="4d996-275">Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen.</span><span class="sxs-lookup"><span data-stu-id="4d996-275">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="4d996-276">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4d996-276">Read Only</span></span> <span data-ttu-id="4d996-277">Mögliche Werte sind: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity` und `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="4d996-277">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`.</span></span>|



## <a name="response"></a><span data-ttu-id="4d996-278">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d996-278">Response</span></span>
<span data-ttu-id="4d996-279">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDevice](../resources/intune_devices_manageddevice.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4d996-279">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d996-280">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d996-280">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d996-281">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d996-281">Request</span></span>
<span data-ttu-id="4d996-282">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d996-282">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 4564

{
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

### <a name="response"></a><span data-ttu-id="4d996-283">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d996-283">Response</span></span>
<span data-ttu-id="4d996-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d996-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



