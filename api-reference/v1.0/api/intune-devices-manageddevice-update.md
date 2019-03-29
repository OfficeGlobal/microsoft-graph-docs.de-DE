---
title: Aktualisieren von „managedDevice“
description: Aktualisieren der Eigenschaften eines managedDeviceOverview-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12c8c2dc628b7fcecef81296ca56f17845b39478
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962862"
---
# <a name="update-manageddevice"></a><span data-ttu-id="4fc58-103">Aktualisieren von „managedDevice“</span><span class="sxs-lookup"><span data-stu-id="4fc58-103">Update managedDevice</span></span>

> <span data-ttu-id="4fc58-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4fc58-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fc58-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="4fc58-105">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fc58-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4fc58-106">Prerequisites</span></span>
<span data-ttu-id="4fc58-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fc58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fc58-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4fc58-109">Permission type</span></span>|<span data-ttu-id="4fc58-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4fc58-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fc58-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4fc58-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4fc58-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fc58-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4fc58-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4fc58-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fc58-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4fc58-114">Not supported.</span></span>|
|<span data-ttu-id="4fc58-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4fc58-115">Application</span></span>|<span data-ttu-id="4fc58-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4fc58-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fc58-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4fc58-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="4fc58-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4fc58-118">Request headers</span></span>
|<span data-ttu-id="4fc58-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4fc58-119">Header</span></span>|<span data-ttu-id="4fc58-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4fc58-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fc58-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fc58-121">Authorization</span></span>|<span data-ttu-id="4fc58-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4fc58-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fc58-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4fc58-123">Accept</span></span>|<span data-ttu-id="4fc58-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4fc58-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fc58-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4fc58-125">Request body</span></span>
<span data-ttu-id="4fc58-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDevice](../resources/intune-devices-manageddevice.md) an.</span><span class="sxs-lookup"><span data-stu-id="4fc58-126">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="4fc58-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDevice](../resources/intune-devices-manageddevice.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="4fc58-127">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="4fc58-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4fc58-128">Property</span></span>|<span data-ttu-id="4fc58-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4fc58-129">Type</span></span>|<span data-ttu-id="4fc58-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4fc58-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fc58-131">id</span><span class="sxs-lookup"><span data-stu-id="4fc58-131">id</span></span>|<span data-ttu-id="4fc58-132">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-132">String</span></span>|<span data-ttu-id="4fc58-133">Eindeutiger Bezeichner für das Gerät</span><span class="sxs-lookup"><span data-stu-id="4fc58-133">Unique Identifier for the device</span></span>|
|<span data-ttu-id="4fc58-134">userId</span><span class="sxs-lookup"><span data-stu-id="4fc58-134">userId</span></span>|<span data-ttu-id="4fc58-135">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-135">String</span></span>|<span data-ttu-id="4fc58-136">Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="4fc58-136">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="4fc58-137">deviceName</span><span class="sxs-lookup"><span data-stu-id="4fc58-137">deviceName</span></span>|<span data-ttu-id="4fc58-138">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-138">String</span></span>|<span data-ttu-id="4fc58-139">Der Name des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4fc58-139">Name of the device</span></span>|
|<span data-ttu-id="4fc58-140">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="4fc58-140">managedDeviceOwnerType</span></span>|[<span data-ttu-id="4fc58-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="4fc58-141">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="4fc58-142">Der Besitzer des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4fc58-142">Ownership of the device.</span></span> <span data-ttu-id="4fc58-143">Kann "Company" oder "Personal" sein.</span><span class="sxs-lookup"><span data-stu-id="4fc58-143">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="4fc58-144">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="4fc58-144">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="4fc58-145">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="4fc58-145">deviceActionResults</span></span>|<span data-ttu-id="4fc58-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4fc58-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="4fc58-147">Liste von ComplexType DeviceActionResult-Objekten.</span><span class="sxs-lookup"><span data-stu-id="4fc58-147">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="4fc58-148">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="4fc58-148">enrolledDateTime</span></span>|<span data-ttu-id="4fc58-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fc58-149">DateTimeOffset</span></span>|<span data-ttu-id="4fc58-150">Registrierungszeit des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4fc58-150">Enrollment time of the device.</span></span>|
|<span data-ttu-id="4fc58-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4fc58-151">lastSyncDateTime</span></span>|<span data-ttu-id="4fc58-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fc58-152">DateTimeOffset</span></span>|<span data-ttu-id="4fc58-153">Datum und Uhrzeit, zu dem bzw. der das Gerät zuletzt eine erfolgreiche Synchronisierung mit Intune durchgeführt hat.</span><span class="sxs-lookup"><span data-stu-id="4fc58-153">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="4fc58-154">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="4fc58-154">operatingSystem</span></span>|<span data-ttu-id="4fc58-155">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-155">String</span></span>|<span data-ttu-id="4fc58-156">Betriebssystem des Geräts</span><span class="sxs-lookup"><span data-stu-id="4fc58-156">Operating system of the device.</span></span> <span data-ttu-id="4fc58-157">Windows, iOS, etc.</span><span class="sxs-lookup"><span data-stu-id="4fc58-157">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="4fc58-158">complianceState</span><span class="sxs-lookup"><span data-stu-id="4fc58-158">complianceState</span></span>|[<span data-ttu-id="4fc58-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="4fc58-159">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="4fc58-160">Compliancestatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4fc58-160">Compliance state of the device.</span></span> <span data-ttu-id="4fc58-161">Mögliche Werte: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="4fc58-161">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="4fc58-162">jailBroken</span><span class="sxs-lookup"><span data-stu-id="4fc58-162">jailBroken</span></span>|<span data-ttu-id="4fc58-163">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-163">String</span></span>|<span data-ttu-id="4fc58-164">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="4fc58-164">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="4fc58-165">managementAgent</span><span class="sxs-lookup"><span data-stu-id="4fc58-165">managementAgent</span></span>|[<span data-ttu-id="4fc58-166">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="4fc58-166">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="4fc58-167">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4fc58-167">Management channel of the device.</span></span> <span data-ttu-id="4fc58-168">Intune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="4fc58-168">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="4fc58-169">osVersion</span><span class="sxs-lookup"><span data-stu-id="4fc58-169">osVersion</span></span>|<span data-ttu-id="4fc58-170">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-170">String</span></span>|<span data-ttu-id="4fc58-171">Betriebssystemversion auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="4fc58-171">Operating system version of the device.</span></span>|
|<span data-ttu-id="4fc58-172">easActivated</span><span class="sxs-lookup"><span data-stu-id="4fc58-172">easActivated</span></span>|<span data-ttu-id="4fc58-173">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4fc58-173">Boolean</span></span>|<span data-ttu-id="4fc58-174">Gibt an, ob das Gerät über Exchange ActiveSync-aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="4fc58-174">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="4fc58-175">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="4fc58-175">easDeviceId</span></span>|<span data-ttu-id="4fc58-176">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-176">String</span></span>|<span data-ttu-id="4fc58-177">Exchange ActiveSync-ID des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4fc58-177">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="4fc58-178">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="4fc58-178">easActivationDateTime</span></span>|<span data-ttu-id="4fc58-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fc58-179">DateTimeOffset</span></span>|<span data-ttu-id="4fc58-180">Exchange ActivationSync-Aktivierungszeit des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4fc58-180">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="4fc58-181">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="4fc58-181">azureADRegistered</span></span>|<span data-ttu-id="4fc58-182">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4fc58-182">Boolean</span></span>|<span data-ttu-id="4fc58-183">Gibt an, ob das Gerät für Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="4fc58-183">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="4fc58-184">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="4fc58-184">deviceEnrollmentType</span></span>|[<span data-ttu-id="4fc58-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="4fc58-185">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="4fc58-186">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4fc58-186">Enrollment type of the device.</span></span> <span data-ttu-id="4fc58-187">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="4fc58-187">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="4fc58-188">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="4fc58-188">activationLockBypassCode</span></span>|<span data-ttu-id="4fc58-189">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-189">String</span></span>|<span data-ttu-id="4fc58-190">Code, der ermöglicht, dass die Aktivierungssperre auf einem Gerät umgangen wird.</span><span class="sxs-lookup"><span data-stu-id="4fc58-190">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="4fc58-191">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4fc58-191">emailAddress</span></span>|<span data-ttu-id="4fc58-192">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-192">String</span></span>|<span data-ttu-id="4fc58-193">E-Mail(s) für den Benutzer, der dem Gerät zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="4fc58-193">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="4fc58-194">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="4fc58-194">azureADDeviceId</span></span>|<span data-ttu-id="4fc58-195">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-195">String</span></span>|<span data-ttu-id="4fc58-196">Die eindeutige ID für das Azure Active Directory-Gerät.</span><span class="sxs-lookup"><span data-stu-id="4fc58-196">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="4fc58-197">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4fc58-197">Read only.</span></span>|
|<span data-ttu-id="4fc58-198">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="4fc58-198">deviceRegistrationState</span></span>|[<span data-ttu-id="4fc58-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="4fc58-199">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="4fc58-200">Geräteregistrierungsstatus</span><span class="sxs-lookup"><span data-stu-id="4fc58-200">Device registration state.</span></span> <span data-ttu-id="4fc58-201">Mögliche Werte: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4fc58-201">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="4fc58-202">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="4fc58-202">deviceCategoryDisplayName</span></span>|<span data-ttu-id="4fc58-203">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-203">String</span></span>|<span data-ttu-id="4fc58-204">Anzeigename der Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="4fc58-204">Device category display name</span></span>|
|<span data-ttu-id="4fc58-205">isSupervised</span><span class="sxs-lookup"><span data-stu-id="4fc58-205">isSupervised</span></span>|<span data-ttu-id="4fc58-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fc58-206">Boolean</span></span>|<span data-ttu-id="4fc58-207">Überwachter Gerätestatus</span><span class="sxs-lookup"><span data-stu-id="4fc58-207">Device supervised status</span></span>|
|<span data-ttu-id="4fc58-208">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4fc58-208">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="4fc58-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fc58-209">DateTimeOffset</span></span>|<span data-ttu-id="4fc58-210">Letzter Zeitpunkt, zu dem das Gerät Exchange kontaktiert hat.</span><span class="sxs-lookup"><span data-stu-id="4fc58-210">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="4fc58-211">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="4fc58-211">exchangeAccessState</span></span>|[<span data-ttu-id="4fc58-212">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="4fc58-212">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="4fc58-213">Der Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fc58-213">The Access State of the device in Exchange.</span></span> <span data-ttu-id="4fc58-214">Mögliche Werte: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="4fc58-214">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="4fc58-215">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="4fc58-215">exchangeAccessStateReason</span></span>|[<span data-ttu-id="4fc58-216">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="4fc58-216">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="4fc58-217">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fc58-217">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="4fc58-218">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="4fc58-218">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="4fc58-219">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="4fc58-219">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="4fc58-220">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-220">String</span></span>|<span data-ttu-id="4fc58-221">Die URL, die ermöglicht, dass mit dem Gerät eine Remoteunterstützungssitzung eingerichtet wird.</span><span class="sxs-lookup"><span data-stu-id="4fc58-221">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="4fc58-222">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="4fc58-222">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="4fc58-223">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-223">String</span></span>|<span data-ttu-id="4fc58-224">Eine Fehlerzeichenfolge, die Probleme beim Erstellen von Objekten für die Remoteunterstützungssitzung identifiziert.</span><span class="sxs-lookup"><span data-stu-id="4fc58-224">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="4fc58-225">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="4fc58-225">isEncrypted</span></span>|<span data-ttu-id="4fc58-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fc58-226">Boolean</span></span>|<span data-ttu-id="4fc58-227">Geräteverschlüsselungsstatus</span><span class="sxs-lookup"><span data-stu-id="4fc58-227">Device encryption status</span></span>|
|<span data-ttu-id="4fc58-228">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4fc58-228">userPrincipalName</span></span>|<span data-ttu-id="4fc58-229">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-229">String</span></span>|<span data-ttu-id="4fc58-230">Benutzerprinzipalname für das Gerät</span><span class="sxs-lookup"><span data-stu-id="4fc58-230">Device user principal name</span></span>|
|<span data-ttu-id="4fc58-231">model</span><span class="sxs-lookup"><span data-stu-id="4fc58-231">model</span></span>|<span data-ttu-id="4fc58-232">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-232">String</span></span>|<span data-ttu-id="4fc58-233">Das Modell des Geräts.</span><span class="sxs-lookup"><span data-stu-id="4fc58-233">Model of the device</span></span>|
|<span data-ttu-id="4fc58-234">Hersteller</span><span class="sxs-lookup"><span data-stu-id="4fc58-234">manufacturer</span></span>|<span data-ttu-id="4fc58-235">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-235">String</span></span>|<span data-ttu-id="4fc58-236">Hersteller des Geräts</span><span class="sxs-lookup"><span data-stu-id="4fc58-236">Manufacturer of the device</span></span>|
|<span data-ttu-id="4fc58-237">imei</span><span class="sxs-lookup"><span data-stu-id="4fc58-237">imei</span></span>|<span data-ttu-id="4fc58-238">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-238">String</span></span>|<span data-ttu-id="4fc58-239">IMEI</span><span class="sxs-lookup"><span data-stu-id="4fc58-239">IMEI</span></span>|
|<span data-ttu-id="4fc58-240">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4fc58-240">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="4fc58-241">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fc58-241">DateTimeOffset</span></span>|<span data-ttu-id="4fc58-242">Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="4fc58-242">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="4fc58-243">serialNumber</span><span class="sxs-lookup"><span data-stu-id="4fc58-243">serialNumber</span></span>|<span data-ttu-id="4fc58-244">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-244">String</span></span>|<span data-ttu-id="4fc58-245">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="4fc58-245">SerialNumber</span></span>|
|<span data-ttu-id="4fc58-246">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="4fc58-246">phoneNumber</span></span>|<span data-ttu-id="4fc58-247">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-247">String</span></span>|<span data-ttu-id="4fc58-248">Telefonnummer des Geräts</span><span class="sxs-lookup"><span data-stu-id="4fc58-248">Phone number of the device</span></span>|
|<span data-ttu-id="4fc58-249">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="4fc58-249">androidSecurityPatchLevel</span></span>|<span data-ttu-id="4fc58-250">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-250">String</span></span>|<span data-ttu-id="4fc58-251">Sicherheitspatchlevel von Android</span><span class="sxs-lookup"><span data-stu-id="4fc58-251">Android security patch level</span></span>|
|<span data-ttu-id="4fc58-252">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4fc58-252">userDisplayName</span></span>|<span data-ttu-id="4fc58-253">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-253">String</span></span>|<span data-ttu-id="4fc58-254">Anzeigename des Benutzers</span><span class="sxs-lookup"><span data-stu-id="4fc58-254">User display name</span></span>|
|<span data-ttu-id="4fc58-255">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="4fc58-255">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="4fc58-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="4fc58-256">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="4fc58-257">Für ConfigrMgr-Client aktivierte Features</span><span class="sxs-lookup"><span data-stu-id="4fc58-257">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="4fc58-258">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="4fc58-258">wiFiMacAddress</span></span>|<span data-ttu-id="4fc58-259">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-259">String</span></span>|<span data-ttu-id="4fc58-260">Wi-Fi-MAC</span><span class="sxs-lookup"><span data-stu-id="4fc58-260">Wi-Fi MAC</span></span>|
|<span data-ttu-id="4fc58-261">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="4fc58-261">deviceHealthAttestationState</span></span>|[<span data-ttu-id="4fc58-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="4fc58-262">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="4fc58-263">Integritätsnachweis für Geräte – Status</span><span class="sxs-lookup"><span data-stu-id="4fc58-263">The device health attestation state.</span></span>|
|<span data-ttu-id="4fc58-264">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="4fc58-264">subscriberCarrier</span></span>|<span data-ttu-id="4fc58-265">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-265">String</span></span>|<span data-ttu-id="4fc58-266">Netzbetreiber des Abonnenten</span><span class="sxs-lookup"><span data-stu-id="4fc58-266">Subscriber Carrier</span></span>|
|<span data-ttu-id="4fc58-267">meid</span><span class="sxs-lookup"><span data-stu-id="4fc58-267">meid</span></span>|<span data-ttu-id="4fc58-268">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-268">String</span></span>|<span data-ttu-id="4fc58-269">MEID</span><span class="sxs-lookup"><span data-stu-id="4fc58-269">MEID</span></span>|
|<span data-ttu-id="4fc58-270">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="4fc58-270">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="4fc58-271">Int64</span><span class="sxs-lookup"><span data-stu-id="4fc58-271">Int64</span></span>|<span data-ttu-id="4fc58-272">Gesamtspeicher in Byte</span><span class="sxs-lookup"><span data-stu-id="4fc58-272">Total Storage in Bytes</span></span>|
|<span data-ttu-id="4fc58-273">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="4fc58-273">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="4fc58-274">Int64</span><span class="sxs-lookup"><span data-stu-id="4fc58-274">Int64</span></span>|<span data-ttu-id="4fc58-275">Freier Speicher in Byte</span><span class="sxs-lookup"><span data-stu-id="4fc58-275">Free Storage in Bytes</span></span>|
|<span data-ttu-id="4fc58-276">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="4fc58-276">managedDeviceName</span></span>|<span data-ttu-id="4fc58-277">String</span><span class="sxs-lookup"><span data-stu-id="4fc58-277">String</span></span>|<span data-ttu-id="4fc58-278">Automatisch generierter Name zum Identifizieren eines Geräts.</span><span class="sxs-lookup"><span data-stu-id="4fc58-278">Automatically generated name to identify a device.</span></span> <span data-ttu-id="4fc58-279">Kann mit einem Anzeigenamen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="4fc58-279">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="4fc58-280">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="4fc58-280">partnerReportedThreatState</span></span>|[<span data-ttu-id="4fc58-281">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="4fc58-281">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="4fc58-282">Gibt den Bedrohungsstatus eines Geräts an, wenn ein vom Konto und Gerät ein Mobile Threat Defense-Partner verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="4fc58-282">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="4fc58-283">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4fc58-283">Read Only.</span></span> <span data-ttu-id="4fc58-284">Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="4fc58-284">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="4fc58-285">Antwort</span><span class="sxs-lookup"><span data-stu-id="4fc58-285">Response</span></span>
<span data-ttu-id="4fc58-286">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDevice](../resources/intune-devices-manageddevice.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4fc58-286">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fc58-287">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4fc58-287">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fc58-288">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4fc58-288">Request</span></span>
<span data-ttu-id="4fc58-289">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4fc58-289">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
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

### <a name="response"></a><span data-ttu-id="4fc58-290">Antwort</span><span class="sxs-lookup"><span data-stu-id="4fc58-290">Response</span></span>
<span data-ttu-id="4fc58-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4fc58-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



