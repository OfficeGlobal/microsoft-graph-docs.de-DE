---
title: Aktualisieren von „managedDevice“
description: Aktualisieren der Eigenschaften eines managedDeviceOverview-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 56c45659d3e644a80d97f92ff6fe6659c4038d58
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967937"
---
# <a name="update-manageddevice"></a><span data-ttu-id="f77c6-103">Aktualisieren von „managedDevice“</span><span class="sxs-lookup"><span data-stu-id="f77c6-103">Update managedDevice</span></span>

> <span data-ttu-id="f77c6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f77c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f77c6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f77c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f77c6-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f77c6-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f77c6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f77c6-107">Prerequisites</span></span>
<span data-ttu-id="f77c6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f77c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f77c6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f77c6-110">Permission type</span></span>|<span data-ttu-id="f77c6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f77c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f77c6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f77c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f77c6-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f77c6-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f77c6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f77c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f77c6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f77c6-115">Not supported.</span></span>|
|<span data-ttu-id="f77c6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f77c6-116">Application</span></span>|<span data-ttu-id="f77c6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f77c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f77c6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f77c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="f77c6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f77c6-119">Request headers</span></span>
|<span data-ttu-id="f77c6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f77c6-120">Header</span></span>|<span data-ttu-id="f77c6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f77c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f77c6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f77c6-122">Authorization</span></span>|<span data-ttu-id="f77c6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f77c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f77c6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f77c6-124">Accept</span></span>|<span data-ttu-id="f77c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f77c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f77c6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f77c6-126">Request body</span></span>
<span data-ttu-id="f77c6-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDevice](../resources/intune-devices-manageddevice.md) an.</span><span class="sxs-lookup"><span data-stu-id="f77c6-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="f77c6-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDevice](../resources/intune-devices-manageddevice.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f77c6-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="f77c6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f77c6-129">Property</span></span>|<span data-ttu-id="f77c6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f77c6-130">Type</span></span>|<span data-ttu-id="f77c6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f77c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f77c6-132">id</span><span class="sxs-lookup"><span data-stu-id="f77c6-132">id</span></span>|<span data-ttu-id="f77c6-133">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-133">String</span></span>|<span data-ttu-id="f77c6-134">Eindeutiger Bezeichner für das Gerät</span><span class="sxs-lookup"><span data-stu-id="f77c6-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="f77c6-135">userId</span><span class="sxs-lookup"><span data-stu-id="f77c6-135">userId</span></span>|<span data-ttu-id="f77c6-136">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-136">String</span></span>|<span data-ttu-id="f77c6-137">Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="f77c6-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="f77c6-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="f77c6-138">deviceName</span></span>|<span data-ttu-id="f77c6-139">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-139">String</span></span>|<span data-ttu-id="f77c6-140">Der Name des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-140">Name of the device</span></span>|
|<span data-ttu-id="f77c6-141">Dem</span><span class="sxs-lookup"><span data-stu-id="f77c6-141">hardwareInformation</span></span>|[<span data-ttu-id="f77c6-142">Dem</span><span class="sxs-lookup"><span data-stu-id="f77c6-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="f77c6-143">Die hardward-Details für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="f77c6-143">The hardward details for the device.</span></span>  <span data-ttu-id="f77c6-144">Enthält Informationen wie Speicherplatz, Hersteller, Seriennummer usw.</span><span class="sxs-lookup"><span data-stu-id="f77c6-144">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="f77c6-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="f77c6-145">ownerType</span></span>|[<span data-ttu-id="f77c6-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="f77c6-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="f77c6-147">Der Besitzer des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-147">Ownership of the device.</span></span> <span data-ttu-id="f77c6-148">Kann "Company" oder "Personal" sein.</span><span class="sxs-lookup"><span data-stu-id="f77c6-148">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="f77c6-149">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="f77c6-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="f77c6-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="f77c6-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="f77c6-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="f77c6-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="f77c6-152">Der Besitzer des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-152">Ownership of the device.</span></span> <span data-ttu-id="f77c6-153">Kann "Company" oder "Personal" sein.</span><span class="sxs-lookup"><span data-stu-id="f77c6-153">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="f77c6-154">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="f77c6-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="f77c6-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="f77c6-155">deviceActionResults</span></span>|<span data-ttu-id="f77c6-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f77c6-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="f77c6-157">Liste von ComplexType DeviceActionResult-Objekten.</span><span class="sxs-lookup"><span data-stu-id="f77c6-157">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="f77c6-158">managementState</span><span class="sxs-lookup"><span data-stu-id="f77c6-158">managementState</span></span>|[<span data-ttu-id="f77c6-159">managementState</span><span class="sxs-lookup"><span data-stu-id="f77c6-159">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="f77c6-160">Verwaltungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-160">Management state of the device.</span></span> <span data-ttu-id="f77c6-161">Mögliche Werte sind: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled` und `discovered`.</span><span class="sxs-lookup"><span data-stu-id="f77c6-161">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="f77c6-162">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="f77c6-162">enrolledDateTime</span></span>|<span data-ttu-id="f77c6-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77c6-163">DateTimeOffset</span></span>|<span data-ttu-id="f77c6-164">Registrierungszeit des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-164">Enrollment time of the device.</span></span>|
|<span data-ttu-id="f77c6-165">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f77c6-165">lastSyncDateTime</span></span>|<span data-ttu-id="f77c6-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77c6-166">DateTimeOffset</span></span>|<span data-ttu-id="f77c6-167">Datum und Uhrzeit, zu dem bzw. der das Gerät zuletzt eine erfolgreiche Synchronisierung mit Intune durchgeführt hat.</span><span class="sxs-lookup"><span data-stu-id="f77c6-167">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="f77c6-168">chassitype</span><span class="sxs-lookup"><span data-stu-id="f77c6-168">chassisType</span></span>|[<span data-ttu-id="f77c6-169">chassitype</span><span class="sxs-lookup"><span data-stu-id="f77c6-169">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="f77c6-170">Gehäusetyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-170">Chassis type of the device.</span></span> <span data-ttu-id="f77c6-171">Mögliche Werte: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="f77c6-171">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="f77c6-172">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f77c6-172">operatingSystem</span></span>|<span data-ttu-id="f77c6-173">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-173">String</span></span>|<span data-ttu-id="f77c6-174">Betriebssystem des Geräts</span><span class="sxs-lookup"><span data-stu-id="f77c6-174">Operating system of the device.</span></span> <span data-ttu-id="f77c6-175">Windows, iOS, etc.</span><span class="sxs-lookup"><span data-stu-id="f77c6-175">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="f77c6-176">deviceType</span><span class="sxs-lookup"><span data-stu-id="f77c6-176">deviceType</span></span>|[<span data-ttu-id="f77c6-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="f77c6-177">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="f77c6-178">Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-178">Platform of the device.</span></span> <span data-ttu-id="f77c6-179">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f77c6-179">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="f77c6-180">complianceState</span><span class="sxs-lookup"><span data-stu-id="f77c6-180">complianceState</span></span>|[<span data-ttu-id="f77c6-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="f77c6-181">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="f77c6-182">Compliancestatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-182">Compliance state of the device.</span></span> <span data-ttu-id="f77c6-183">Mögliche Werte: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="f77c6-183">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="f77c6-184">jailBroken</span><span class="sxs-lookup"><span data-stu-id="f77c6-184">jailBroken</span></span>|<span data-ttu-id="f77c6-185">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-185">String</span></span>|<span data-ttu-id="f77c6-186">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="f77c6-186">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="f77c6-187">managementAgent</span><span class="sxs-lookup"><span data-stu-id="f77c6-187">managementAgent</span></span>|[<span data-ttu-id="f77c6-188">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="f77c6-188">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="f77c6-189">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-189">Management channel of the device.</span></span> <span data-ttu-id="f77c6-190">InTune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm` `intuneClient`,, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm` `configurationManagerClientMdmEas`,, `unknown`, `jamf` `googleCloudDevicePolicyController`,, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="f77c6-190">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="f77c6-191">osVersion</span><span class="sxs-lookup"><span data-stu-id="f77c6-191">osVersion</span></span>|<span data-ttu-id="f77c6-192">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-192">String</span></span>|<span data-ttu-id="f77c6-193">Betriebssystemversion auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="f77c6-193">Operating system version of the device.</span></span>|
|<span data-ttu-id="f77c6-194">easActivated</span><span class="sxs-lookup"><span data-stu-id="f77c6-194">easActivated</span></span>|<span data-ttu-id="f77c6-195">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f77c6-195">Boolean</span></span>|<span data-ttu-id="f77c6-196">Gibt an, ob das Gerät über Exchange ActiveSync-aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f77c6-196">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="f77c6-197">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="f77c6-197">easDeviceId</span></span>|<span data-ttu-id="f77c6-198">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-198">String</span></span>|<span data-ttu-id="f77c6-199">Exchange ActiveSync-ID des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-199">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="f77c6-200">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="f77c6-200">easActivationDateTime</span></span>|<span data-ttu-id="f77c6-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77c6-201">DateTimeOffset</span></span>|<span data-ttu-id="f77c6-202">Exchange ActivationSync-Aktivierungszeit des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-202">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="f77c6-203">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="f77c6-203">aadRegistered</span></span>|<span data-ttu-id="f77c6-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77c6-204">Boolean</span></span>|<span data-ttu-id="f77c6-205">Gibt an, ob das Gerät für Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="f77c6-205">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="f77c6-206">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="f77c6-206">azureADRegistered</span></span>|<span data-ttu-id="f77c6-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77c6-207">Boolean</span></span>|<span data-ttu-id="f77c6-208">Gibt an, ob das Gerät für Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="f77c6-208">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="f77c6-209">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f77c6-209">deviceEnrollmentType</span></span>|[<span data-ttu-id="f77c6-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f77c6-210">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="f77c6-211">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-211">Enrollment type of the device.</span></span> <span data-ttu-id="f77c6-212">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="f77c6-212">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="f77c6-213">lostModeState</span><span class="sxs-lookup"><span data-stu-id="f77c6-213">lostModeState</span></span>|[<span data-ttu-id="f77c6-214">lostModeState</span><span class="sxs-lookup"><span data-stu-id="f77c6-214">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="f77c6-215">Gibt an, ob der Modus verloren aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f77c6-215">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="f77c6-216">Mögliche Werte sind: `disabled` und `enabled`.</span><span class="sxs-lookup"><span data-stu-id="f77c6-216">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="f77c6-217">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="f77c6-217">activationLockBypassCode</span></span>|<span data-ttu-id="f77c6-218">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-218">String</span></span>|<span data-ttu-id="f77c6-219">Code, der ermöglicht, dass die Aktivierungssperre auf einem Gerät umgangen wird.</span><span class="sxs-lookup"><span data-stu-id="f77c6-219">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="f77c6-220">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f77c6-220">emailAddress</span></span>|<span data-ttu-id="f77c6-221">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-221">String</span></span>|<span data-ttu-id="f77c6-222">E-Mail(s) für den Benutzer, der dem Gerät zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="f77c6-222">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="f77c6-223">Eigenschaften azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="f77c6-223">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="f77c6-224">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-224">String</span></span>|<span data-ttu-id="f77c6-225">Die eindeutige ID für das Azure Active Directory-Gerät.</span><span class="sxs-lookup"><span data-stu-id="f77c6-225">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="f77c6-226">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f77c6-226">Read only.</span></span>|
|<span data-ttu-id="f77c6-227">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="f77c6-227">azureADDeviceId</span></span>|<span data-ttu-id="f77c6-228">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-228">String</span></span>|<span data-ttu-id="f77c6-229">Die eindeutige ID für das Azure Active Directory-Gerät.</span><span class="sxs-lookup"><span data-stu-id="f77c6-229">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="f77c6-230">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f77c6-230">Read only.</span></span>|
|<span data-ttu-id="f77c6-231">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f77c6-231">deviceRegistrationState</span></span>|[<span data-ttu-id="f77c6-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f77c6-232">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="f77c6-233">Geräteregistrierungsstatus</span><span class="sxs-lookup"><span data-stu-id="f77c6-233">Device registration state.</span></span> <span data-ttu-id="f77c6-234">Mögliche Werte: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f77c6-234">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="f77c6-235">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="f77c6-235">deviceCategoryDisplayName</span></span>|<span data-ttu-id="f77c6-236">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-236">String</span></span>|<span data-ttu-id="f77c6-237">Anzeigename der Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="f77c6-237">Device category display name</span></span>|
|<span data-ttu-id="f77c6-238">isSupervised</span><span class="sxs-lookup"><span data-stu-id="f77c6-238">isSupervised</span></span>|<span data-ttu-id="f77c6-239">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f77c6-239">Boolean</span></span>|<span data-ttu-id="f77c6-240">Überwachter Gerätestatus</span><span class="sxs-lookup"><span data-stu-id="f77c6-240">Device supervised status</span></span>|
|<span data-ttu-id="f77c6-241">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f77c6-241">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="f77c6-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77c6-242">DateTimeOffset</span></span>|<span data-ttu-id="f77c6-243">Letzter Zeitpunkt, zu dem das Gerät Exchange kontaktiert hat.</span><span class="sxs-lookup"><span data-stu-id="f77c6-243">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="f77c6-244">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="f77c6-244">exchangeAccessState</span></span>|[<span data-ttu-id="f77c6-245">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="f77c6-245">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="f77c6-246">Der Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="f77c6-246">The Access State of the device in Exchange.</span></span> <span data-ttu-id="f77c6-247">Mögliche Werte: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="f77c6-247">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="f77c6-248">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="f77c6-248">exchangeAccessStateReason</span></span>|[<span data-ttu-id="f77c6-249">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="f77c6-249">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="f77c6-250">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="f77c6-250">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="f77c6-251">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="f77c6-251">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="f77c6-252">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="f77c6-252">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="f77c6-253">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-253">String</span></span>|<span data-ttu-id="f77c6-254">Die URL, die ermöglicht, dass mit dem Gerät eine Remoteunterstützungssitzung eingerichtet wird.</span><span class="sxs-lookup"><span data-stu-id="f77c6-254">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="f77c6-255">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f77c6-255">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="f77c6-256">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-256">String</span></span>|<span data-ttu-id="f77c6-257">Eine Fehlerzeichenfolge, die Probleme beim Erstellen von Objekten für die Remoteunterstützungssitzung identifiziert.</span><span class="sxs-lookup"><span data-stu-id="f77c6-257">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="f77c6-258">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="f77c6-258">isEncrypted</span></span>|<span data-ttu-id="f77c6-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77c6-259">Boolean</span></span>|<span data-ttu-id="f77c6-260">Geräteverschlüsselungsstatus</span><span class="sxs-lookup"><span data-stu-id="f77c6-260">Device encryption status</span></span>|
|<span data-ttu-id="f77c6-261">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f77c6-261">userPrincipalName</span></span>|<span data-ttu-id="f77c6-262">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-262">String</span></span>|<span data-ttu-id="f77c6-263">Benutzerprinzipalname für das Gerät</span><span class="sxs-lookup"><span data-stu-id="f77c6-263">Device user principal name</span></span>|
|<span data-ttu-id="f77c6-264">model</span><span class="sxs-lookup"><span data-stu-id="f77c6-264">model</span></span>|<span data-ttu-id="f77c6-265">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-265">String</span></span>|<span data-ttu-id="f77c6-266">Das Modell des Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-266">Model of the device</span></span>|
|<span data-ttu-id="f77c6-267">Hersteller</span><span class="sxs-lookup"><span data-stu-id="f77c6-267">manufacturer</span></span>|<span data-ttu-id="f77c6-268">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-268">String</span></span>|<span data-ttu-id="f77c6-269">Hersteller des Geräts</span><span class="sxs-lookup"><span data-stu-id="f77c6-269">Manufacturer of the device</span></span>|
|<span data-ttu-id="f77c6-270">imei</span><span class="sxs-lookup"><span data-stu-id="f77c6-270">imei</span></span>|<span data-ttu-id="f77c6-271">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-271">String</span></span>|<span data-ttu-id="f77c6-272">IMEI</span><span class="sxs-lookup"><span data-stu-id="f77c6-272">IMEI</span></span>|
|<span data-ttu-id="f77c6-273">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f77c6-273">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f77c6-274">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77c6-274">DateTimeOffset</span></span>|<span data-ttu-id="f77c6-275">Datum und Uhrzeit des Ablaufs der Karenzzeit für die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="f77c6-275">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="f77c6-276">serialNumber</span><span class="sxs-lookup"><span data-stu-id="f77c6-276">serialNumber</span></span>|<span data-ttu-id="f77c6-277">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-277">String</span></span>|<span data-ttu-id="f77c6-278">SerialNumber</span><span class="sxs-lookup"><span data-stu-id="f77c6-278">SerialNumber</span></span>|
|<span data-ttu-id="f77c6-279">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="f77c6-279">phoneNumber</span></span>|<span data-ttu-id="f77c6-280">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-280">String</span></span>|<span data-ttu-id="f77c6-281">Telefonnummer des Geräts</span><span class="sxs-lookup"><span data-stu-id="f77c6-281">Phone number of the device</span></span>|
|<span data-ttu-id="f77c6-282">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="f77c6-282">androidSecurityPatchLevel</span></span>|<span data-ttu-id="f77c6-283">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-283">String</span></span>|<span data-ttu-id="f77c6-284">Sicherheitspatchlevel von Android</span><span class="sxs-lookup"><span data-stu-id="f77c6-284">Android security patch level</span></span>|
|<span data-ttu-id="f77c6-285">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f77c6-285">userDisplayName</span></span>|<span data-ttu-id="f77c6-286">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-286">String</span></span>|<span data-ttu-id="f77c6-287">Anzeigename des Benutzers</span><span class="sxs-lookup"><span data-stu-id="f77c6-287">User display name</span></span>|
|<span data-ttu-id="f77c6-288">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f77c6-288">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="f77c6-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f77c6-289">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="f77c6-290">Für ConfigrMgr-Client aktivierte Features</span><span class="sxs-lookup"><span data-stu-id="f77c6-290">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="f77c6-291">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="f77c6-291">wiFiMacAddress</span></span>|<span data-ttu-id="f77c6-292">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-292">String</span></span>|<span data-ttu-id="f77c6-293">Wi-Fi-MAC</span><span class="sxs-lookup"><span data-stu-id="f77c6-293">Wi-Fi MAC</span></span>|
|<span data-ttu-id="f77c6-294">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="f77c6-294">deviceHealthAttestationState</span></span>|[<span data-ttu-id="f77c6-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="f77c6-295">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="f77c6-296">Integritätsnachweis für Geräte – Status</span><span class="sxs-lookup"><span data-stu-id="f77c6-296">The device health attestation state.</span></span>|
|<span data-ttu-id="f77c6-297">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="f77c6-297">subscriberCarrier</span></span>|<span data-ttu-id="f77c6-298">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-298">String</span></span>|<span data-ttu-id="f77c6-299">Netzbetreiber des Abonnenten</span><span class="sxs-lookup"><span data-stu-id="f77c6-299">Subscriber Carrier</span></span>|
|<span data-ttu-id="f77c6-300">meid</span><span class="sxs-lookup"><span data-stu-id="f77c6-300">meid</span></span>|<span data-ttu-id="f77c6-301">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-301">String</span></span>|<span data-ttu-id="f77c6-302">MEID</span><span class="sxs-lookup"><span data-stu-id="f77c6-302">MEID</span></span>|
|<span data-ttu-id="f77c6-303">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="f77c6-303">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="f77c6-304">Int64</span><span class="sxs-lookup"><span data-stu-id="f77c6-304">Int64</span></span>|<span data-ttu-id="f77c6-305">Gesamtspeicher in Byte</span><span class="sxs-lookup"><span data-stu-id="f77c6-305">Total Storage in Bytes</span></span>|
|<span data-ttu-id="f77c6-306">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="f77c6-306">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="f77c6-307">Int64</span><span class="sxs-lookup"><span data-stu-id="f77c6-307">Int64</span></span>|<span data-ttu-id="f77c6-308">Freier Speicher in Byte</span><span class="sxs-lookup"><span data-stu-id="f77c6-308">Free Storage in Bytes</span></span>|
|<span data-ttu-id="f77c6-309">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="f77c6-309">managedDeviceName</span></span>|<span data-ttu-id="f77c6-310">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-310">String</span></span>|<span data-ttu-id="f77c6-311">Automatisch generierter Name zum Identifizieren eines Geräts.</span><span class="sxs-lookup"><span data-stu-id="f77c6-311">Automatically generated name to identify a device.</span></span> <span data-ttu-id="f77c6-312">Kann mit einem Anzeigenamen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="f77c6-312">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="f77c6-313">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="f77c6-313">partnerReportedThreatState</span></span>|[<span data-ttu-id="f77c6-314">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="f77c6-314">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="f77c6-315">Gibt den Bedrohungsstatus eines Geräts an, wenn ein vom Konto und Gerät ein Mobile Threat Defense-Partner verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f77c6-315">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="f77c6-316">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f77c6-316">Read Only.</span></span> <span data-ttu-id="f77c6-317">Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="f77c6-317">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="f77c6-318">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="f77c6-318">usersLoggedOn</span></span>|<span data-ttu-id="f77c6-319">[loggedOnUser](../resources/intune-devices-loggedonuser.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="f77c6-319">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="f77c6-320">Gibt die zuletzt angemeldeten Benutzer eines Geräts an.</span><span class="sxs-lookup"><span data-stu-id="f77c6-320">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="f77c6-321">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="f77c6-321">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="f77c6-322">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77c6-322">DateTimeOffset</span></span>|<span data-ttu-id="f77c6-323">Meldet den DateTime-Wert für die Einstellung preferMdmOverGroupPolicy.</span><span class="sxs-lookup"><span data-stu-id="f77c6-323">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="f77c6-324">Ist diese Einstellung festgelegt, überschreiben die Intune-MDM-Einstellungen Gruppenrichtlinieneinstellungen bei einem Konflikt.</span><span class="sxs-lookup"><span data-stu-id="f77c6-324">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="f77c6-325">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f77c6-325">Read Only.</span></span>|
|<span data-ttu-id="f77c6-326">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="f77c6-326">autopilotEnrolled</span></span>|<span data-ttu-id="f77c6-327">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f77c6-327">Boolean</span></span>|<span data-ttu-id="f77c6-328">Meldet, ob das verwaltete Gerät über Auto-Pilot registriert wird.</span><span class="sxs-lookup"><span data-stu-id="f77c6-328">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="f77c6-329">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="f77c6-329">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="f77c6-330">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f77c6-330">Boolean</span></span>|<span data-ttu-id="f77c6-331">Meldet, ob das verwaltete iOS-Gerät Benutzer Genehmigungs Registrierung ist.</span><span class="sxs-lookup"><span data-stu-id="f77c6-331">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="f77c6-332">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="f77c6-332">managementCertificateExpirationDate</span></span>|<span data-ttu-id="f77c6-333">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77c6-333">DateTimeOffset</span></span>|<span data-ttu-id="f77c6-334">Meldet Ablaufdatum für das Geräte Verwaltungszertifikat</span><span class="sxs-lookup"><span data-stu-id="f77c6-334">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="f77c6-335">ICCID</span><span class="sxs-lookup"><span data-stu-id="f77c6-335">iccid</span></span>|<span data-ttu-id="f77c6-336">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-336">String</span></span>|<span data-ttu-id="f77c6-337">Integrated Circuit Card Identifier, es ist die eindeutige Identifikationsnummer einer SIM-Karte.</span><span class="sxs-lookup"><span data-stu-id="f77c6-337">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="f77c6-338">UDID</span><span class="sxs-lookup"><span data-stu-id="f77c6-338">udid</span></span>|<span data-ttu-id="f77c6-339">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-339">String</span></span>|<span data-ttu-id="f77c6-340">Eindeutige Gerätekennung für iOS-und macOS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="f77c6-340">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="f77c6-341">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="f77c6-341">roleScopeTagIds</span></span>|<span data-ttu-id="f77c6-342">String collection</span><span class="sxs-lookup"><span data-stu-id="f77c6-342">String collection</span></span>|<span data-ttu-id="f77c6-343">Liste der Bereichstag-IDs für diese Geräteinstanz.</span><span class="sxs-lookup"><span data-stu-id="f77c6-343">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="f77c6-344">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="f77c6-344">windowsActiveMalwareCount</span></span>|<span data-ttu-id="f77c6-345">Int32</span><span class="sxs-lookup"><span data-stu-id="f77c6-345">Int32</span></span>|<span data-ttu-id="f77c6-346">Anzahl der aktiven Schadsoftware für dieses Windows-Gerät</span><span class="sxs-lookup"><span data-stu-id="f77c6-346">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="f77c6-347">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="f77c6-347">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="f77c6-348">Int32</span><span class="sxs-lookup"><span data-stu-id="f77c6-348">Int32</span></span>|<span data-ttu-id="f77c6-349">Anzahl der korrigierten Schadsoftware für dieses Windows-Gerät</span><span class="sxs-lookup"><span data-stu-id="f77c6-349">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="f77c6-350">notes</span><span class="sxs-lookup"><span data-stu-id="f77c6-350">notes</span></span>|<span data-ttu-id="f77c6-351">String</span><span class="sxs-lookup"><span data-stu-id="f77c6-351">String</span></span>|<span data-ttu-id="f77c6-352">Hinweise zu dem von IT-Administrator erstellten Gerät</span><span class="sxs-lookup"><span data-stu-id="f77c6-352">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="f77c6-353">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="f77c6-353">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="f77c6-354">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="f77c6-354">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="f77c6-355">Configuration Manager-Clientintegritätsstatus, nur gültig für Geräte, die vom MDM/ConfigMgr-Agent verwaltet werden</span><span class="sxs-lookup"><span data-stu-id="f77c6-355">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="f77c6-356">Antwort</span><span class="sxs-lookup"><span data-stu-id="f77c6-356">Response</span></span>
<span data-ttu-id="f77c6-357">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDevice](../resources/intune-devices-manageddevice.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f77c6-357">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f77c6-358">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f77c6-358">Example</span></span>

### <a name="request"></a><span data-ttu-id="f77c6-359">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f77c6-359">Request</span></span>
<span data-ttu-id="f77c6-360">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f77c6-360">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7224

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
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
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "partnerReportedThreatState": "activated",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```

### <a name="response"></a><span data-ttu-id="f77c6-361">Antwort</span><span class="sxs-lookup"><span data-stu-id="f77c6-361">Response</span></span>
<span data-ttu-id="f77c6-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f77c6-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7273

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
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
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "partnerReportedThreatState": "activated",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```




