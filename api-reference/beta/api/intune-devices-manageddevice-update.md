---
title: Aktualisieren von „managedDevice“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDevice.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 525623c99d8f3238ee548e634bc7ffe2c3162111
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404386"
---
# <a name="update-manageddevice"></a><span data-ttu-id="312c4-103">Aktualisieren von „managedDevice“</span><span class="sxs-lookup"><span data-stu-id="312c4-103">Update managedDevice</span></span>

> <span data-ttu-id="312c4-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="312c4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="312c4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="312c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="312c4-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="312c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="312c4-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="312c4-107">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="312c4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="312c4-108">Prerequisites</span></span>
<span data-ttu-id="312c4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="312c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="312c4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="312c4-111">Permission type</span></span>|<span data-ttu-id="312c4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="312c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="312c4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="312c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="312c4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="312c4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="312c4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="312c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="312c4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="312c4-116">Not supported.</span></span>|
|<span data-ttu-id="312c4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="312c4-117">Application</span></span>|<span data-ttu-id="312c4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="312c4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="312c4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="312c4-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="312c4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="312c4-120">Request headers</span></span>
|<span data-ttu-id="312c4-121">Header</span><span class="sxs-lookup"><span data-stu-id="312c4-121">Header</span></span>|<span data-ttu-id="312c4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="312c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="312c4-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="312c4-123">Authorization</span></span>|<span data-ttu-id="312c4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="312c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="312c4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="312c4-125">Accept</span></span>|<span data-ttu-id="312c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="312c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="312c4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="312c4-127">Request body</span></span>
<span data-ttu-id="312c4-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDevice](../resources/intune-devices-manageddevice.md) an.</span><span class="sxs-lookup"><span data-stu-id="312c4-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="312c4-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDevice](../resources/intune-devices-manageddevice.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="312c4-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="312c4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="312c4-130">Property</span></span>|<span data-ttu-id="312c4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="312c4-131">Type</span></span>|<span data-ttu-id="312c4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="312c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="312c4-133">id</span><span class="sxs-lookup"><span data-stu-id="312c4-133">id</span></span>|<span data-ttu-id="312c4-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-134">String</span></span>|<span data-ttu-id="312c4-135">Eindeutiger Bezeichner für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="312c4-135">Unique Identifier for the device</span></span>|
|<span data-ttu-id="312c4-136">userId</span><span class="sxs-lookup"><span data-stu-id="312c4-136">userId</span></span>|<span data-ttu-id="312c4-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-137">String</span></span>|<span data-ttu-id="312c4-138">Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="312c4-138">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="312c4-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="312c4-139">deviceName</span></span>|<span data-ttu-id="312c4-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-140">String</span></span>|<span data-ttu-id="312c4-141">Name des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="312c4-141">Name of the device</span></span>|
|<span data-ttu-id="312c4-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="312c4-142">hardwareInformation</span></span>|[<span data-ttu-id="312c4-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="312c4-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="312c4-144">Die Hardward Details für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="312c4-144">The hardward details for the device.</span></span>  <span data-ttu-id="312c4-145">Enthält Informationen, wie Speicherplatz, Hersteller, Seriennummer.</span><span class="sxs-lookup"><span data-stu-id="312c4-145">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="312c4-146">Besitzertyp</span><span class="sxs-lookup"><span data-stu-id="312c4-146">ownerType</span></span>|[<span data-ttu-id="312c4-147">Besitzertyp</span><span class="sxs-lookup"><span data-stu-id="312c4-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="312c4-148">Besitz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-148">Ownership of the device.</span></span> <span data-ttu-id="312c4-149">'Company' oder 'Privat' kann sein.</span><span class="sxs-lookup"><span data-stu-id="312c4-149">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="312c4-150">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="312c4-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="312c4-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="312c4-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="312c4-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="312c4-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="312c4-153">Besitz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-153">Ownership of the device.</span></span> <span data-ttu-id="312c4-154">'Company' oder 'Privat' kann sein.</span><span class="sxs-lookup"><span data-stu-id="312c4-154">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="312c4-155">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="312c4-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="312c4-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="312c4-156">deviceActionResults</span></span>|<span data-ttu-id="312c4-157">Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="312c4-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="312c4-158">Liste von Objekten des Typs „ComplexType deviceActionResult“.
</span><span class="sxs-lookup"><span data-stu-id="312c4-158">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="312c4-159">managementState</span><span class="sxs-lookup"><span data-stu-id="312c4-159">managementState</span></span>|[<span data-ttu-id="312c4-160">managementState</span><span class="sxs-lookup"><span data-stu-id="312c4-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="312c4-161">Verwaltungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-161">Management state of the device.</span></span> <span data-ttu-id="312c4-162">Mögliche Werte sind: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled` und `discovered`.</span><span class="sxs-lookup"><span data-stu-id="312c4-162">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="312c4-163">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="312c4-163">enrolledDateTime</span></span>|<span data-ttu-id="312c4-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="312c4-164">DateTimeOffset</span></span>|<span data-ttu-id="312c4-165">Datum und Uhrzeit der Geräteregistrierung.
</span><span class="sxs-lookup"><span data-stu-id="312c4-165">Enrollment time of the device.</span></span>|
|<span data-ttu-id="312c4-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="312c4-166">lastSyncDateTime</span></span>|<span data-ttu-id="312c4-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="312c4-167">DateTimeOffset</span></span>|<span data-ttu-id="312c4-168">Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
</span><span class="sxs-lookup"><span data-stu-id="312c4-168">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="312c4-169">chassisType</span><span class="sxs-lookup"><span data-stu-id="312c4-169">chassisType</span></span>|[<span data-ttu-id="312c4-170">chassisType</span><span class="sxs-lookup"><span data-stu-id="312c4-170">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="312c4-171">Chassistyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-171">Chassis type of the device.</span></span> <span data-ttu-id="312c4-172">Mögliche Werte: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="312c4-172">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="312c4-173">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="312c4-173">operatingSystem</span></span>|<span data-ttu-id="312c4-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-174">String</span></span>|<span data-ttu-id="312c4-175">Betriebssystem des Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-175">Operating system of the device.</span></span> <span data-ttu-id="312c4-176">Windows, iOS usw.</span><span class="sxs-lookup"><span data-stu-id="312c4-176">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="312c4-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="312c4-177">deviceType</span></span>|[<span data-ttu-id="312c4-178">deviceType</span><span class="sxs-lookup"><span data-stu-id="312c4-178">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="312c4-179">Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-179">Platform of the device.</span></span> <span data-ttu-id="312c4-180">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="312c4-180">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="312c4-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="312c4-181">complianceState</span></span>|[<span data-ttu-id="312c4-182">complianceState</span><span class="sxs-lookup"><span data-stu-id="312c4-182">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="312c4-183">Konformitätsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-183">Compliance state of the device.</span></span> <span data-ttu-id="312c4-184">Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.</span><span class="sxs-lookup"><span data-stu-id="312c4-184">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="312c4-185">jailBroken</span><span class="sxs-lookup"><span data-stu-id="312c4-185">jailBroken</span></span>|<span data-ttu-id="312c4-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-186">String</span></span>|<span data-ttu-id="312c4-187">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="312c4-187">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="312c4-188">managementAgent</span><span class="sxs-lookup"><span data-stu-id="312c4-188">managementAgent</span></span>|[<span data-ttu-id="312c4-189">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="312c4-189">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="312c4-190">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-190">Management channel of the device.</span></span> <span data-ttu-id="312c4-191">Intune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="312c4-191">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="312c4-192">osVersion</span><span class="sxs-lookup"><span data-stu-id="312c4-192">osVersion</span></span>|<span data-ttu-id="312c4-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-193">String</span></span>|<span data-ttu-id="312c4-194">Auf dem Gerät installierte Betriebssystemversion.
</span><span class="sxs-lookup"><span data-stu-id="312c4-194">Operating system version of the device.</span></span>|
|<span data-ttu-id="312c4-195">easActivated</span><span class="sxs-lookup"><span data-stu-id="312c4-195">easActivated</span></span>|<span data-ttu-id="312c4-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="312c4-196">Boolean</span></span>|<span data-ttu-id="312c4-197">Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="312c4-197">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="312c4-198">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="312c4-198">easDeviceId</span></span>|<span data-ttu-id="312c4-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-199">String</span></span>|<span data-ttu-id="312c4-200">Exchange ActiveSync-ID des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="312c4-200">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="312c4-201">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="312c4-201">easActivationDateTime</span></span>|<span data-ttu-id="312c4-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="312c4-202">DateTimeOffset</span></span>|<span data-ttu-id="312c4-203">Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="312c4-203">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="312c4-204">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="312c4-204">aadRegistered</span></span>|<span data-ttu-id="312c4-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="312c4-205">Boolean</span></span>|<span data-ttu-id="312c4-206">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="312c4-206">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="312c4-207">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="312c4-207">azureADRegistered</span></span>|<span data-ttu-id="312c4-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="312c4-208">Boolean</span></span>|<span data-ttu-id="312c4-209">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="312c4-209">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="312c4-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="312c4-210">deviceEnrollmentType</span></span>|[<span data-ttu-id="312c4-211">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="312c4-211">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="312c4-212">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-212">Enrollment type of the device.</span></span> <span data-ttu-id="312c4-213">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="312c4-213">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="312c4-214">lostModeState</span><span class="sxs-lookup"><span data-stu-id="312c4-214">lostModeState</span></span>|[<span data-ttu-id="312c4-215">lostModeState</span><span class="sxs-lookup"><span data-stu-id="312c4-215">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="312c4-216">Gibt an, ob verloren-Modus aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="312c4-216">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="312c4-217">Mögliche Werte sind: `disabled` und `enabled`.</span><span class="sxs-lookup"><span data-stu-id="312c4-217">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="312c4-218">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="312c4-218">activationLockBypassCode</span></span>|<span data-ttu-id="312c4-219">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-219">String</span></span>|<span data-ttu-id="312c4-220">Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht</span><span class="sxs-lookup"><span data-stu-id="312c4-220">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="312c4-221">emailAddress</span><span class="sxs-lookup"><span data-stu-id="312c4-221">emailAddress</span></span>|<span data-ttu-id="312c4-222">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-222">String</span></span>|<span data-ttu-id="312c4-223">E-Mail-Adressen des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="312c4-223">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="312c4-224">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="312c4-224">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="312c4-225">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-225">String</span></span>|<span data-ttu-id="312c4-226">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-226">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="312c4-227">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="312c4-227">Read only.</span></span>|
|<span data-ttu-id="312c4-228">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="312c4-228">azureADDeviceId</span></span>|<span data-ttu-id="312c4-229">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-229">String</span></span>|<span data-ttu-id="312c4-230">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-230">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="312c4-231">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="312c4-231">Read only.</span></span>|
|<span data-ttu-id="312c4-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="312c4-232">deviceRegistrationState</span></span>|[<span data-ttu-id="312c4-233">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="312c4-233">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="312c4-234">Registrierungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-234">Device registration state.</span></span> <span data-ttu-id="312c4-235">Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="312c4-235">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="312c4-236">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="312c4-236">deviceCategoryDisplayName</span></span>|<span data-ttu-id="312c4-237">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-237">String</span></span>|<span data-ttu-id="312c4-238">Anzeigename der Gerätekategorie.
</span><span class="sxs-lookup"><span data-stu-id="312c4-238">Device category display name</span></span>|
|<span data-ttu-id="312c4-239">isSupervised</span><span class="sxs-lookup"><span data-stu-id="312c4-239">isSupervised</span></span>|<span data-ttu-id="312c4-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="312c4-240">Boolean</span></span>|<span data-ttu-id="312c4-241">Überwachungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="312c4-241">Device supervised status</span></span>|
|<span data-ttu-id="312c4-242">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="312c4-242">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="312c4-243">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="312c4-243">DateTimeOffset</span></span>|<span data-ttu-id="312c4-244">Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange</span><span class="sxs-lookup"><span data-stu-id="312c4-244">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="312c4-245">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="312c4-245">exchangeAccessState</span></span>|[<span data-ttu-id="312c4-246">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="312c4-246">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="312c4-247">Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="312c4-247">The Access State of the device in Exchange.</span></span> <span data-ttu-id="312c4-248">Mögliche Werte sind: `none`, `unknown`, `allowed`, `blocked` und `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="312c4-248">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="312c4-249">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="312c4-249">exchangeAccessStateReason</span></span>|[<span data-ttu-id="312c4-250">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="312c4-250">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="312c4-251">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="312c4-251">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="312c4-252">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="312c4-252">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="312c4-253">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="312c4-253">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="312c4-254">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-254">String</span></span>|<span data-ttu-id="312c4-255">URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
</span><span class="sxs-lookup"><span data-stu-id="312c4-255">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="312c4-256">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="312c4-256">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="312c4-257">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-257">String</span></span>|<span data-ttu-id="312c4-258">Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
</span><span class="sxs-lookup"><span data-stu-id="312c4-258">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="312c4-259">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="312c4-259">isEncrypted</span></span>|<span data-ttu-id="312c4-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="312c4-260">Boolean</span></span>|<span data-ttu-id="312c4-261">Verschlüsselungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="312c4-261">Device encryption status</span></span>|
|<span data-ttu-id="312c4-262">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="312c4-262">userPrincipalName</span></span>|<span data-ttu-id="312c4-263">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-263">String</span></span>|<span data-ttu-id="312c4-264">Benutzerprinzipalname für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="312c4-264">Device user principal name</span></span>|
|<span data-ttu-id="312c4-265">model</span><span class="sxs-lookup"><span data-stu-id="312c4-265">model</span></span>|<span data-ttu-id="312c4-266">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-266">String</span></span>|<span data-ttu-id="312c4-267">Modell des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="312c4-267">Model of the device</span></span>|
|<span data-ttu-id="312c4-268">manufacturer</span><span class="sxs-lookup"><span data-stu-id="312c4-268">manufacturer</span></span>|<span data-ttu-id="312c4-269">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-269">String</span></span>|<span data-ttu-id="312c4-270">Hersteller des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="312c4-270">Manufacturer of the device</span></span>|
|<span data-ttu-id="312c4-271">imei</span><span class="sxs-lookup"><span data-stu-id="312c4-271">imei</span></span>|<span data-ttu-id="312c4-272">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-272">String</span></span>|<span data-ttu-id="312c4-273">IMEI</span><span class="sxs-lookup"><span data-stu-id="312c4-273">IMEI</span></span>|
|<span data-ttu-id="312c4-274">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="312c4-274">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="312c4-275">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="312c4-275">DateTimeOffset</span></span>|<span data-ttu-id="312c4-276">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität.
</span><span class="sxs-lookup"><span data-stu-id="312c4-276">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="312c4-277">serialNumber</span><span class="sxs-lookup"><span data-stu-id="312c4-277">serialNumber</span></span>|<span data-ttu-id="312c4-278">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-278">String</span></span>|<span data-ttu-id="312c4-279">Seriennummer.
</span><span class="sxs-lookup"><span data-stu-id="312c4-279">SerialNumber</span></span>|
|<span data-ttu-id="312c4-280">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="312c4-280">phoneNumber</span></span>|<span data-ttu-id="312c4-281">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-281">String</span></span>|<span data-ttu-id="312c4-282">Telefonnummer des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="312c4-282">Phone number of the device</span></span>|
|<span data-ttu-id="312c4-283">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="312c4-283">androidSecurityPatchLevel</span></span>|<span data-ttu-id="312c4-284">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-284">String</span></span>|<span data-ttu-id="312c4-285">Android-Sicherheitspatchlevel.
</span><span class="sxs-lookup"><span data-stu-id="312c4-285">Android security patch level</span></span>|
|<span data-ttu-id="312c4-286">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="312c4-286">userDisplayName</span></span>|<span data-ttu-id="312c4-287">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-287">String</span></span>|<span data-ttu-id="312c4-288">Anzeigename des Benutzers.
</span><span class="sxs-lookup"><span data-stu-id="312c4-288">User display name</span></span>|
|<span data-ttu-id="312c4-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="312c4-289">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="312c4-290">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="312c4-290">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="312c4-291">Aktivierte Funktionen des Konfigurations-Manager-Clients.
</span><span class="sxs-lookup"><span data-stu-id="312c4-291">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="312c4-292">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="312c4-292">wiFiMacAddress</span></span>|<span data-ttu-id="312c4-293">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-293">String</span></span>|<span data-ttu-id="312c4-294">WLAN-MAC</span><span class="sxs-lookup"><span data-stu-id="312c4-294">Wi-Fi MAC</span></span>|
|<span data-ttu-id="312c4-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="312c4-295">deviceHealthAttestationState</span></span>|[<span data-ttu-id="312c4-296">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="312c4-296">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="312c4-297">Status des Integritätsnachweises für Geräte.
</span><span class="sxs-lookup"><span data-stu-id="312c4-297">The device health attestation state.</span></span>|
|<span data-ttu-id="312c4-298">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="312c4-298">subscriberCarrier</span></span>|<span data-ttu-id="312c4-299">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-299">String</span></span>|<span data-ttu-id="312c4-300">Netzbetreiber des Abonnenten.
</span><span class="sxs-lookup"><span data-stu-id="312c4-300">Subscriber Carrier</span></span>|
|<span data-ttu-id="312c4-301">meid</span><span class="sxs-lookup"><span data-stu-id="312c4-301">meid</span></span>|<span data-ttu-id="312c4-302">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-302">String</span></span>|<span data-ttu-id="312c4-303">MEID</span><span class="sxs-lookup"><span data-stu-id="312c4-303">MEID</span></span>|
|<span data-ttu-id="312c4-304">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="312c4-304">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="312c4-305">Int64</span><span class="sxs-lookup"><span data-stu-id="312c4-305">Int64</span></span>|<span data-ttu-id="312c4-306">Gesamtspeicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="312c4-306">Total Storage in Bytes</span></span>|
|<span data-ttu-id="312c4-307">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="312c4-307">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="312c4-308">Int64</span><span class="sxs-lookup"><span data-stu-id="312c4-308">Int64</span></span>|<span data-ttu-id="312c4-309">Freier Speicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="312c4-309">Free Storage in Bytes</span></span>|
|<span data-ttu-id="312c4-310">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="312c4-310">managedDeviceName</span></span>|<span data-ttu-id="312c4-311">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-311">String</span></span>|<span data-ttu-id="312c4-312">Automatisch generierter Name zur Identifizierung des Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-312">Automatically generated name to identify a device.</span></span> <span data-ttu-id="312c4-313">Kann mit einem benutzerfreundlichen Namen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="312c4-313">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="312c4-314">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="312c4-314">partnerReportedThreatState</span></span>|[<span data-ttu-id="312c4-315">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="312c4-315">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="312c4-316">Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen.</span><span class="sxs-lookup"><span data-stu-id="312c4-316">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="312c4-317">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="312c4-317">Read Only.</span></span> <span data-ttu-id="312c4-318">Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="312c4-318">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="312c4-319">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="312c4-319">usersLoggedOn</span></span>|<span data-ttu-id="312c4-320">[LoggedOnUser](../resources/intune-devices-loggedonuser.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="312c4-320">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="312c4-321">Gibt das letzte angemeldete Benutzer eines Geräts</span><span class="sxs-lookup"><span data-stu-id="312c4-321">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="312c4-322">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="312c4-322">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="312c4-323">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="312c4-323">DateTimeOffset</span></span>|<span data-ttu-id="312c4-324">Meldet den DateTime-Wert die Einstellung PreferMdmOverGroupPolicy festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="312c4-324">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="312c4-325">Wenn festgelegt ist, werden die Intune MDM Einstellungen Group Policy Settings außer Kraft setzen, wenn ein Konflikt vorliegt.</span><span class="sxs-lookup"><span data-stu-id="312c4-325">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="312c4-326">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="312c4-326">Read Only.</span></span>|
|<span data-ttu-id="312c4-327">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="312c4-327">autopilotEnrolled</span></span>|<span data-ttu-id="312c4-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="312c4-328">Boolean</span></span>|<span data-ttu-id="312c4-329">Gibt an, ob das verwaltete Geräte über den Auto-Pilot registriert ist.</span><span class="sxs-lookup"><span data-stu-id="312c4-329">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="312c4-330">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="312c4-330">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="312c4-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="312c4-331">Boolean</span></span>|<span data-ttu-id="312c4-332">Gibt an, ob das Gerät verwalteten iOS Benutzer Genehmigung Registrierung wird.</span><span class="sxs-lookup"><span data-stu-id="312c4-332">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="312c4-333">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="312c4-333">managementCertificateExpirationDate</span></span>|<span data-ttu-id="312c4-334">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="312c4-334">DateTimeOffset</span></span>|<span data-ttu-id="312c4-335">Ablaufdatum des Zertifikats Berichte Gerät management</span><span class="sxs-lookup"><span data-stu-id="312c4-335">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="312c4-336">iccid</span><span class="sxs-lookup"><span data-stu-id="312c4-336">iccid</span></span>|<span data-ttu-id="312c4-337">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-337">String</span></span>|<span data-ttu-id="312c4-338">Chip Karte Bezeichner, ist es eine SIM-Karte eindeutige ID-Nummer.</span><span class="sxs-lookup"><span data-stu-id="312c4-338">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="312c4-339">UDID</span><span class="sxs-lookup"><span data-stu-id="312c4-339">udid</span></span>|<span data-ttu-id="312c4-340">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-340">String</span></span>|<span data-ttu-id="312c4-341">Eindeutige Geräte-ID für iOS und Mac OS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="312c4-341">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="312c4-342">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="312c4-342">roleScopeTagIds</span></span>|<span data-ttu-id="312c4-343">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="312c4-343">String collection</span></span>|<span data-ttu-id="312c4-344">Liste der Bereichs-Tag-IDs für diese Instanz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="312c4-344">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="312c4-345">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="312c4-345">windowsActiveMalwareCount</span></span>|<span data-ttu-id="312c4-346">Int32</span><span class="sxs-lookup"><span data-stu-id="312c4-346">Int32</span></span>|<span data-ttu-id="312c4-347">Anzahl von aktiven Malware für dieses Windows-Gerät</span><span class="sxs-lookup"><span data-stu-id="312c4-347">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="312c4-348">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="312c4-348">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="312c4-349">Int32</span><span class="sxs-lookup"><span data-stu-id="312c4-349">Int32</span></span>|<span data-ttu-id="312c4-350">Anzahl der für gewartete Malware für dieses Windows-Gerät</span><span class="sxs-lookup"><span data-stu-id="312c4-350">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="312c4-351">notes</span><span class="sxs-lookup"><span data-stu-id="312c4-351">notes</span></span>|<span data-ttu-id="312c4-352">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="312c4-352">String</span></span>|<span data-ttu-id="312c4-353">Notes auf dem Gerät durch den IT-Administrator erstellt</span><span class="sxs-lookup"><span data-stu-id="312c4-353">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="312c4-354">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="312c4-354">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="312c4-355">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="312c4-355">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="312c4-356">Konfigurations-Manager-Client Integritätsstatus, gilt nur für Geräte verwaltet von MDM/Configuration Manager-Agent</span><span class="sxs-lookup"><span data-stu-id="312c4-356">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="312c4-357">Antwort</span><span class="sxs-lookup"><span data-stu-id="312c4-357">Response</span></span>
<span data-ttu-id="312c4-358">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDevice](../resources/intune-devices-manageddevice.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="312c4-358">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="312c4-359">Beispiel</span><span class="sxs-lookup"><span data-stu-id="312c4-359">Example</span></span>

### <a name="request"></a><span data-ttu-id="312c4-360">Anforderung</span><span class="sxs-lookup"><span data-stu-id="312c4-360">Request</span></span>
<span data-ttu-id="312c4-361">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="312c4-361">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7166

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

### <a name="response"></a><span data-ttu-id="312c4-362">Antwort</span><span class="sxs-lookup"><span data-stu-id="312c4-362">Response</span></span>
<span data-ttu-id="312c4-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="312c4-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7215

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




