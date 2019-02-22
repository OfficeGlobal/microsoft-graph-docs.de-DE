---
title: WindowsManagedDevice erstellen
description: Erstellen eines neuen windowsManagedDevice-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d2860a5e982e9079356df81b527a0cf9d02f6f7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161145"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="910cc-103">WindowsManagedDevice erstellen</span><span class="sxs-lookup"><span data-stu-id="910cc-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="910cc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="910cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="910cc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="910cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="910cc-106">Erstellen eines neuen [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="910cc-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="910cc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="910cc-107">Prerequisites</span></span>
<span data-ttu-id="910cc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="910cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="910cc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="910cc-110">Permission type</span></span>|<span data-ttu-id="910cc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="910cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="910cc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="910cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="910cc-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="910cc-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="910cc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="910cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="910cc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="910cc-115">Not supported.</span></span>|
|<span data-ttu-id="910cc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="910cc-116">Application</span></span>|<span data-ttu-id="910cc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="910cc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="910cc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="910cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="910cc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="910cc-119">Request headers</span></span>
|<span data-ttu-id="910cc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="910cc-120">Header</span></span>|<span data-ttu-id="910cc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="910cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="910cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="910cc-122">Authorization</span></span>|<span data-ttu-id="910cc-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="910cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="910cc-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="910cc-124">Accept</span></span>|<span data-ttu-id="910cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="910cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="910cc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="910cc-126">Request body</span></span>
<span data-ttu-id="910cc-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsManagedDevice-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="910cc-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="910cc-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsManagedDevice erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="910cc-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="910cc-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="910cc-129">Property</span></span>|<span data-ttu-id="910cc-130">Typ</span><span class="sxs-lookup"><span data-stu-id="910cc-130">Type</span></span>|<span data-ttu-id="910cc-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="910cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="910cc-132">id</span><span class="sxs-lookup"><span data-stu-id="910cc-132">id</span></span>|<span data-ttu-id="910cc-133">string</span><span class="sxs-lookup"><span data-stu-id="910cc-133">String</span></span>|<span data-ttu-id="910cc-134">Eindeutiger Bezeichner für das von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbte Gerät</span><span class="sxs-lookup"><span data-stu-id="910cc-134">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-135">userId</span><span class="sxs-lookup"><span data-stu-id="910cc-135">userId</span></span>|<span data-ttu-id="910cc-136">String</span><span class="sxs-lookup"><span data-stu-id="910cc-136">String</span></span>|<span data-ttu-id="910cc-137">Eindeutiger Bezeichner für den Benutzer, der mit dem von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Gerät verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="910cc-137">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="910cc-138">deviceName</span></span>|<span data-ttu-id="910cc-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-139">String</span></span>|<span data-ttu-id="910cc-140">Name des von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="910cc-140">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-141">Dem</span><span class="sxs-lookup"><span data-stu-id="910cc-141">hardwareInformation</span></span>|[<span data-ttu-id="910cc-142">Dem</span><span class="sxs-lookup"><span data-stu-id="910cc-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="910cc-143">Die hardward-Details für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="910cc-143">The hardward details for the device.</span></span>  <span data-ttu-id="910cc-144">Enthält Informationen wie Speicherplatz, Hersteller, Seriennummer usw. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-144">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="910cc-145">ownerType</span></span>|[<span data-ttu-id="910cc-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="910cc-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="910cc-147">Der Besitzer des Geräts.</span><span class="sxs-lookup"><span data-stu-id="910cc-147">Ownership of the device.</span></span> <span data-ttu-id="910cc-148">Kann "Company" oder "Personal" von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt werden.</span><span class="sxs-lookup"><span data-stu-id="910cc-148">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="910cc-149">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="910cc-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="910cc-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="910cc-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="910cc-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="910cc-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="910cc-152">Der Besitzer des Geräts.</span><span class="sxs-lookup"><span data-stu-id="910cc-152">Ownership of the device.</span></span> <span data-ttu-id="910cc-153">Kann "Company" oder "Personal" von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt werden.</span><span class="sxs-lookup"><span data-stu-id="910cc-153">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="910cc-154">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="910cc-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="910cc-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="910cc-155">deviceActionResults</span></span>|<span data-ttu-id="910cc-156">Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="910cc-157">Liste von Objekten des Typs „ComplexType deviceActionResult“.
</span><span class="sxs-lookup"><span data-stu-id="910cc-157">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="910cc-158">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-158">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-159">managementState</span><span class="sxs-lookup"><span data-stu-id="910cc-159">managementState</span></span>|[<span data-ttu-id="910cc-160">managementState</span><span class="sxs-lookup"><span data-stu-id="910cc-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="910cc-161">Verwaltungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="910cc-161">Management state of the device.</span></span> <span data-ttu-id="910cc-162">Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="910cc-162">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="910cc-163">Mögliche Werte sind: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled` und `discovered`.</span><span class="sxs-lookup"><span data-stu-id="910cc-163">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="910cc-164">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="910cc-164">enrolledDateTime</span></span>|<span data-ttu-id="910cc-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="910cc-165">DateTimeOffset</span></span>|<span data-ttu-id="910cc-166">Datum und Uhrzeit der Geräteregistrierung.
</span><span class="sxs-lookup"><span data-stu-id="910cc-166">Enrollment time of the device.</span></span> <span data-ttu-id="910cc-167">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-168">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="910cc-168">lastSyncDateTime</span></span>|<span data-ttu-id="910cc-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="910cc-169">DateTimeOffset</span></span>|<span data-ttu-id="910cc-170">Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
</span><span class="sxs-lookup"><span data-stu-id="910cc-170">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="910cc-171">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-172">chassitype</span><span class="sxs-lookup"><span data-stu-id="910cc-172">chassisType</span></span>|[<span data-ttu-id="910cc-173">chassitype</span><span class="sxs-lookup"><span data-stu-id="910cc-173">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="910cc-174">Gehäusetyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="910cc-174">Chassis type of the device.</span></span> <span data-ttu-id="910cc-175">Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="910cc-175">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="910cc-176">Mögliche Werte: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="910cc-176">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="910cc-177">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="910cc-177">operatingSystem</span></span>|<span data-ttu-id="910cc-178">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-178">String</span></span>|<span data-ttu-id="910cc-179">Betriebssystem des Geräts.</span><span class="sxs-lookup"><span data-stu-id="910cc-179">Operating system of the device.</span></span> <span data-ttu-id="910cc-180">Windows, iOS, etc. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-180">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-181">deviceType</span><span class="sxs-lookup"><span data-stu-id="910cc-181">deviceType</span></span>|[<span data-ttu-id="910cc-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="910cc-182">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="910cc-183">Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="910cc-183">Platform of the device.</span></span> <span data-ttu-id="910cc-184">Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="910cc-184">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="910cc-185">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="910cc-185">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="910cc-186">complianceState</span><span class="sxs-lookup"><span data-stu-id="910cc-186">complianceState</span></span>|[<span data-ttu-id="910cc-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="910cc-187">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="910cc-188">Konformitätsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="910cc-188">Compliance state of the device.</span></span> <span data-ttu-id="910cc-189">Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="910cc-189">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="910cc-190">Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.</span><span class="sxs-lookup"><span data-stu-id="910cc-190">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="910cc-191">jailBroken</span><span class="sxs-lookup"><span data-stu-id="910cc-191">jailBroken</span></span>|<span data-ttu-id="910cc-192">String</span><span class="sxs-lookup"><span data-stu-id="910cc-192">String</span></span>|<span data-ttu-id="910cc-193">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="910cc-193">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="910cc-194">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-195">managementAgent</span><span class="sxs-lookup"><span data-stu-id="910cc-195">managementAgent</span></span>|[<span data-ttu-id="910cc-196">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="910cc-196">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="910cc-197">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="910cc-197">Management channel of the device.</span></span> <span data-ttu-id="910cc-198">InTune, EAS usw. Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="910cc-198">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="910cc-199">Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController` und `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="910cc-199">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="910cc-200">osVersion</span><span class="sxs-lookup"><span data-stu-id="910cc-200">osVersion</span></span>|<span data-ttu-id="910cc-201">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-201">String</span></span>|<span data-ttu-id="910cc-202">Auf dem Gerät installierte Betriebssystemversion.
</span><span class="sxs-lookup"><span data-stu-id="910cc-202">Operating system version of the device.</span></span> <span data-ttu-id="910cc-203">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-203">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-204">easActivated</span><span class="sxs-lookup"><span data-stu-id="910cc-204">easActivated</span></span>|<span data-ttu-id="910cc-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="910cc-205">Boolean</span></span>|<span data-ttu-id="910cc-206">Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="910cc-206">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="910cc-207">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-207">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-208">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="910cc-208">easDeviceId</span></span>|<span data-ttu-id="910cc-209">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-209">String</span></span>|<span data-ttu-id="910cc-210">Exchange ActiveSync-ID des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="910cc-210">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="910cc-211">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-212">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="910cc-212">easActivationDateTime</span></span>|<span data-ttu-id="910cc-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="910cc-213">DateTimeOffset</span></span>|<span data-ttu-id="910cc-214">Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="910cc-214">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="910cc-215">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-216">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="910cc-216">aadRegistered</span></span>|<span data-ttu-id="910cc-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="910cc-217">Boolean</span></span>|<span data-ttu-id="910cc-218">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="910cc-218">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="910cc-219">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-219">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-220">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="910cc-220">azureADRegistered</span></span>|<span data-ttu-id="910cc-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="910cc-221">Boolean</span></span>|<span data-ttu-id="910cc-222">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="910cc-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="910cc-223">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-223">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-224">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="910cc-224">deviceEnrollmentType</span></span>|[<span data-ttu-id="910cc-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="910cc-225">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="910cc-226">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="910cc-226">Enrollment type of the device.</span></span> <span data-ttu-id="910cc-227">Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="910cc-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="910cc-228">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="910cc-228">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="910cc-229">lostModeState</span><span class="sxs-lookup"><span data-stu-id="910cc-229">lostModeState</span></span>|[<span data-ttu-id="910cc-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="910cc-230">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="910cc-231">Gibt an, ob der Modus verloren aktiviert oder deaktiviert von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt wurde.</span><span class="sxs-lookup"><span data-stu-id="910cc-231">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="910cc-232">Mögliche Werte sind: `disabled` und `enabled`.</span><span class="sxs-lookup"><span data-stu-id="910cc-232">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="910cc-233">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="910cc-233">activationLockBypassCode</span></span>|<span data-ttu-id="910cc-234">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-234">String</span></span>|<span data-ttu-id="910cc-235">Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht</span><span class="sxs-lookup"><span data-stu-id="910cc-235">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="910cc-236">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-237">emailAddress</span><span class="sxs-lookup"><span data-stu-id="910cc-237">emailAddress</span></span>|<span data-ttu-id="910cc-238">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-238">String</span></span>|<span data-ttu-id="910cc-239">E-Mail (e) für den Benutzer, der mit dem von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Gerät verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="910cc-239">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-240">Eigenschaften azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="910cc-240">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="910cc-241">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-241">String</span></span>|<span data-ttu-id="910cc-242">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="910cc-242">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="910cc-243">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="910cc-243">Read only.</span></span> <span data-ttu-id="910cc-244">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-244">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-245">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="910cc-245">azureADDeviceId</span></span>|<span data-ttu-id="910cc-246">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-246">String</span></span>|<span data-ttu-id="910cc-247">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="910cc-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="910cc-248">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="910cc-248">Read only.</span></span> <span data-ttu-id="910cc-249">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-249">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-250">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="910cc-250">deviceRegistrationState</span></span>|[<span data-ttu-id="910cc-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="910cc-251">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="910cc-252">Registrierungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="910cc-252">Device registration state.</span></span> <span data-ttu-id="910cc-253">Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="910cc-253">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="910cc-254">Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="910cc-254">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="910cc-255">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="910cc-255">deviceCategoryDisplayName</span></span>|<span data-ttu-id="910cc-256">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-256">String</span></span>|<span data-ttu-id="910cc-257">Anzeigename der Gerätekategorie, geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-257">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-258">isSupervised</span><span class="sxs-lookup"><span data-stu-id="910cc-258">isSupervised</span></span>|<span data-ttu-id="910cc-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="910cc-259">Boolean</span></span>|<span data-ttu-id="910cc-260">Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Geräte überwachter Status</span><span class="sxs-lookup"><span data-stu-id="910cc-260">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-261">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="910cc-261">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="910cc-262">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="910cc-262">DateTimeOffset</span></span>|<span data-ttu-id="910cc-263">Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange</span><span class="sxs-lookup"><span data-stu-id="910cc-263">Last time the device contacted Exchange.</span></span> <span data-ttu-id="910cc-264">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-265">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="910cc-265">exchangeAccessState</span></span>|[<span data-ttu-id="910cc-266">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="910cc-266">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="910cc-267">Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="910cc-267">The Access State of the device in Exchange.</span></span> <span data-ttu-id="910cc-268">Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="910cc-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="910cc-269">Mögliche Werte: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="910cc-269">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="910cc-270">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="910cc-270">exchangeAccessStateReason</span></span>|[<span data-ttu-id="910cc-271">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="910cc-271">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="910cc-272">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="910cc-272">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="910cc-273">Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="910cc-273">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="910cc-274">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="910cc-274">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="910cc-275">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="910cc-275">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="910cc-276">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-276">String</span></span>|<span data-ttu-id="910cc-277">URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
</span><span class="sxs-lookup"><span data-stu-id="910cc-277">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="910cc-278">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-278">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-279">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="910cc-279">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="910cc-280">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-280">String</span></span>|<span data-ttu-id="910cc-281">Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
</span><span class="sxs-lookup"><span data-stu-id="910cc-281">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="910cc-282">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-282">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-283">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="910cc-283">isEncrypted</span></span>|<span data-ttu-id="910cc-284">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="910cc-284">Boolean</span></span>|<span data-ttu-id="910cc-285">Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Geräte Verschlüsselungsstatus</span><span class="sxs-lookup"><span data-stu-id="910cc-285">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-286">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="910cc-286">userPrincipalName</span></span>|<span data-ttu-id="910cc-287">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-287">String</span></span>|<span data-ttu-id="910cc-288">Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Geräte Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="910cc-288">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-289">model</span><span class="sxs-lookup"><span data-stu-id="910cc-289">model</span></span>|<span data-ttu-id="910cc-290">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-290">String</span></span>|<span data-ttu-id="910cc-291">Modell des von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="910cc-291">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-292">manufacturer</span><span class="sxs-lookup"><span data-stu-id="910cc-292">manufacturer</span></span>|<span data-ttu-id="910cc-293">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-293">String</span></span>|<span data-ttu-id="910cc-294">Hersteller des von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="910cc-294">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-295">imei</span><span class="sxs-lookup"><span data-stu-id="910cc-295">imei</span></span>|<span data-ttu-id="910cc-296">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-296">String</span></span>|<span data-ttu-id="910cc-297">IMEI geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-297">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-298">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="910cc-298">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="910cc-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="910cc-299">DateTimeOffset</span></span>|<span data-ttu-id="910cc-300">Das Datum, an dem die Zeitdauer für die Geräte Konformität von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt wurde</span><span class="sxs-lookup"><span data-stu-id="910cc-300">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-301">serialNumber</span><span class="sxs-lookup"><span data-stu-id="910cc-301">serialNumber</span></span>|<span data-ttu-id="910cc-302">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-302">String</span></span>|<span data-ttu-id="910cc-303">Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbte Seriennummer</span><span class="sxs-lookup"><span data-stu-id="910cc-303">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-304">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="910cc-304">phoneNumber</span></span>|<span data-ttu-id="910cc-305">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-305">String</span></span>|<span data-ttu-id="910cc-306">Telefonnummer des von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts</span><span class="sxs-lookup"><span data-stu-id="910cc-306">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-307">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="910cc-307">androidSecurityPatchLevel</span></span>|<span data-ttu-id="910cc-308">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-308">String</span></span>|<span data-ttu-id="910cc-309">Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbte Sicherheitspatch-Stufe von Android</span><span class="sxs-lookup"><span data-stu-id="910cc-309">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-310">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="910cc-310">userDisplayName</span></span>|<span data-ttu-id="910cc-311">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-311">String</span></span>|<span data-ttu-id="910cc-312">Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Benutzeranzeigename</span><span class="sxs-lookup"><span data-stu-id="910cc-312">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-313">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="910cc-313">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="910cc-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="910cc-314">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="910cc-315">Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbte aktivierte-Client aktivierte Features</span><span class="sxs-lookup"><span data-stu-id="910cc-315">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-316">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="910cc-316">wiFiMacAddress</span></span>|<span data-ttu-id="910cc-317">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-317">String</span></span>|<span data-ttu-id="910cc-318">Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Wi-Fi-Mac</span><span class="sxs-lookup"><span data-stu-id="910cc-318">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-319">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="910cc-319">deviceHealthAttestationState</span></span>|[<span data-ttu-id="910cc-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="910cc-320">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="910cc-321">Status des Integritätsnachweises für Geräte.
</span><span class="sxs-lookup"><span data-stu-id="910cc-321">The device health attestation state.</span></span> <span data-ttu-id="910cc-322">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-322">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-323">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="910cc-323">subscriberCarrier</span></span>|<span data-ttu-id="910cc-324">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-324">String</span></span>|<span data-ttu-id="910cc-325">Von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbter Abonnent</span><span class="sxs-lookup"><span data-stu-id="910cc-325">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-326">meid</span><span class="sxs-lookup"><span data-stu-id="910cc-326">meid</span></span>|<span data-ttu-id="910cc-327">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-327">String</span></span>|<span data-ttu-id="910cc-328">Von [ManagedDevice](../resources/intune-devices-manageddevice.md) GEERBTe MEID</span><span class="sxs-lookup"><span data-stu-id="910cc-328">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-329">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="910cc-329">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="910cc-330">Int64</span><span class="sxs-lookup"><span data-stu-id="910cc-330">Int64</span></span>|<span data-ttu-id="910cc-331">Gesamtspeicher in Byte, geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-331">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-332">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="910cc-332">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="910cc-333">Int64</span><span class="sxs-lookup"><span data-stu-id="910cc-333">Int64</span></span>|<span data-ttu-id="910cc-334">Freier Speicher in von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten bytes</span><span class="sxs-lookup"><span data-stu-id="910cc-334">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-335">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="910cc-335">managedDeviceName</span></span>|<span data-ttu-id="910cc-336">String</span><span class="sxs-lookup"><span data-stu-id="910cc-336">String</span></span>|<span data-ttu-id="910cc-337">Automatisch generierter Name zur Identifizierung des Geräts.</span><span class="sxs-lookup"><span data-stu-id="910cc-337">Automatically generated name to identify a device.</span></span> <span data-ttu-id="910cc-338">Kann mit einem benutzerfreundlichen Namen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="910cc-338">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="910cc-339">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-340">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="910cc-340">partnerReportedThreatState</span></span>|[<span data-ttu-id="910cc-341">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="910cc-341">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="910cc-342">Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen.</span><span class="sxs-lookup"><span data-stu-id="910cc-342">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="910cc-343">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="910cc-343">Read Only.</span></span> <span data-ttu-id="910cc-344">Von [ManagedDevice](../resources/intune-devices-manageddevice.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="910cc-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="910cc-345">Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="910cc-345">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="910cc-346">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="910cc-346">usersLoggedOn</span></span>|<span data-ttu-id="910cc-347">[loggedOnUser](../resources/intune-devices-loggedonuser.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="910cc-347">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="910cc-348">Gibt die zuletzt angemeldeten Benutzer eines von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten Geräts an.</span><span class="sxs-lookup"><span data-stu-id="910cc-348">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-349">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="910cc-349">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="910cc-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="910cc-350">DateTimeOffset</span></span>|<span data-ttu-id="910cc-351">Meldet den DateTime-Wert für die Einstellung preferMdmOverGroupPolicy.</span><span class="sxs-lookup"><span data-stu-id="910cc-351">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="910cc-352">Ist diese Einstellung festgelegt, überschreiben die Intune-MDM-Einstellungen Gruppenrichtlinieneinstellungen bei einem Konflikt.</span><span class="sxs-lookup"><span data-stu-id="910cc-352">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="910cc-353">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="910cc-353">Read Only.</span></span> <span data-ttu-id="910cc-354">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-355">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="910cc-355">autopilotEnrolled</span></span>|<span data-ttu-id="910cc-356">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="910cc-356">Boolean</span></span>|<span data-ttu-id="910cc-357">Meldet, ob das verwaltete Gerät über Auto-Pilot registriert wird.</span><span class="sxs-lookup"><span data-stu-id="910cc-357">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="910cc-358">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-359">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="910cc-359">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="910cc-360">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="910cc-360">Boolean</span></span>|<span data-ttu-id="910cc-361">Meldet, ob das verwaltete iOS-Gerät Benutzer Genehmigungs Registrierung ist.</span><span class="sxs-lookup"><span data-stu-id="910cc-361">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="910cc-362">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-362">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-363">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="910cc-363">managementCertificateExpirationDate</span></span>|<span data-ttu-id="910cc-364">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="910cc-364">DateTimeOffset</span></span>|<span data-ttu-id="910cc-365">Meldet Ablaufdatum für das Geräte Verwaltungszertifikat, das von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt wurde</span><span class="sxs-lookup"><span data-stu-id="910cc-365">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-366">ICCID</span><span class="sxs-lookup"><span data-stu-id="910cc-366">iccid</span></span>|<span data-ttu-id="910cc-367">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-367">String</span></span>|<span data-ttu-id="910cc-368">Integrated Circuit Card Identifier, es ist die eindeutige Identifikationsnummer einer SIM-Karte.</span><span class="sxs-lookup"><span data-stu-id="910cc-368">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="910cc-369">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-370">UDID</span><span class="sxs-lookup"><span data-stu-id="910cc-370">udid</span></span>|<span data-ttu-id="910cc-371">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-371">String</span></span>|<span data-ttu-id="910cc-372">Eindeutige Gerätekennung für iOS-und macOS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="910cc-372">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="910cc-373">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-374">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="910cc-374">roleScopeTagIds</span></span>|<span data-ttu-id="910cc-375">String collection</span><span class="sxs-lookup"><span data-stu-id="910cc-375">String collection</span></span>|<span data-ttu-id="910cc-376">Liste der Bereichstag-IDs für diese Geräteinstanz.</span><span class="sxs-lookup"><span data-stu-id="910cc-376">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="910cc-377">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-377">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-378">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="910cc-378">windowsActiveMalwareCount</span></span>|<span data-ttu-id="910cc-379">Int32</span><span class="sxs-lookup"><span data-stu-id="910cc-379">Int32</span></span>|<span data-ttu-id="910cc-380">Anzahl der aktiven Schadsoftware für dieses Windows-Gerät, geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-380">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-381">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="910cc-381">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="910cc-382">Int32</span><span class="sxs-lookup"><span data-stu-id="910cc-382">Int32</span></span>|<span data-ttu-id="910cc-383">Anzahl der korrigierten Schadsoftware für dieses Windows-Gerät, geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="910cc-383">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-384">notes</span><span class="sxs-lookup"><span data-stu-id="910cc-384">notes</span></span>|<span data-ttu-id="910cc-385">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="910cc-385">String</span></span>|<span data-ttu-id="910cc-386">Hinweise auf dem vom IT-Administrator erstellten Gerät werden von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt.</span><span class="sxs-lookup"><span data-stu-id="910cc-386">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="910cc-387">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="910cc-387">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="910cc-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="910cc-388">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="910cc-389">Configuration Manager-Clientintegritätsstatus, nur gültig für Geräte, die von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbten MDM/ConfigMgr-Agent verwaltet werden</span><span class="sxs-lookup"><span data-stu-id="910cc-389">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="910cc-390">Antwort</span><span class="sxs-lookup"><span data-stu-id="910cc-390">Response</span></span>
<span data-ttu-id="910cc-391">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="910cc-391">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="910cc-392">Beispiel</span><span class="sxs-lookup"><span data-stu-id="910cc-392">Example</span></span>

### <a name="request"></a><span data-ttu-id="910cc-393">Anforderung</span><span class="sxs-lookup"><span data-stu-id="910cc-393">Request</span></span>
<span data-ttu-id="910cc-394">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="910cc-394">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 7231

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
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

### <a name="response"></a><span data-ttu-id="910cc-395">Antwort</span><span class="sxs-lookup"><span data-stu-id="910cc-395">Response</span></span>
<span data-ttu-id="910cc-p141">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="910cc-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7280

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "id": "97842b67-2b67-9784-672b-8497672b8497",
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




