---
title: Aktualisieren von „managedDevice“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDevice.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3711888ee2c5e6f3d3a5281ec6e14d521eb9695
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162468"
---
# <a name="update-manageddevice"></a><span data-ttu-id="b1926-103">Aktualisieren von „managedDevice“</span><span class="sxs-lookup"><span data-stu-id="b1926-103">Update managedDevice</span></span>

> <span data-ttu-id="b1926-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1926-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1926-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b1926-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1926-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="b1926-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1926-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b1926-107">Prerequisites</span></span>
<span data-ttu-id="b1926-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1926-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b1926-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1926-110">Permission type</span></span>|<span data-ttu-id="b1926-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1926-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1926-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1926-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1926-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1926-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b1926-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1926-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1926-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1926-115">Not supported.</span></span>|
|<span data-ttu-id="b1926-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1926-116">Application</span></span>|<span data-ttu-id="b1926-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1926-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1926-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1926-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b1926-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1926-119">Request headers</span></span>
|<span data-ttu-id="b1926-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b1926-120">Header</span></span>|<span data-ttu-id="b1926-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b1926-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1926-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1926-122">Authorization</span></span>|<span data-ttu-id="b1926-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b1926-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1926-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b1926-124">Accept</span></span>|<span data-ttu-id="b1926-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1926-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1926-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1926-126">Request body</span></span>
<span data-ttu-id="b1926-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDevice](../resources/intune-devices-manageddevice.md) an.</span><span class="sxs-lookup"><span data-stu-id="b1926-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="b1926-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDevice](../resources/intune-devices-manageddevice.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="b1926-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="b1926-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b1926-129">Property</span></span>|<span data-ttu-id="b1926-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b1926-130">Type</span></span>|<span data-ttu-id="b1926-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1926-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1926-132">id</span><span class="sxs-lookup"><span data-stu-id="b1926-132">id</span></span>|<span data-ttu-id="b1926-133">string</span><span class="sxs-lookup"><span data-stu-id="b1926-133">String</span></span>|<span data-ttu-id="b1926-134">Eindeutiger Bezeichner für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="b1926-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="b1926-135">userId</span><span class="sxs-lookup"><span data-stu-id="b1926-135">userId</span></span>|<span data-ttu-id="b1926-136">String</span><span class="sxs-lookup"><span data-stu-id="b1926-136">String</span></span>|<span data-ttu-id="b1926-137">Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="b1926-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="b1926-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="b1926-138">deviceName</span></span>|<span data-ttu-id="b1926-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-139">String</span></span>|<span data-ttu-id="b1926-140">Name des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="b1926-140">Name of the device</span></span>|
|<span data-ttu-id="b1926-141">Dem</span><span class="sxs-lookup"><span data-stu-id="b1926-141">hardwareInformation</span></span>|[<span data-ttu-id="b1926-142">Dem</span><span class="sxs-lookup"><span data-stu-id="b1926-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="b1926-143">Die hardward-Details für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="b1926-143">The hardward details for the device.</span></span>  <span data-ttu-id="b1926-144">Enthält Informationen wie Speicherplatz, Hersteller, Seriennummer usw.</span><span class="sxs-lookup"><span data-stu-id="b1926-144">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="b1926-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="b1926-145">ownerType</span></span>|[<span data-ttu-id="b1926-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="b1926-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="b1926-147">Der Besitzer des Geräts.</span><span class="sxs-lookup"><span data-stu-id="b1926-147">Ownership of the device.</span></span> <span data-ttu-id="b1926-148">Kann "Company" oder "Personal" sein.</span><span class="sxs-lookup"><span data-stu-id="b1926-148">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="b1926-149">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="b1926-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="b1926-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="b1926-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="b1926-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="b1926-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="b1926-152">Der Besitzer des Geräts.</span><span class="sxs-lookup"><span data-stu-id="b1926-152">Ownership of the device.</span></span> <span data-ttu-id="b1926-153">Kann "Company" oder "Personal" sein.</span><span class="sxs-lookup"><span data-stu-id="b1926-153">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="b1926-154">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="b1926-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="b1926-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="b1926-155">deviceActionResults</span></span>|<span data-ttu-id="b1926-156">Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b1926-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="b1926-157">Liste von Objekten des Typs „ComplexType deviceActionResult“.
</span><span class="sxs-lookup"><span data-stu-id="b1926-157">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="b1926-158">managementState</span><span class="sxs-lookup"><span data-stu-id="b1926-158">managementState</span></span>|[<span data-ttu-id="b1926-159">managementState</span><span class="sxs-lookup"><span data-stu-id="b1926-159">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="b1926-160">Verwaltungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="b1926-160">Management state of the device.</span></span> <span data-ttu-id="b1926-161">Mögliche Werte sind: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled` und `discovered`.</span><span class="sxs-lookup"><span data-stu-id="b1926-161">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="b1926-162">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="b1926-162">enrolledDateTime</span></span>|<span data-ttu-id="b1926-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1926-163">DateTimeOffset</span></span>|<span data-ttu-id="b1926-164">Datum und Uhrzeit der Geräteregistrierung.
</span><span class="sxs-lookup"><span data-stu-id="b1926-164">Enrollment time of the device.</span></span>|
|<span data-ttu-id="b1926-165">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b1926-165">lastSyncDateTime</span></span>|<span data-ttu-id="b1926-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1926-166">DateTimeOffset</span></span>|<span data-ttu-id="b1926-167">Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
</span><span class="sxs-lookup"><span data-stu-id="b1926-167">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="b1926-168">chassitype</span><span class="sxs-lookup"><span data-stu-id="b1926-168">chassisType</span></span>|[<span data-ttu-id="b1926-169">chassitype</span><span class="sxs-lookup"><span data-stu-id="b1926-169">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="b1926-170">Gehäusetyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="b1926-170">Chassis type of the device.</span></span> <span data-ttu-id="b1926-171">Mögliche Werte: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="b1926-171">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="b1926-172">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b1926-172">operatingSystem</span></span>|<span data-ttu-id="b1926-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-173">String</span></span>|<span data-ttu-id="b1926-174">Betriebssystem des Geräts.</span><span class="sxs-lookup"><span data-stu-id="b1926-174">Operating system of the device.</span></span> <span data-ttu-id="b1926-175">Windows, iOS usw.</span><span class="sxs-lookup"><span data-stu-id="b1926-175">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="b1926-176">deviceType</span><span class="sxs-lookup"><span data-stu-id="b1926-176">deviceType</span></span>|[<span data-ttu-id="b1926-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="b1926-177">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="b1926-178">Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="b1926-178">Platform of the device.</span></span> <span data-ttu-id="b1926-179">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b1926-179">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="b1926-180">complianceState</span><span class="sxs-lookup"><span data-stu-id="b1926-180">complianceState</span></span>|[<span data-ttu-id="b1926-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="b1926-181">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="b1926-182">Konformitätsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="b1926-182">Compliance state of the device.</span></span> <span data-ttu-id="b1926-183">Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.</span><span class="sxs-lookup"><span data-stu-id="b1926-183">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="b1926-184">jailBroken</span><span class="sxs-lookup"><span data-stu-id="b1926-184">jailBroken</span></span>|<span data-ttu-id="b1926-185">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-185">String</span></span>|<span data-ttu-id="b1926-186">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="b1926-186">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="b1926-187">managementAgent</span><span class="sxs-lookup"><span data-stu-id="b1926-187">managementAgent</span></span>|[<span data-ttu-id="b1926-188">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="b1926-188">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="b1926-189">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="b1926-189">Management channel of the device.</span></span> <span data-ttu-id="b1926-190">InTune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm` `intuneClient`,, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm` `configurationManagerClientMdmEas`,, `unknown`, `jamf` `googleCloudDevicePolicyController`,, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="b1926-190">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="b1926-191">osVersion</span><span class="sxs-lookup"><span data-stu-id="b1926-191">osVersion</span></span>|<span data-ttu-id="b1926-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-192">String</span></span>|<span data-ttu-id="b1926-193">Auf dem Gerät installierte Betriebssystemversion.
</span><span class="sxs-lookup"><span data-stu-id="b1926-193">Operating system version of the device.</span></span>|
|<span data-ttu-id="b1926-194">easActivated</span><span class="sxs-lookup"><span data-stu-id="b1926-194">easActivated</span></span>|<span data-ttu-id="b1926-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1926-195">Boolean</span></span>|<span data-ttu-id="b1926-196">Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b1926-196">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="b1926-197">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="b1926-197">easDeviceId</span></span>|<span data-ttu-id="b1926-198">String</span><span class="sxs-lookup"><span data-stu-id="b1926-198">String</span></span>|<span data-ttu-id="b1926-199">Exchange ActiveSync-ID des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="b1926-199">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="b1926-200">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="b1926-200">easActivationDateTime</span></span>|<span data-ttu-id="b1926-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1926-201">DateTimeOffset</span></span>|<span data-ttu-id="b1926-202">Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="b1926-202">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="b1926-203">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="b1926-203">aadRegistered</span></span>|<span data-ttu-id="b1926-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1926-204">Boolean</span></span>|<span data-ttu-id="b1926-205">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="b1926-205">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="b1926-206">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="b1926-206">azureADRegistered</span></span>|<span data-ttu-id="b1926-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1926-207">Boolean</span></span>|<span data-ttu-id="b1926-208">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="b1926-208">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="b1926-209">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b1926-209">deviceEnrollmentType</span></span>|[<span data-ttu-id="b1926-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b1926-210">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="b1926-211">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="b1926-211">Enrollment type of the device.</span></span> <span data-ttu-id="b1926-212">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="b1926-212">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="b1926-213">lostModeState</span><span class="sxs-lookup"><span data-stu-id="b1926-213">lostModeState</span></span>|[<span data-ttu-id="b1926-214">lostModeState</span><span class="sxs-lookup"><span data-stu-id="b1926-214">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="b1926-215">Gibt an, ob der Modus verloren aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b1926-215">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="b1926-216">Mögliche Werte sind: `disabled` und `enabled`.</span><span class="sxs-lookup"><span data-stu-id="b1926-216">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="b1926-217">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="b1926-217">activationLockBypassCode</span></span>|<span data-ttu-id="b1926-218">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-218">String</span></span>|<span data-ttu-id="b1926-219">Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht</span><span class="sxs-lookup"><span data-stu-id="b1926-219">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="b1926-220">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b1926-220">emailAddress</span></span>|<span data-ttu-id="b1926-221">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-221">String</span></span>|<span data-ttu-id="b1926-222">E-Mail-Adressen des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="b1926-222">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="b1926-223">Eigenschaften azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="b1926-223">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="b1926-224">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-224">String</span></span>|<span data-ttu-id="b1926-225">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="b1926-225">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="b1926-226">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b1926-226">Read only.</span></span>|
|<span data-ttu-id="b1926-227">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="b1926-227">azureADDeviceId</span></span>|<span data-ttu-id="b1926-228">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-228">String</span></span>|<span data-ttu-id="b1926-229">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="b1926-229">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="b1926-230">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b1926-230">Read only.</span></span>|
|<span data-ttu-id="b1926-231">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="b1926-231">deviceRegistrationState</span></span>|[<span data-ttu-id="b1926-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="b1926-232">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="b1926-233">Registrierungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="b1926-233">Device registration state.</span></span> <span data-ttu-id="b1926-234">Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b1926-234">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="b1926-235">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="b1926-235">deviceCategoryDisplayName</span></span>|<span data-ttu-id="b1926-236">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-236">String</span></span>|<span data-ttu-id="b1926-237">Anzeigename der Gerätekategorie.
</span><span class="sxs-lookup"><span data-stu-id="b1926-237">Device category display name</span></span>|
|<span data-ttu-id="b1926-238">isSupervised</span><span class="sxs-lookup"><span data-stu-id="b1926-238">isSupervised</span></span>|<span data-ttu-id="b1926-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1926-239">Boolean</span></span>|<span data-ttu-id="b1926-240">Überwachungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="b1926-240">Device supervised status</span></span>|
|<span data-ttu-id="b1926-241">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b1926-241">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="b1926-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1926-242">DateTimeOffset</span></span>|<span data-ttu-id="b1926-243">Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange</span><span class="sxs-lookup"><span data-stu-id="b1926-243">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="b1926-244">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="b1926-244">exchangeAccessState</span></span>|[<span data-ttu-id="b1926-245">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="b1926-245">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="b1926-246">Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="b1926-246">The Access State of the device in Exchange.</span></span> <span data-ttu-id="b1926-247">Mögliche Werte: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="b1926-247">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="b1926-248">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="b1926-248">exchangeAccessStateReason</span></span>|[<span data-ttu-id="b1926-249">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="b1926-249">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="b1926-250">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="b1926-250">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="b1926-251">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="b1926-251">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="b1926-252">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="b1926-252">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="b1926-253">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-253">String</span></span>|<span data-ttu-id="b1926-254">URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
</span><span class="sxs-lookup"><span data-stu-id="b1926-254">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="b1926-255">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="b1926-255">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="b1926-256">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-256">String</span></span>|<span data-ttu-id="b1926-257">Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
</span><span class="sxs-lookup"><span data-stu-id="b1926-257">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="b1926-258">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="b1926-258">isEncrypted</span></span>|<span data-ttu-id="b1926-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1926-259">Boolean</span></span>|<span data-ttu-id="b1926-260">Verschlüsselungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="b1926-260">Device encryption status</span></span>|
|<span data-ttu-id="b1926-261">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1926-261">userPrincipalName</span></span>|<span data-ttu-id="b1926-262">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-262">String</span></span>|<span data-ttu-id="b1926-263">Benutzerprinzipalname für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="b1926-263">Device user principal name</span></span>|
|<span data-ttu-id="b1926-264">model</span><span class="sxs-lookup"><span data-stu-id="b1926-264">model</span></span>|<span data-ttu-id="b1926-265">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-265">String</span></span>|<span data-ttu-id="b1926-266">Modell des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="b1926-266">Model of the device</span></span>|
|<span data-ttu-id="b1926-267">manufacturer</span><span class="sxs-lookup"><span data-stu-id="b1926-267">manufacturer</span></span>|<span data-ttu-id="b1926-268">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-268">String</span></span>|<span data-ttu-id="b1926-269">Hersteller des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="b1926-269">Manufacturer of the device</span></span>|
|<span data-ttu-id="b1926-270">imei</span><span class="sxs-lookup"><span data-stu-id="b1926-270">imei</span></span>|<span data-ttu-id="b1926-271">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-271">String</span></span>|<span data-ttu-id="b1926-272">IMEI</span><span class="sxs-lookup"><span data-stu-id="b1926-272">IMEI</span></span>|
|<span data-ttu-id="b1926-273">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b1926-273">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b1926-274">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1926-274">DateTimeOffset</span></span>|<span data-ttu-id="b1926-275">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität.
</span><span class="sxs-lookup"><span data-stu-id="b1926-275">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="b1926-276">serialNumber</span><span class="sxs-lookup"><span data-stu-id="b1926-276">serialNumber</span></span>|<span data-ttu-id="b1926-277">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-277">String</span></span>|<span data-ttu-id="b1926-278">Seriennummer.
</span><span class="sxs-lookup"><span data-stu-id="b1926-278">SerialNumber</span></span>|
|<span data-ttu-id="b1926-279">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="b1926-279">phoneNumber</span></span>|<span data-ttu-id="b1926-280">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-280">String</span></span>|<span data-ttu-id="b1926-281">Telefonnummer des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="b1926-281">Phone number of the device</span></span>|
|<span data-ttu-id="b1926-282">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="b1926-282">androidSecurityPatchLevel</span></span>|<span data-ttu-id="b1926-283">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-283">String</span></span>|<span data-ttu-id="b1926-284">Android-Sicherheitspatchlevel.
</span><span class="sxs-lookup"><span data-stu-id="b1926-284">Android security patch level</span></span>|
|<span data-ttu-id="b1926-285">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b1926-285">userDisplayName</span></span>|<span data-ttu-id="b1926-286">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-286">String</span></span>|<span data-ttu-id="b1926-287">Anzeigename des Benutzers.
</span><span class="sxs-lookup"><span data-stu-id="b1926-287">User display name</span></span>|
|<span data-ttu-id="b1926-288">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="b1926-288">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="b1926-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="b1926-289">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="b1926-290">Aktivierte Funktionen des Konfigurations-Manager-Clients.
</span><span class="sxs-lookup"><span data-stu-id="b1926-290">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="b1926-291">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="b1926-291">wiFiMacAddress</span></span>|<span data-ttu-id="b1926-292">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-292">String</span></span>|<span data-ttu-id="b1926-293">WLAN-MAC</span><span class="sxs-lookup"><span data-stu-id="b1926-293">Wi-Fi MAC</span></span>|
|<span data-ttu-id="b1926-294">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="b1926-294">deviceHealthAttestationState</span></span>|[<span data-ttu-id="b1926-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="b1926-295">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="b1926-296">Status des Integritätsnachweises für Geräte.
</span><span class="sxs-lookup"><span data-stu-id="b1926-296">The device health attestation state.</span></span>|
|<span data-ttu-id="b1926-297">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="b1926-297">subscriberCarrier</span></span>|<span data-ttu-id="b1926-298">String</span><span class="sxs-lookup"><span data-stu-id="b1926-298">String</span></span>|<span data-ttu-id="b1926-299">Netzbetreiber des Abonnenten.
</span><span class="sxs-lookup"><span data-stu-id="b1926-299">Subscriber Carrier</span></span>|
|<span data-ttu-id="b1926-300">meid</span><span class="sxs-lookup"><span data-stu-id="b1926-300">meid</span></span>|<span data-ttu-id="b1926-301">String</span><span class="sxs-lookup"><span data-stu-id="b1926-301">String</span></span>|<span data-ttu-id="b1926-302">MEID</span><span class="sxs-lookup"><span data-stu-id="b1926-302">MEID</span></span>|
|<span data-ttu-id="b1926-303">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="b1926-303">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="b1926-304">Int64</span><span class="sxs-lookup"><span data-stu-id="b1926-304">Int64</span></span>|<span data-ttu-id="b1926-305">Gesamtspeicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="b1926-305">Total Storage in Bytes</span></span>|
|<span data-ttu-id="b1926-306">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="b1926-306">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="b1926-307">Int64</span><span class="sxs-lookup"><span data-stu-id="b1926-307">Int64</span></span>|<span data-ttu-id="b1926-308">Freier Speicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="b1926-308">Free Storage in Bytes</span></span>|
|<span data-ttu-id="b1926-309">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="b1926-309">managedDeviceName</span></span>|<span data-ttu-id="b1926-310">String</span><span class="sxs-lookup"><span data-stu-id="b1926-310">String</span></span>|<span data-ttu-id="b1926-311">Automatisch generierter Name zur Identifizierung des Geräts.</span><span class="sxs-lookup"><span data-stu-id="b1926-311">Automatically generated name to identify a device.</span></span> <span data-ttu-id="b1926-312">Kann mit einem benutzerfreundlichen Namen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="b1926-312">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="b1926-313">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="b1926-313">partnerReportedThreatState</span></span>|[<span data-ttu-id="b1926-314">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="b1926-314">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="b1926-315">Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen.</span><span class="sxs-lookup"><span data-stu-id="b1926-315">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="b1926-316">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b1926-316">Read Only.</span></span> <span data-ttu-id="b1926-317">Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="b1926-317">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="b1926-318">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="b1926-318">usersLoggedOn</span></span>|<span data-ttu-id="b1926-319">[loggedOnUser](../resources/intune-devices-loggedonuser.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="b1926-319">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="b1926-320">Gibt die zuletzt angemeldeten Benutzer eines Geräts an.</span><span class="sxs-lookup"><span data-stu-id="b1926-320">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="b1926-321">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1926-321">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="b1926-322">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1926-322">DateTimeOffset</span></span>|<span data-ttu-id="b1926-323">Meldet den DateTime-Wert für die Einstellung preferMdmOverGroupPolicy.</span><span class="sxs-lookup"><span data-stu-id="b1926-323">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="b1926-324">Ist diese Einstellung festgelegt, überschreiben die Intune-MDM-Einstellungen Gruppenrichtlinieneinstellungen bei einem Konflikt.</span><span class="sxs-lookup"><span data-stu-id="b1926-324">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="b1926-325">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b1926-325">Read Only.</span></span>|
|<span data-ttu-id="b1926-326">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="b1926-326">autopilotEnrolled</span></span>|<span data-ttu-id="b1926-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1926-327">Boolean</span></span>|<span data-ttu-id="b1926-328">Meldet, ob das verwaltete Gerät über Auto-Pilot registriert wird.</span><span class="sxs-lookup"><span data-stu-id="b1926-328">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="b1926-329">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="b1926-329">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="b1926-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1926-330">Boolean</span></span>|<span data-ttu-id="b1926-331">Meldet, ob das verwaltete iOS-Gerät Benutzer Genehmigungs Registrierung ist.</span><span class="sxs-lookup"><span data-stu-id="b1926-331">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="b1926-332">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="b1926-332">managementCertificateExpirationDate</span></span>|<span data-ttu-id="b1926-333">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1926-333">DateTimeOffset</span></span>|<span data-ttu-id="b1926-334">Meldet Ablaufdatum für das Geräte Verwaltungszertifikat</span><span class="sxs-lookup"><span data-stu-id="b1926-334">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="b1926-335">ICCID</span><span class="sxs-lookup"><span data-stu-id="b1926-335">iccid</span></span>|<span data-ttu-id="b1926-336">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-336">String</span></span>|<span data-ttu-id="b1926-337">Integrated Circuit Card Identifier, es ist die eindeutige Identifikationsnummer einer SIM-Karte.</span><span class="sxs-lookup"><span data-stu-id="b1926-337">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="b1926-338">UDID</span><span class="sxs-lookup"><span data-stu-id="b1926-338">udid</span></span>|<span data-ttu-id="b1926-339">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-339">String</span></span>|<span data-ttu-id="b1926-340">Eindeutige Gerätekennung für iOS-und macOS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="b1926-340">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="b1926-341">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="b1926-341">roleScopeTagIds</span></span>|<span data-ttu-id="b1926-342">String collection</span><span class="sxs-lookup"><span data-stu-id="b1926-342">String collection</span></span>|<span data-ttu-id="b1926-343">Liste der Bereichstag-IDs für diese Geräteinstanz.</span><span class="sxs-lookup"><span data-stu-id="b1926-343">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="b1926-344">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="b1926-344">windowsActiveMalwareCount</span></span>|<span data-ttu-id="b1926-345">Int32</span><span class="sxs-lookup"><span data-stu-id="b1926-345">Int32</span></span>|<span data-ttu-id="b1926-346">Anzahl der aktiven Schadsoftware für dieses Windows-Gerät</span><span class="sxs-lookup"><span data-stu-id="b1926-346">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="b1926-347">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="b1926-347">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="b1926-348">Int32</span><span class="sxs-lookup"><span data-stu-id="b1926-348">Int32</span></span>|<span data-ttu-id="b1926-349">Anzahl der korrigierten Schadsoftware für dieses Windows-Gerät</span><span class="sxs-lookup"><span data-stu-id="b1926-349">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="b1926-350">notes</span><span class="sxs-lookup"><span data-stu-id="b1926-350">notes</span></span>|<span data-ttu-id="b1926-351">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b1926-351">String</span></span>|<span data-ttu-id="b1926-352">Hinweise zu dem von IT-Administrator erstellten Gerät</span><span class="sxs-lookup"><span data-stu-id="b1926-352">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="b1926-353">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="b1926-353">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="b1926-354">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="b1926-354">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="b1926-355">Configuration Manager-Clientintegritätsstatus, nur gültig für Geräte, die vom MDM/ConfigMgr-Agent verwaltet werden</span><span class="sxs-lookup"><span data-stu-id="b1926-355">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="b1926-356">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1926-356">Response</span></span>
<span data-ttu-id="b1926-357">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDevice](../resources/intune-devices-manageddevice.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b1926-357">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1926-358">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1926-358">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1926-359">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1926-359">Request</span></span>
<span data-ttu-id="b1926-360">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1926-360">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1926-361">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1926-361">Response</span></span>
<span data-ttu-id="b1926-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1926-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




