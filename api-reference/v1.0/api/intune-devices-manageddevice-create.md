---
title: Erstellen von „managedDevice“
description: Diese Methode erstellt ein neues Objekt des Typs managedDevice.
ms.openlocfilehash: 9fa8efe9a4dd1a4ec753c25382f95f383bf0fe8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016494"
---
# <a name="create-manageddevice"></a><span data-ttu-id="3410a-103">Erstellen von „managedDevice“</span><span class="sxs-lookup"><span data-stu-id="3410a-103">Create managedDevice</span></span>

> <span data-ttu-id="3410a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3410a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3410a-105">Diese Methode erstellt ein neues Objekt des Typs [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="3410a-105">Create a new [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3410a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3410a-106">Prerequisites</span></span>
<span data-ttu-id="3410a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3410a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3410a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3410a-109">Permission type</span></span>|<span data-ttu-id="3410a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3410a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3410a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3410a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3410a-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3410a-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3410a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3410a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3410a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3410a-114">Not supported.</span></span>|
|<span data-ttu-id="3410a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3410a-115">Application</span></span>|<span data-ttu-id="3410a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3410a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3410a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3410a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="3410a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3410a-118">Request headers</span></span>
|<span data-ttu-id="3410a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3410a-119">Header</span></span>|<span data-ttu-id="3410a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3410a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3410a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3410a-121">Authorization</span></span>|<span data-ttu-id="3410a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3410a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3410a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3410a-123">Accept</span></span>|<span data-ttu-id="3410a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3410a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3410a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3410a-125">Request body</span></span>
<span data-ttu-id="3410a-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedDevice“ an.</span><span class="sxs-lookup"><span data-stu-id="3410a-126">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="3410a-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedDevice“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="3410a-127">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="3410a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3410a-128">Property</span></span>|<span data-ttu-id="3410a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3410a-129">Type</span></span>|<span data-ttu-id="3410a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3410a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3410a-131">id</span><span class="sxs-lookup"><span data-stu-id="3410a-131">id</span></span>|<span data-ttu-id="3410a-132">String</span><span class="sxs-lookup"><span data-stu-id="3410a-132">String</span></span>|<span data-ttu-id="3410a-133">Eindeutiger Bezeichner für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="3410a-133">Unique Identifier for the device</span></span>|
|<span data-ttu-id="3410a-134">userId</span><span class="sxs-lookup"><span data-stu-id="3410a-134">userId</span></span>|<span data-ttu-id="3410a-135">String</span><span class="sxs-lookup"><span data-stu-id="3410a-135">String</span></span>|<span data-ttu-id="3410a-136">Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="3410a-136">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="3410a-137">deviceName</span><span class="sxs-lookup"><span data-stu-id="3410a-137">deviceName</span></span>|<span data-ttu-id="3410a-138">String</span><span class="sxs-lookup"><span data-stu-id="3410a-138">String</span></span>|<span data-ttu-id="3410a-139">Name des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="3410a-139">Name of the device</span></span>|
|<span data-ttu-id="3410a-140">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="3410a-140">managedDeviceOwnerType</span></span>|[<span data-ttu-id="3410a-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="3410a-141">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="3410a-142">Besitz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="3410a-142">Ownership of the device.</span></span> <span data-ttu-id="3410a-143">'Company' oder 'Privat' kann sein.</span><span class="sxs-lookup"><span data-stu-id="3410a-143">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="3410a-144">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="3410a-144">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="3410a-145">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="3410a-145">deviceActionResults</span></span>|<span data-ttu-id="3410a-146">Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3410a-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="3410a-147">Liste von Objekten des Typs „ComplexType deviceActionResult“.
</span><span class="sxs-lookup"><span data-stu-id="3410a-147">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="3410a-148">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="3410a-148">enrolledDateTime</span></span>|<span data-ttu-id="3410a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3410a-149">DateTimeOffset</span></span>|<span data-ttu-id="3410a-150">Datum und Uhrzeit der Geräteregistrierung.
</span><span class="sxs-lookup"><span data-stu-id="3410a-150">Enrollment time of the device.</span></span>|
|<span data-ttu-id="3410a-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3410a-151">lastSyncDateTime</span></span>|<span data-ttu-id="3410a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3410a-152">DateTimeOffset</span></span>|<span data-ttu-id="3410a-153">Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
</span><span class="sxs-lookup"><span data-stu-id="3410a-153">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="3410a-154">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="3410a-154">operatingSystem</span></span>|<span data-ttu-id="3410a-155">String</span><span class="sxs-lookup"><span data-stu-id="3410a-155">String</span></span>|<span data-ttu-id="3410a-156">Betriebssystem des Geräts.</span><span class="sxs-lookup"><span data-stu-id="3410a-156">Operating system of the device.</span></span> <span data-ttu-id="3410a-157">Windows, iOS usw.</span><span class="sxs-lookup"><span data-stu-id="3410a-157">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="3410a-158">complianceState</span><span class="sxs-lookup"><span data-stu-id="3410a-158">complianceState</span></span>|[<span data-ttu-id="3410a-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="3410a-159">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="3410a-160">Konformitätsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="3410a-160">Compliance state of the device.</span></span> <span data-ttu-id="3410a-161">Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.</span><span class="sxs-lookup"><span data-stu-id="3410a-161">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="3410a-162">jailBroken</span><span class="sxs-lookup"><span data-stu-id="3410a-162">jailBroken</span></span>|<span data-ttu-id="3410a-163">String</span><span class="sxs-lookup"><span data-stu-id="3410a-163">String</span></span>|<span data-ttu-id="3410a-164">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="3410a-164">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="3410a-165">managementAgent</span><span class="sxs-lookup"><span data-stu-id="3410a-165">managementAgent</span></span>|[<span data-ttu-id="3410a-166">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="3410a-166">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="3410a-167">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="3410a-167">Management channel of the device.</span></span> <span data-ttu-id="3410a-168">Intune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf` und `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="3410a-168">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="3410a-169">osVersion</span><span class="sxs-lookup"><span data-stu-id="3410a-169">osVersion</span></span>|<span data-ttu-id="3410a-170">String</span><span class="sxs-lookup"><span data-stu-id="3410a-170">String</span></span>|<span data-ttu-id="3410a-171">Auf dem Gerät installierte Betriebssystemversion.
</span><span class="sxs-lookup"><span data-stu-id="3410a-171">Operating system version of the device.</span></span>|
|<span data-ttu-id="3410a-172">easActivated</span><span class="sxs-lookup"><span data-stu-id="3410a-172">easActivated</span></span>|<span data-ttu-id="3410a-173">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3410a-173">Boolean</span></span>|<span data-ttu-id="3410a-174">Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="3410a-174">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="3410a-175">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="3410a-175">easDeviceId</span></span>|<span data-ttu-id="3410a-176">String</span><span class="sxs-lookup"><span data-stu-id="3410a-176">String</span></span>|<span data-ttu-id="3410a-177">Exchange ActiveSync-ID des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="3410a-177">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="3410a-178">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="3410a-178">easActivationDateTime</span></span>|<span data-ttu-id="3410a-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3410a-179">DateTimeOffset</span></span>|<span data-ttu-id="3410a-180">Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="3410a-180">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="3410a-181">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="3410a-181">azureADRegistered</span></span>|<span data-ttu-id="3410a-182">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3410a-182">Boolean</span></span>|<span data-ttu-id="3410a-183">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="3410a-183">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="3410a-184">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="3410a-184">deviceEnrollmentType</span></span>|[<span data-ttu-id="3410a-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="3410a-185">deviceEnrollmentType</span></span>](../resources/intune-devices-deviceenrollmenttype.md)|<span data-ttu-id="3410a-186">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="3410a-186">Enrollment type of the device.</span></span> <span data-ttu-id="3410a-187">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="3410a-187">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="3410a-188">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="3410a-188">activationLockBypassCode</span></span>|<span data-ttu-id="3410a-189">String</span><span class="sxs-lookup"><span data-stu-id="3410a-189">String</span></span>|<span data-ttu-id="3410a-190">Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht</span><span class="sxs-lookup"><span data-stu-id="3410a-190">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="3410a-191">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3410a-191">emailAddress</span></span>|<span data-ttu-id="3410a-192">String</span><span class="sxs-lookup"><span data-stu-id="3410a-192">String</span></span>|<span data-ttu-id="3410a-193">E-Mail-Adressen des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="3410a-193">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="3410a-194">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="3410a-194">azureADDeviceId</span></span>|<span data-ttu-id="3410a-195">String</span><span class="sxs-lookup"><span data-stu-id="3410a-195">String</span></span>|<span data-ttu-id="3410a-196">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="3410a-196">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="3410a-197">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3410a-197">Read only.</span></span>|
|<span data-ttu-id="3410a-198">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="3410a-198">deviceRegistrationState</span></span>|[<span data-ttu-id="3410a-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="3410a-199">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="3410a-200">Registrierungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="3410a-200">Device registration state.</span></span> <span data-ttu-id="3410a-201">Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3410a-201">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="3410a-202">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="3410a-202">deviceCategoryDisplayName</span></span>|<span data-ttu-id="3410a-203">String</span><span class="sxs-lookup"><span data-stu-id="3410a-203">String</span></span>|<span data-ttu-id="3410a-204">Anzeigename der Gerätekategorie.
</span><span class="sxs-lookup"><span data-stu-id="3410a-204">Device category display name</span></span>|
|<span data-ttu-id="3410a-205">isSupervised</span><span class="sxs-lookup"><span data-stu-id="3410a-205">isSupervised</span></span>|<span data-ttu-id="3410a-206">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3410a-206">Boolean</span></span>|<span data-ttu-id="3410a-207">Überwachungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="3410a-207">Device supervised status</span></span>|
|<span data-ttu-id="3410a-208">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3410a-208">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="3410a-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3410a-209">DateTimeOffset</span></span>|<span data-ttu-id="3410a-210">Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange</span><span class="sxs-lookup"><span data-stu-id="3410a-210">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="3410a-211">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="3410a-211">exchangeAccessState</span></span>|[<span data-ttu-id="3410a-212">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="3410a-212">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="3410a-213">Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="3410a-213">The Access State of the device in Exchange.</span></span> <span data-ttu-id="3410a-214">Mögliche Werte sind: `none`, `unknown`, `allowed`, `blocked` und `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="3410a-214">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="3410a-215">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="3410a-215">exchangeAccessStateReason</span></span>|[<span data-ttu-id="3410a-216">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="3410a-216">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="3410a-217">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="3410a-217">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="3410a-218">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="3410a-218">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="3410a-219">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="3410a-219">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="3410a-220">String</span><span class="sxs-lookup"><span data-stu-id="3410a-220">String</span></span>|<span data-ttu-id="3410a-221">URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
</span><span class="sxs-lookup"><span data-stu-id="3410a-221">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="3410a-222">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3410a-222">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="3410a-223">String</span><span class="sxs-lookup"><span data-stu-id="3410a-223">String</span></span>|<span data-ttu-id="3410a-224">Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
</span><span class="sxs-lookup"><span data-stu-id="3410a-224">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="3410a-225">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="3410a-225">isEncrypted</span></span>|<span data-ttu-id="3410a-226">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3410a-226">Boolean</span></span>|<span data-ttu-id="3410a-227">Verschlüsselungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="3410a-227">Device encryption status</span></span>|
|<span data-ttu-id="3410a-228">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3410a-228">userPrincipalName</span></span>|<span data-ttu-id="3410a-229">String</span><span class="sxs-lookup"><span data-stu-id="3410a-229">String</span></span>|<span data-ttu-id="3410a-230">Benutzerprinzipalname für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="3410a-230">Device user principal name</span></span>|
|<span data-ttu-id="3410a-231">model</span><span class="sxs-lookup"><span data-stu-id="3410a-231">model</span></span>|<span data-ttu-id="3410a-232">String</span><span class="sxs-lookup"><span data-stu-id="3410a-232">String</span></span>|<span data-ttu-id="3410a-233">Modell des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="3410a-233">Model of the device</span></span>|
|<span data-ttu-id="3410a-234">manufacturer</span><span class="sxs-lookup"><span data-stu-id="3410a-234">manufacturer</span></span>|<span data-ttu-id="3410a-235">String</span><span class="sxs-lookup"><span data-stu-id="3410a-235">String</span></span>|<span data-ttu-id="3410a-236">Hersteller des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="3410a-236">Manufacturer of the device</span></span>|
|<span data-ttu-id="3410a-237">imei</span><span class="sxs-lookup"><span data-stu-id="3410a-237">imei</span></span>|<span data-ttu-id="3410a-238">String</span><span class="sxs-lookup"><span data-stu-id="3410a-238">String</span></span>|<span data-ttu-id="3410a-239">IMEI</span><span class="sxs-lookup"><span data-stu-id="3410a-239">IMEI</span></span>|
|<span data-ttu-id="3410a-240">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3410a-240">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="3410a-241">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3410a-241">DateTimeOffset</span></span>|<span data-ttu-id="3410a-242">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität.
</span><span class="sxs-lookup"><span data-stu-id="3410a-242">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="3410a-243">serialNumber</span><span class="sxs-lookup"><span data-stu-id="3410a-243">serialNumber</span></span>|<span data-ttu-id="3410a-244">String</span><span class="sxs-lookup"><span data-stu-id="3410a-244">String</span></span>|<span data-ttu-id="3410a-245">Seriennummer.
</span><span class="sxs-lookup"><span data-stu-id="3410a-245">SerialNumber</span></span>|
|<span data-ttu-id="3410a-246">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="3410a-246">phoneNumber</span></span>|<span data-ttu-id="3410a-247">String</span><span class="sxs-lookup"><span data-stu-id="3410a-247">String</span></span>|<span data-ttu-id="3410a-248">Telefonnummer des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="3410a-248">Phone number of the device</span></span>|
|<span data-ttu-id="3410a-249">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="3410a-249">androidSecurityPatchLevel</span></span>|<span data-ttu-id="3410a-250">String</span><span class="sxs-lookup"><span data-stu-id="3410a-250">String</span></span>|<span data-ttu-id="3410a-251">Android-Sicherheitspatchlevel.
</span><span class="sxs-lookup"><span data-stu-id="3410a-251">Android security patch level</span></span>|
|<span data-ttu-id="3410a-252">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3410a-252">userDisplayName</span></span>|<span data-ttu-id="3410a-253">String</span><span class="sxs-lookup"><span data-stu-id="3410a-253">String</span></span>|<span data-ttu-id="3410a-254">Anzeigename des Benutzers.
</span><span class="sxs-lookup"><span data-stu-id="3410a-254">User display name</span></span>|
|<span data-ttu-id="3410a-255">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="3410a-255">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="3410a-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="3410a-256">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="3410a-257">Aktivierte Funktionen des Konfigurations-Manager-Clients.
</span><span class="sxs-lookup"><span data-stu-id="3410a-257">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="3410a-258">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="3410a-258">wiFiMacAddress</span></span>|<span data-ttu-id="3410a-259">String</span><span class="sxs-lookup"><span data-stu-id="3410a-259">String</span></span>|<span data-ttu-id="3410a-260">WLAN-MAC</span><span class="sxs-lookup"><span data-stu-id="3410a-260">Wi-Fi MAC</span></span>|
|<span data-ttu-id="3410a-261">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="3410a-261">deviceHealthAttestationState</span></span>|[<span data-ttu-id="3410a-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="3410a-262">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="3410a-263">Status des Integritätsnachweises für Geräte.
</span><span class="sxs-lookup"><span data-stu-id="3410a-263">The device health attestation state.</span></span>|
|<span data-ttu-id="3410a-264">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="3410a-264">subscriberCarrier</span></span>|<span data-ttu-id="3410a-265">String</span><span class="sxs-lookup"><span data-stu-id="3410a-265">String</span></span>|<span data-ttu-id="3410a-266">Netzbetreiber des Abonnenten.
</span><span class="sxs-lookup"><span data-stu-id="3410a-266">Subscriber Carrier</span></span>|
|<span data-ttu-id="3410a-267">meid</span><span class="sxs-lookup"><span data-stu-id="3410a-267">meid</span></span>|<span data-ttu-id="3410a-268">String</span><span class="sxs-lookup"><span data-stu-id="3410a-268">String</span></span>|<span data-ttu-id="3410a-269">MEID</span><span class="sxs-lookup"><span data-stu-id="3410a-269">MEID</span></span>|
|<span data-ttu-id="3410a-270">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="3410a-270">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="3410a-271">Int64</span><span class="sxs-lookup"><span data-stu-id="3410a-271">Int64</span></span>|<span data-ttu-id="3410a-272">Gesamtspeicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="3410a-272">Total Storage in Bytes</span></span>|
|<span data-ttu-id="3410a-273">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="3410a-273">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="3410a-274">Int64</span><span class="sxs-lookup"><span data-stu-id="3410a-274">Int64</span></span>|<span data-ttu-id="3410a-275">Freier Speicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="3410a-275">Free Storage in Bytes</span></span>|
|<span data-ttu-id="3410a-276">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="3410a-276">managedDeviceName</span></span>|<span data-ttu-id="3410a-277">String</span><span class="sxs-lookup"><span data-stu-id="3410a-277">String</span></span>|<span data-ttu-id="3410a-278">Automatisch generierter Name zur Identifizierung des Geräts.</span><span class="sxs-lookup"><span data-stu-id="3410a-278">Automatically generated name to identify a device.</span></span> <span data-ttu-id="3410a-279">Kann mit einem benutzerfreundlichen Namen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="3410a-279">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="3410a-280">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="3410a-280">partnerReportedThreatState</span></span>|[<span data-ttu-id="3410a-281">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="3410a-281">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="3410a-282">Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen.</span><span class="sxs-lookup"><span data-stu-id="3410a-282">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="3410a-283">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3410a-283">Read Only.</span></span> <span data-ttu-id="3410a-284">Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="3410a-284">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="3410a-285">Antwort</span><span class="sxs-lookup"><span data-stu-id="3410a-285">Response</span></span>
<span data-ttu-id="3410a-286">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [managedDevice](../resources/intune-devices-manageddevice.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3410a-286">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3410a-287">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3410a-287">Example</span></span>
### <a name="request"></a><span data-ttu-id="3410a-288">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3410a-288">Request</span></span>
<span data-ttu-id="3410a-289">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3410a-289">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 4656

{
  "@odata.type": "#microsoft.graph.managedDevice",
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

### <a name="response"></a><span data-ttu-id="3410a-290">Antwort</span><span class="sxs-lookup"><span data-stu-id="3410a-290">Response</span></span>
<span data-ttu-id="3410a-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3410a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



