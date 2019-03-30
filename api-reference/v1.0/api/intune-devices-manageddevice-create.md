---
title: Erstellen von „managedDevice“
description: Erstellen eines neuen managedDevice-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 320b2fd8878d5ecd0af34152761bda1af6a5985c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984219"
---
# <a name="create-manageddevice"></a><span data-ttu-id="99b66-103">Erstellen von „managedDevice“</span><span class="sxs-lookup"><span data-stu-id="99b66-103">Create managedDevice</span></span>

> <span data-ttu-id="99b66-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="99b66-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99b66-105">Diese Methode erstellt ein neues Objekt des Typs [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="99b66-105">Create a new [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99b66-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="99b66-106">Prerequisites</span></span>
<span data-ttu-id="99b66-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99b66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99b66-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="99b66-109">Permission type</span></span>|<span data-ttu-id="99b66-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="99b66-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99b66-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="99b66-111">Delegated (work or school account)</span></span>|<span data-ttu-id="99b66-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99b66-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="99b66-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="99b66-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99b66-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99b66-114">Not supported.</span></span>|
|<span data-ttu-id="99b66-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="99b66-115">Application</span></span>|<span data-ttu-id="99b66-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99b66-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99b66-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="99b66-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="99b66-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="99b66-118">Request headers</span></span>
|<span data-ttu-id="99b66-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="99b66-119">Header</span></span>|<span data-ttu-id="99b66-120">Wert</span><span class="sxs-lookup"><span data-stu-id="99b66-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99b66-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="99b66-121">Authorization</span></span>|<span data-ttu-id="99b66-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="99b66-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99b66-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="99b66-123">Accept</span></span>|<span data-ttu-id="99b66-124">application/json</span><span class="sxs-lookup"><span data-stu-id="99b66-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99b66-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="99b66-125">Request body</span></span>
<span data-ttu-id="99b66-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „managedDevice“ an.</span><span class="sxs-lookup"><span data-stu-id="99b66-126">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="99b66-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „managedDevice“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="99b66-127">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="99b66-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="99b66-128">Property</span></span>|<span data-ttu-id="99b66-129">Typ</span><span class="sxs-lookup"><span data-stu-id="99b66-129">Type</span></span>|<span data-ttu-id="99b66-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99b66-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99b66-131">id</span><span class="sxs-lookup"><span data-stu-id="99b66-131">id</span></span>|<span data-ttu-id="99b66-132">String</span><span class="sxs-lookup"><span data-stu-id="99b66-132">String</span></span>|<span data-ttu-id="99b66-133">Eindeutiger Bezeichner für das Gerät</span><span class="sxs-lookup"><span data-stu-id="99b66-133">Unique Identifier for the device</span></span>|
|<span data-ttu-id="99b66-134">userId</span><span class="sxs-lookup"><span data-stu-id="99b66-134">userId</span></span>|<span data-ttu-id="99b66-135">String</span><span class="sxs-lookup"><span data-stu-id="99b66-135">String</span></span>|<span data-ttu-id="99b66-136">Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="99b66-136">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="99b66-137">deviceName</span><span class="sxs-lookup"><span data-stu-id="99b66-137">deviceName</span></span>|<span data-ttu-id="99b66-138">String</span><span class="sxs-lookup"><span data-stu-id="99b66-138">String</span></span>|<span data-ttu-id="99b66-139">Der Name des Geräts.</span><span class="sxs-lookup"><span data-stu-id="99b66-139">Name of the device</span></span>|
|<span data-ttu-id="99b66-140">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="99b66-140">managedDeviceOwnerType</span></span>|[<span data-ttu-id="99b66-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="99b66-141">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="99b66-142">Der Besitzer des Geräts.</span><span class="sxs-lookup"><span data-stu-id="99b66-142">Ownership of the device.</span></span> <span data-ttu-id="99b66-143">Kann "Company" oder "Personal" sein.</span><span class="sxs-lookup"><span data-stu-id="99b66-143">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="99b66-144">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="99b66-144">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="99b66-145">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="99b66-145">deviceActionResults</span></span>|<span data-ttu-id="99b66-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="99b66-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="99b66-147">Liste von ComplexType DeviceActionResult-Objekten.</span><span class="sxs-lookup"><span data-stu-id="99b66-147">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="99b66-148">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="99b66-148">enrolledDateTime</span></span>|<span data-ttu-id="99b66-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b66-149">DateTimeOffset</span></span>|<span data-ttu-id="99b66-150">Registrierungszeit des Geräts.</span><span class="sxs-lookup"><span data-stu-id="99b66-150">Enrollment time of the device.</span></span>|
|<span data-ttu-id="99b66-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="99b66-151">lastSyncDateTime</span></span>|<span data-ttu-id="99b66-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b66-152">DateTimeOffset</span></span>|<span data-ttu-id="99b66-153">Datum und Uhrzeit, zu dem bzw. der das Gerät zuletzt eine erfolgreiche Synchronisierung mit Intune durchgeführt hat.</span><span class="sxs-lookup"><span data-stu-id="99b66-153">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="99b66-154">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="99b66-154">operatingSystem</span></span>|<span data-ttu-id="99b66-155">String</span><span class="sxs-lookup"><span data-stu-id="99b66-155">String</span></span>|<span data-ttu-id="99b66-156">Betriebssystem des Geräts</span><span class="sxs-lookup"><span data-stu-id="99b66-156">Operating system of the device.</span></span> <span data-ttu-id="99b66-157">Windows, iOS, etc.</span><span class="sxs-lookup"><span data-stu-id="99b66-157">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="99b66-158">complianceState</span><span class="sxs-lookup"><span data-stu-id="99b66-158">complianceState</span></span>|[<span data-ttu-id="99b66-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="99b66-159">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="99b66-160">Compliancestatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="99b66-160">Compliance state of the device.</span></span> <span data-ttu-id="99b66-161">Mögliche Werte: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="99b66-161">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="99b66-162">jailBroken</span><span class="sxs-lookup"><span data-stu-id="99b66-162">jailBroken</span></span>|<span data-ttu-id="99b66-163">String</span><span class="sxs-lookup"><span data-stu-id="99b66-163">String</span></span>|<span data-ttu-id="99b66-164">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="99b66-164">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="99b66-165">managementAgent</span><span class="sxs-lookup"><span data-stu-id="99b66-165">managementAgent</span></span>|[<span data-ttu-id="99b66-166">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="99b66-166">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="99b66-167">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="99b66-167">Management channel of the device.</span></span> <span data-ttu-id="99b66-168">Intune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="99b66-168">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="99b66-169">osVersion</span><span class="sxs-lookup"><span data-stu-id="99b66-169">osVersion</span></span>|<span data-ttu-id="99b66-170">String</span><span class="sxs-lookup"><span data-stu-id="99b66-170">String</span></span>|<span data-ttu-id="99b66-171">Betriebssystemversion auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="99b66-171">Operating system version of the device.</span></span>|
|<span data-ttu-id="99b66-172">easActivated</span><span class="sxs-lookup"><span data-stu-id="99b66-172">easActivated</span></span>|<span data-ttu-id="99b66-173">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="99b66-173">Boolean</span></span>|<span data-ttu-id="99b66-174">Gibt an, ob das Gerät über Exchange ActiveSync-aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="99b66-174">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="99b66-175">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="99b66-175">easDeviceId</span></span>|<span data-ttu-id="99b66-176">String</span><span class="sxs-lookup"><span data-stu-id="99b66-176">String</span></span>|<span data-ttu-id="99b66-177">Exchange ActiveSync-ID des Geräts.</span><span class="sxs-lookup"><span data-stu-id="99b66-177">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="99b66-178">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="99b66-178">easActivationDateTime</span></span>|<span data-ttu-id="99b66-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b66-179">DateTimeOffset</span></span>|<span data-ttu-id="99b66-180">Exchange ActivationSync-Aktivierungszeit des Geräts.</span><span class="sxs-lookup"><span data-stu-id="99b66-180">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="99b66-181">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="99b66-181">azureADRegistered</span></span>|<span data-ttu-id="99b66-182">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="99b66-182">Boolean</span></span>|<span data-ttu-id="99b66-183">Gibt an, ob das Gerät für Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="99b66-183">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="99b66-184">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="99b66-184">deviceEnrollmentType</span></span>|[<span data-ttu-id="99b66-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="99b66-185">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="99b66-186">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="99b66-186">Enrollment type of the device.</span></span> <span data-ttu-id="99b66-187">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="99b66-187">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="99b66-188">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="99b66-188">activationLockBypassCode</span></span>|<span data-ttu-id="99b66-189">String</span><span class="sxs-lookup"><span data-stu-id="99b66-189">String</span></span>|<span data-ttu-id="99b66-190">Code, der ermöglicht, dass die Aktivierungssperre auf einem Gerät umgangen wird.</span><span class="sxs-lookup"><span data-stu-id="99b66-190">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="99b66-191">emailAddress</span><span class="sxs-lookup"><span data-stu-id="99b66-191">emailAddress</span></span>|<span data-ttu-id="99b66-192">String</span><span class="sxs-lookup"><span data-stu-id="99b66-192">String</span></span>|<span data-ttu-id="99b66-193">E-Mail(s) für den Benutzer, der dem Gerät zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="99b66-193">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="99b66-194">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="99b66-194">azureADDeviceId</span></span>|<span data-ttu-id="99b66-195">String</span><span class="sxs-lookup"><span data-stu-id="99b66-195">String</span></span>|<span data-ttu-id="99b66-196">Die eindeutige ID für das Azure Active Directory-Gerät.</span><span class="sxs-lookup"><span data-stu-id="99b66-196">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="99b66-197">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="99b66-197">Read only.</span></span>|
|<span data-ttu-id="99b66-198">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="99b66-198">deviceRegistrationState</span></span>|[<span data-ttu-id="99b66-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="99b66-199">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="99b66-200">Geräteregistrierungsstatus</span><span class="sxs-lookup"><span data-stu-id="99b66-200">Device registration state.</span></span> <span data-ttu-id="99b66-201">Mögliche Werte: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="99b66-201">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="99b66-202">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="99b66-202">deviceCategoryDisplayName</span></span>|<span data-ttu-id="99b66-203">String</span><span class="sxs-lookup"><span data-stu-id="99b66-203">String</span></span>|<span data-ttu-id="99b66-204">Anzeigename der Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="99b66-204">Device category display name</span></span>|
|<span data-ttu-id="99b66-205">isSupervised</span><span class="sxs-lookup"><span data-stu-id="99b66-205">isSupervised</span></span>|<span data-ttu-id="99b66-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="99b66-206">Boolean</span></span>|<span data-ttu-id="99b66-207">Überwachter Gerätestatus</span><span class="sxs-lookup"><span data-stu-id="99b66-207">Device supervised status</span></span>|
|<span data-ttu-id="99b66-208">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="99b66-208">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="99b66-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b66-209">DateTimeOffset</span></span>|<span data-ttu-id="99b66-210">Letzter Zeitpunkt, zu dem das Gerät Exchange kontaktiert hat.</span><span class="sxs-lookup"><span data-stu-id="99b66-210">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="99b66-211">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="99b66-211">exchangeAccessState</span></span>|[<span data-ttu-id="99b66-212">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="99b66-212">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="99b66-213">Der Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="99b66-213">The Access State of the device in Exchange.</span></span> <span data-ttu-id="99b66-214">Mögliche Werte: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="99b66-214">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="99b66-215">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="99b66-215">exchangeAccessStateReason</span></span>|[<span data-ttu-id="99b66-216">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="99b66-216">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="99b66-217">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="99b66-217">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="99b66-218">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="99b66-218">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="99b66-219">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="99b66-219">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="99b66-220">String</span><span class="sxs-lookup"><span data-stu-id="99b66-220">String</span></span>|<span data-ttu-id="99b66-221">Die URL, die ermöglicht, dass mit dem Gerät eine Remoteunterstützungssitzung eingerichtet wird.</span><span class="sxs-lookup"><span data-stu-id="99b66-221">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="99b66-222">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="99b66-222">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="99b66-223">String</span><span class="sxs-lookup"><span data-stu-id="99b66-223">String</span></span>|<span data-ttu-id="99b66-224">Eine Fehlerzeichenfolge, die Probleme beim Erstellen von Objekten für die Remoteunterstützungssitzung identifiziert.</span><span class="sxs-lookup"><span data-stu-id="99b66-224">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="99b66-225">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="99b66-225">isEncrypted</span></span>|<span data-ttu-id="99b66-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="99b66-226">Boolean</span></span>|<span data-ttu-id="99b66-227">Geräteverschlüsselungsstatus</span><span class="sxs-lookup"><span data-stu-id="99b66-227">Device encryption status</span></span>|
|<span data-ttu-id="99b66-228">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="99b66-228">userPrincipalName</span></span>|<span data-ttu-id="99b66-229">String</span><span class="sxs-lookup"><span data-stu-id="99b66-229">String</span></span>|<span data-ttu-id="99b66-230">Benutzerprinzipalname für das Gerät</span><span class="sxs-lookup"><span data-stu-id="99b66-230">Device user principal name</span></span>|
|<span data-ttu-id="99b66-231">model</span><span class="sxs-lookup"><span data-stu-id="99b66-231">model</span></span>|<span data-ttu-id="99b66-232">String</span><span class="sxs-lookup"><span data-stu-id="99b66-232">String</span></span>|<span data-ttu-id="99b66-233">Das Modell des Geräts.</span><span class="sxs-lookup"><span data-stu-id="99b66-233">Model of the device</span></span>|
|<span data-ttu-id="99b66-234">Hersteller</span><span class="sxs-lookup"><span data-stu-id="99b66-234">manufacturer</span></span>|<span data-ttu-id="99b66-235">String</span><span class="sxs-lookup"><span data-stu-id="99b66-235">String</span></span>|<span data-ttu-id="99b66-236">Hersteller des Geräts</span><span class="sxs-lookup"><span data-stu-id="99b66-236">Manufacturer of the device</span></span>|
|<span data-ttu-id="99b66-237">imei</span><span class="sxs-lookup"><span data-stu-id="99b66-237">imei</span></span>|<span data-ttu-id="99b66-238">String</span><span class="sxs-lookup"><span data-stu-id="99b66-238">String</span></span>|<span data-ttu-id="99b66-239">IMEI</span><span class="sxs-lookup"><span data-stu-id="99b66-239">IMEI</span></span>|
|<span data-ttu-id="99b66-240">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="99b66-240">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="99b66-241">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b66-241">DateTimeOffset</span></span>|<span data-ttu-id="99b66-242">Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="99b66-242">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="99b66-243">serialNumber</span><span class="sxs-lookup"><span data-stu-id="99b66-243">serialNumber</span></span>|<span data-ttu-id="99b66-244">String</span><span class="sxs-lookup"><span data-stu-id="99b66-244">String</span></span>|<span data-ttu-id="99b66-245">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="99b66-245">SerialNumber</span></span>|
|<span data-ttu-id="99b66-246">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="99b66-246">phoneNumber</span></span>|<span data-ttu-id="99b66-247">String</span><span class="sxs-lookup"><span data-stu-id="99b66-247">String</span></span>|<span data-ttu-id="99b66-248">Telefonnummer des Geräts</span><span class="sxs-lookup"><span data-stu-id="99b66-248">Phone number of the device</span></span>|
|<span data-ttu-id="99b66-249">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="99b66-249">androidSecurityPatchLevel</span></span>|<span data-ttu-id="99b66-250">String</span><span class="sxs-lookup"><span data-stu-id="99b66-250">String</span></span>|<span data-ttu-id="99b66-251">Sicherheitspatchlevel von Android</span><span class="sxs-lookup"><span data-stu-id="99b66-251">Android security patch level</span></span>|
|<span data-ttu-id="99b66-252">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="99b66-252">userDisplayName</span></span>|<span data-ttu-id="99b66-253">String</span><span class="sxs-lookup"><span data-stu-id="99b66-253">String</span></span>|<span data-ttu-id="99b66-254">Anzeigename des Benutzers</span><span class="sxs-lookup"><span data-stu-id="99b66-254">User display name</span></span>|
|<span data-ttu-id="99b66-255">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="99b66-255">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="99b66-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="99b66-256">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="99b66-257">Für ConfigrMgr-Client aktivierte Features</span><span class="sxs-lookup"><span data-stu-id="99b66-257">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="99b66-258">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="99b66-258">wiFiMacAddress</span></span>|<span data-ttu-id="99b66-259">String</span><span class="sxs-lookup"><span data-stu-id="99b66-259">String</span></span>|<span data-ttu-id="99b66-260">Wi-Fi-MAC</span><span class="sxs-lookup"><span data-stu-id="99b66-260">Wi-Fi MAC</span></span>|
|<span data-ttu-id="99b66-261">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="99b66-261">deviceHealthAttestationState</span></span>|[<span data-ttu-id="99b66-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="99b66-262">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="99b66-263">Integritätsnachweis für Geräte – Status</span><span class="sxs-lookup"><span data-stu-id="99b66-263">The device health attestation state.</span></span>|
|<span data-ttu-id="99b66-264">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="99b66-264">subscriberCarrier</span></span>|<span data-ttu-id="99b66-265">String</span><span class="sxs-lookup"><span data-stu-id="99b66-265">String</span></span>|<span data-ttu-id="99b66-266">Netzbetreiber des Abonnenten</span><span class="sxs-lookup"><span data-stu-id="99b66-266">Subscriber Carrier</span></span>|
|<span data-ttu-id="99b66-267">meid</span><span class="sxs-lookup"><span data-stu-id="99b66-267">meid</span></span>|<span data-ttu-id="99b66-268">String</span><span class="sxs-lookup"><span data-stu-id="99b66-268">String</span></span>|<span data-ttu-id="99b66-269">MEID</span><span class="sxs-lookup"><span data-stu-id="99b66-269">MEID</span></span>|
|<span data-ttu-id="99b66-270">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="99b66-270">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="99b66-271">Int64</span><span class="sxs-lookup"><span data-stu-id="99b66-271">Int64</span></span>|<span data-ttu-id="99b66-272">Gesamtspeicher in Byte</span><span class="sxs-lookup"><span data-stu-id="99b66-272">Total Storage in Bytes</span></span>|
|<span data-ttu-id="99b66-273">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="99b66-273">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="99b66-274">Int64</span><span class="sxs-lookup"><span data-stu-id="99b66-274">Int64</span></span>|<span data-ttu-id="99b66-275">Freier Speicher in Byte</span><span class="sxs-lookup"><span data-stu-id="99b66-275">Free Storage in Bytes</span></span>|
|<span data-ttu-id="99b66-276">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="99b66-276">managedDeviceName</span></span>|<span data-ttu-id="99b66-277">String</span><span class="sxs-lookup"><span data-stu-id="99b66-277">String</span></span>|<span data-ttu-id="99b66-278">Automatisch generierter Name zum Identifizieren eines Geräts.</span><span class="sxs-lookup"><span data-stu-id="99b66-278">Automatically generated name to identify a device.</span></span> <span data-ttu-id="99b66-279">Kann mit einem Anzeigenamen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="99b66-279">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="99b66-280">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="99b66-280">partnerReportedThreatState</span></span>|[<span data-ttu-id="99b66-281">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="99b66-281">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="99b66-282">Gibt den Bedrohungsstatus eines Geräts an, wenn ein vom Konto und Gerät ein Mobile Threat Defense-Partner verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="99b66-282">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="99b66-283">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="99b66-283">Read Only.</span></span> <span data-ttu-id="99b66-284">Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="99b66-284">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="99b66-285">Antwort</span><span class="sxs-lookup"><span data-stu-id="99b66-285">Response</span></span>
<span data-ttu-id="99b66-286">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [managedDevice](../resources/intune-devices-manageddevice.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="99b66-286">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99b66-287">Beispiel</span><span class="sxs-lookup"><span data-stu-id="99b66-287">Example</span></span>

### <a name="request"></a><span data-ttu-id="99b66-288">Anforderung</span><span class="sxs-lookup"><span data-stu-id="99b66-288">Request</span></span>
<span data-ttu-id="99b66-289">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="99b66-289">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="99b66-290">Antwort</span><span class="sxs-lookup"><span data-stu-id="99b66-290">Response</span></span>
<span data-ttu-id="99b66-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99b66-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



