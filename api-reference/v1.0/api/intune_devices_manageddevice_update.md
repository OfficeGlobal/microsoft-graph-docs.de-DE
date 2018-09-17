# <a name="update-manageddevice"></a><span data-ttu-id="9eef9-101">Aktualisieren von „managedDevice“</span><span class="sxs-lookup"><span data-stu-id="9eef9-101">Update managedDevice</span></span>

> <span data-ttu-id="9eef9-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9eef9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9eef9-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDevice](../resources/intune_devices_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="9eef9-103">Update the properties of a [managedDevice](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9eef9-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9eef9-104">Prerequisites</span></span>
<span data-ttu-id="9eef9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9eef9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9eef9-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9eef9-107">Permission type</span></span>|<span data-ttu-id="9eef9-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9eef9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9eef9-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9eef9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9eef9-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9eef9-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9eef9-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9eef9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9eef9-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9eef9-112">Not supported.</span></span>|
|<span data-ttu-id="9eef9-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9eef9-113">Application</span></span>|<span data-ttu-id="9eef9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9eef9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9eef9-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9eef9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="9eef9-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9eef9-116">Request headers</span></span>
|<span data-ttu-id="9eef9-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9eef9-117">Header</span></span>|<span data-ttu-id="9eef9-118">Wert</span><span class="sxs-lookup"><span data-stu-id="9eef9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9eef9-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9eef9-119">Authorization</span></span>|<span data-ttu-id="9eef9-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9eef9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9eef9-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="9eef9-121">Accept</span></span>|<span data-ttu-id="9eef9-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="9eef9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9eef9-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9eef9-123">Request body</span></span>
<span data-ttu-id="9eef9-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDevice](../resources/intune_devices_manageddevice.md) an.</span><span class="sxs-lookup"><span data-stu-id="9eef9-124">In the request body, supply a JSON representation for the [managedDevice](../resources/intune_devices_manageddevice.md) object.</span></span>

<span data-ttu-id="9eef9-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDevice](../resources/intune_devices_manageddevice.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="9eef9-125">The following table shows the properties that are required when you create the [managedDevice](../resources/intune_devices_manageddevice.md).</span></span>

|<span data-ttu-id="9eef9-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9eef9-126">Property</span></span>|<span data-ttu-id="9eef9-127">Typ</span><span class="sxs-lookup"><span data-stu-id="9eef9-127">Type</span></span>|<span data-ttu-id="9eef9-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9eef9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9eef9-129">ID</span><span class="sxs-lookup"><span data-stu-id="9eef9-129">id</span></span>|<span data-ttu-id="9eef9-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-130">String</span></span>|<span data-ttu-id="9eef9-131">Eindeutiger Bezeichner für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="9eef9-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="9eef9-132">userId</span><span class="sxs-lookup"><span data-stu-id="9eef9-132">userId</span></span>|<span data-ttu-id="9eef9-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-133">String</span></span>|<span data-ttu-id="9eef9-134">Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="9eef9-134">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="9eef9-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="9eef9-135">deviceName</span></span>|<span data-ttu-id="9eef9-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-136">String</span></span>|<span data-ttu-id="9eef9-137">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="9eef9-137">Name of the device</span></span>|
|<span data-ttu-id="9eef9-138">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="9eef9-138">managedDeviceOwnerType</span></span>|[<span data-ttu-id="9eef9-139">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="9eef9-139">managedDeviceOwnerType</span></span>](../resources/intune_devices_manageddeviceownertype.md)|<span data-ttu-id="9eef9-p102">Besitz des Geräts. Kann "Unternehmen" oder "Privat" sein. Mögliche Werte: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="9eef9-p102">Ownership of the device. Can be 'company' or 'personal'. The possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="9eef9-143">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="9eef9-143">deviceActionResults</span></span>|<span data-ttu-id="9eef9-144">Collection von Objekten des Typs [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9eef9-144">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) collection</span></span>|<span data-ttu-id="9eef9-145">Liste von Objekten des Typs „ComplexType deviceActionResult“.</span><span class="sxs-lookup"><span data-stu-id="9eef9-145">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="9eef9-146">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="9eef9-146">enrolledDateTime</span></span>|<span data-ttu-id="9eef9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9eef9-147">DateTimeOffset</span></span>|<span data-ttu-id="9eef9-148">Datum und Uhrzeit der Geräteregistrierung.</span><span class="sxs-lookup"><span data-stu-id="9eef9-148">Enrollment time of the device.</span></span>|
|<span data-ttu-id="9eef9-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9eef9-149">lastSyncDateTime</span></span>|<span data-ttu-id="9eef9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9eef9-150">DateTimeOffset</span></span>|<span data-ttu-id="9eef9-151">Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.</span><span class="sxs-lookup"><span data-stu-id="9eef9-151">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="9eef9-152">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="9eef9-152">operatingSystem</span></span>|<span data-ttu-id="9eef9-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-153">String</span></span>|<span data-ttu-id="9eef9-154">Betriebssystem des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9eef9-154">Operating system of the device.</span></span> <span data-ttu-id="9eef9-155">Windows, iOS usw.</span><span class="sxs-lookup"><span data-stu-id="9eef9-155">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="9eef9-156">complianceState</span><span class="sxs-lookup"><span data-stu-id="9eef9-156">complianceState</span></span>|[<span data-ttu-id="9eef9-157">complianceState</span><span class="sxs-lookup"><span data-stu-id="9eef9-157">complianceState</span></span>](../resources/intune_devices_compliancestate.md)|<span data-ttu-id="9eef9-p104">Compliance-Zustand des Geräts. Mögliche Werte: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="9eef9-p104">Compliance state of the device. The possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="9eef9-160">jailBroken</span><span class="sxs-lookup"><span data-stu-id="9eef9-160">jailBroken</span></span>|<span data-ttu-id="9eef9-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-161">String</span></span>|<span data-ttu-id="9eef9-162">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="9eef9-162">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="9eef9-163">managementAgent</span><span class="sxs-lookup"><span data-stu-id="9eef9-163">managementAgent</span></span>|[<span data-ttu-id="9eef9-164">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="9eef9-164">managementAgentType</span></span>](../resources/intune_devices_managementagenttype.md)|<span data-ttu-id="9eef9-p105">Verwaltungskanal des Geräts. Intune, EAS usw. Mögliche Werte: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="9eef9-p105">Management channel of the device. Intune, EAS, etc. The possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="9eef9-167">osVersion</span><span class="sxs-lookup"><span data-stu-id="9eef9-167">osVersion</span></span>|<span data-ttu-id="9eef9-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-168">String</span></span>|<span data-ttu-id="9eef9-169">Auf dem Gerät installierte Betriebssystemversion.</span><span class="sxs-lookup"><span data-stu-id="9eef9-169">Operating system version of the device.</span></span>|
|<span data-ttu-id="9eef9-170">easActivated</span><span class="sxs-lookup"><span data-stu-id="9eef9-170">easActivated</span></span>|<span data-ttu-id="9eef9-171">boolesch</span><span class="sxs-lookup"><span data-stu-id="9eef9-171">Boolean</span></span>|<span data-ttu-id="9eef9-172">Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="9eef9-172">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="9eef9-173">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="9eef9-173">easDeviceId</span></span>|<span data-ttu-id="9eef9-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-174">String</span></span>|<span data-ttu-id="9eef9-175">Exchange ActiveSync-ID des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9eef9-175">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="9eef9-176">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="9eef9-176">easActivationDateTime</span></span>|<span data-ttu-id="9eef9-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9eef9-177">DateTimeOffset</span></span>|<span data-ttu-id="9eef9-178">Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="9eef9-178">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="9eef9-179">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="9eef9-179">azureADRegistered</span></span>|<span data-ttu-id="9eef9-180">boolesch</span><span class="sxs-lookup"><span data-stu-id="9eef9-180">Boolean</span></span>|<span data-ttu-id="9eef9-181">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="9eef9-181">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="9eef9-182">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="9eef9-182">deviceEnrollmentType</span></span>|[<span data-ttu-id="9eef9-183">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="9eef9-183">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="9eef9-p106">Typ der Registrierung des Geräts. Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="9eef9-p106">Enrollment type of the device. The possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="9eef9-186">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="9eef9-186">activationLockBypassCode</span></span>|<span data-ttu-id="9eef9-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-187">String</span></span>|<span data-ttu-id="9eef9-188">Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht</span><span class="sxs-lookup"><span data-stu-id="9eef9-188">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="9eef9-189">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9eef9-189">emailAddress</span></span>|<span data-ttu-id="9eef9-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-190">String</span></span>|<span data-ttu-id="9eef9-191">E-Mail-Adressen des Benutzers, der dem Gerät zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="9eef9-191">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="9eef9-192">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="9eef9-192">azureADDeviceId</span></span>|<span data-ttu-id="9eef9-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-193">String</span></span>|<span data-ttu-id="9eef9-194">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="9eef9-194">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="9eef9-195">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9eef9-195">Read only.</span></span>|
|<span data-ttu-id="9eef9-196">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="9eef9-196">deviceRegistrationState</span></span>|[<span data-ttu-id="9eef9-197">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="9eef9-197">deviceRegistrationState</span></span>](../resources/intune_devices_deviceregistrationstate.md)|<span data-ttu-id="9eef9-p108">Registrierungsstatus des Geräts. Mögliche Werte: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="9eef9-p108">Device registration state. The possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="9eef9-200">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="9eef9-200">deviceCategoryDisplayName</span></span>|<span data-ttu-id="9eef9-201">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-201">String</span></span>|<span data-ttu-id="9eef9-202">Anzeigename der Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="9eef9-202">Device category display name</span></span>|
|<span data-ttu-id="9eef9-203">isSupervised</span><span class="sxs-lookup"><span data-stu-id="9eef9-203">isSupervised</span></span>|<span data-ttu-id="9eef9-204">boolesch</span><span class="sxs-lookup"><span data-stu-id="9eef9-204">Boolean</span></span>|<span data-ttu-id="9eef9-205">Überwachungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9eef9-205">Device supervised status</span></span>|
|<span data-ttu-id="9eef9-206">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9eef9-206">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="9eef9-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9eef9-207">DateTimeOffset</span></span>|<span data-ttu-id="9eef9-208">Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange</span><span class="sxs-lookup"><span data-stu-id="9eef9-208">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="9eef9-209">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="9eef9-209">exchangeAccessState</span></span>|[<span data-ttu-id="9eef9-210">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="9eef9-210">deviceManagementExchangeAccessState</span></span>](../resources/intune_devices_devicemanagementexchangeaccessstate.md)|<span data-ttu-id="9eef9-p109">Der Zugriffszustand des Geräts in Exchange. Mögliche Werte: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="9eef9-p109">The Access State of the device in Exchange. The possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="9eef9-213">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="9eef9-213">exchangeAccessStateReason</span></span>|[<span data-ttu-id="9eef9-214">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="9eef9-214">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune_devices_devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="9eef9-p110">Der Grund für den Zugriffszustand des Geräts in Exchange. Mögliche Werte: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="9eef9-p110">The reason for the device's access state in Exchange. The possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="9eef9-217">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="9eef9-217">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="9eef9-218">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-218">String</span></span>|<span data-ttu-id="9eef9-219">URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="9eef9-219">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="9eef9-220">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="9eef9-220">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="9eef9-221">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-221">String</span></span>|<span data-ttu-id="9eef9-222">Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.</span><span class="sxs-lookup"><span data-stu-id="9eef9-222">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="9eef9-223">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="9eef9-223">isEncrypted</span></span>|<span data-ttu-id="9eef9-224">boolesch</span><span class="sxs-lookup"><span data-stu-id="9eef9-224">Boolean</span></span>|<span data-ttu-id="9eef9-225">Verschlüsselungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9eef9-225">Device encryption status</span></span>|
|<span data-ttu-id="9eef9-226">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9eef9-226">userPrincipalName</span></span>|<span data-ttu-id="9eef9-227">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-227">String</span></span>|<span data-ttu-id="9eef9-228">Benutzerprinzipalname für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="9eef9-228">Device user principal name</span></span>|
|<span data-ttu-id="9eef9-229">Modell</span><span class="sxs-lookup"><span data-stu-id="9eef9-229">model</span></span>|<span data-ttu-id="9eef9-230">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-230">String</span></span>|<span data-ttu-id="9eef9-231">Modell des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9eef9-231">Model of the device</span></span>|
|<span data-ttu-id="9eef9-232">Hersteller</span><span class="sxs-lookup"><span data-stu-id="9eef9-232">manufacturer</span></span>|<span data-ttu-id="9eef9-233">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-233">String</span></span>|<span data-ttu-id="9eef9-234">Hersteller des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9eef9-234">Manufacturer of the device</span></span>|
|<span data-ttu-id="9eef9-235">IMEI</span><span class="sxs-lookup"><span data-stu-id="9eef9-235">imei</span></span>|<span data-ttu-id="9eef9-236">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-236">String</span></span>|<span data-ttu-id="9eef9-237">IMEI</span><span class="sxs-lookup"><span data-stu-id="9eef9-237">IMEI</span></span>|
|<span data-ttu-id="9eef9-238">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9eef9-238">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9eef9-239">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9eef9-239">DateTimeOffset</span></span>|<span data-ttu-id="9eef9-240">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität.</span><span class="sxs-lookup"><span data-stu-id="9eef9-240">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="9eef9-241">serialNumber</span><span class="sxs-lookup"><span data-stu-id="9eef9-241">serialNumber</span></span>|<span data-ttu-id="9eef9-242">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-242">String</span></span>|<span data-ttu-id="9eef9-243">Seriennummer.</span><span class="sxs-lookup"><span data-stu-id="9eef9-243">SerialNumber</span></span>|
|<span data-ttu-id="9eef9-244">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="9eef9-244">phoneNumber</span></span>|<span data-ttu-id="9eef9-245">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-245">String</span></span>|<span data-ttu-id="9eef9-246">Telefonnummer des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9eef9-246">Phone number of the device</span></span>|
|<span data-ttu-id="9eef9-247">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="9eef9-247">androidSecurityPatchLevel</span></span>|<span data-ttu-id="9eef9-248">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-248">String</span></span>|<span data-ttu-id="9eef9-249">Android-Sicherheitspatchlevel.</span><span class="sxs-lookup"><span data-stu-id="9eef9-249">Android security patch level</span></span>|
|<span data-ttu-id="9eef9-250">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="9eef9-250">userDisplayName</span></span>|<span data-ttu-id="9eef9-251">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-251">String</span></span>|<span data-ttu-id="9eef9-252">Anzeigename des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="9eef9-252">User display name</span></span>|
|<span data-ttu-id="9eef9-253">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="9eef9-253">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="9eef9-254">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="9eef9-254">configurationManagerClientEnabledFeatures</span></span>](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="9eef9-255">Aktivierte Funktionen des Konfigurations-Manager-Clients.</span><span class="sxs-lookup"><span data-stu-id="9eef9-255">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="9eef9-256">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="9eef9-256">wiFiMacAddress</span></span>|<span data-ttu-id="9eef9-257">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-257">String</span></span>|<span data-ttu-id="9eef9-258">WLAN-MAC</span><span class="sxs-lookup"><span data-stu-id="9eef9-258">Wi-Fi MAC</span></span>|
|<span data-ttu-id="9eef9-259">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="9eef9-259">deviceHealthAttestationState</span></span>|[<span data-ttu-id="9eef9-260">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="9eef9-260">deviceHealthAttestationState</span></span>](../resources/intune_devices_devicehealthattestationstate.md)|<span data-ttu-id="9eef9-261">Status des Integritätsnachweises für Geräte.</span><span class="sxs-lookup"><span data-stu-id="9eef9-261">The device health attestation state.</span></span>|
|<span data-ttu-id="9eef9-262">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="9eef9-262">subscriberCarrier</span></span>|<span data-ttu-id="9eef9-263">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-263">String</span></span>|<span data-ttu-id="9eef9-264">Netzbetreiber des Abonnenten.</span><span class="sxs-lookup"><span data-stu-id="9eef9-264">Subscriber Carrier</span></span>|
|<span data-ttu-id="9eef9-265">MEID</span><span class="sxs-lookup"><span data-stu-id="9eef9-265">meid</span></span>|<span data-ttu-id="9eef9-266">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-266">String</span></span>|<span data-ttu-id="9eef9-267">MEID</span><span class="sxs-lookup"><span data-stu-id="9eef9-267">MEID</span></span>|
|<span data-ttu-id="9eef9-268">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="9eef9-268">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="9eef9-269">Int64</span><span class="sxs-lookup"><span data-stu-id="9eef9-269">Int64</span></span>|<span data-ttu-id="9eef9-270">Gesamtspeicher in Byte.</span><span class="sxs-lookup"><span data-stu-id="9eef9-270">Total Storage in Bytes</span></span>|
|<span data-ttu-id="9eef9-271">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="9eef9-271">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="9eef9-272">Int64</span><span class="sxs-lookup"><span data-stu-id="9eef9-272">Int64</span></span>|<span data-ttu-id="9eef9-273">Freier Speicher in Byte.</span><span class="sxs-lookup"><span data-stu-id="9eef9-273">Free Storage in Bytes</span></span>|
|<span data-ttu-id="9eef9-274">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="9eef9-274">managedDeviceName</span></span>|<span data-ttu-id="9eef9-275">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eef9-275">String</span></span>|<span data-ttu-id="9eef9-276">Automatisch generierter Name zur Identifizierung des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9eef9-276">Automatically generated name to identify a device.</span></span> <span data-ttu-id="9eef9-277">Kann mit einem benutzerfreundlichen Namen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="9eef9-277">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="9eef9-278">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="9eef9-278">partnerReportedThreatState</span></span>|[<span data-ttu-id="9eef9-279">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="9eef9-279">managedDevicePartnerReportedHealthState</span></span>](../resources/intune_devices_manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="9eef9-p112">Gibt den Bedrohungszustand eines Geräts an, wenn ein Mobile Threat Defense-Partner vom Konto und dem Gerät genutzt wird. Nur Lesezugriff. Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="9eef9-p112">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span>|



## <a name="response"></a><span data-ttu-id="9eef9-283">Antwort</span><span class="sxs-lookup"><span data-stu-id="9eef9-283">Response</span></span>
<span data-ttu-id="9eef9-284">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDevice](../resources/intune_devices_manageddevice.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9eef9-284">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9eef9-285">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9eef9-285">Example</span></span>
### <a name="request"></a><span data-ttu-id="9eef9-286">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9eef9-286">Request</span></span>
<span data-ttu-id="9eef9-287">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9eef9-287">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 4604

{
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
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

### <a name="response"></a><span data-ttu-id="9eef9-288">Antwort</span><span class="sxs-lookup"><span data-stu-id="9eef9-288">Response</span></span>
<span data-ttu-id="9eef9-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9eef9-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4705

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
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








