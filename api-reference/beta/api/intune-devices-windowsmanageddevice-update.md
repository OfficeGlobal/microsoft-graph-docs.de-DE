---
title: WindowsManagedDevice aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsManagedDevice-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dc3589c49f455f287cf83d921e15973202f73e65
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424147"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="d4ffc-103">WindowsManagedDevice aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d4ffc-103">Update windowsManagedDevice</span></span>

> <span data-ttu-id="d4ffc-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d4ffc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4ffc-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4ffc-107">Aktualisieren Sie die Eigenschaften eines [WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-107">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4ffc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d4ffc-108">Prerequisites</span></span>
<span data-ttu-id="d4ffc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d4ffc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d4ffc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d4ffc-111">Permission type</span></span>|<span data-ttu-id="d4ffc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4ffc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4ffc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4ffc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d4ffc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4ffc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4ffc-116">Not supported.</span></span>|
|<span data-ttu-id="d4ffc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d4ffc-117">Application</span></span>|<span data-ttu-id="d4ffc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4ffc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4ffc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4ffc-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d4ffc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d4ffc-120">Request headers</span></span>
|<span data-ttu-id="d4ffc-121">Header</span><span class="sxs-lookup"><span data-stu-id="d4ffc-121">Header</span></span>|<span data-ttu-id="d4ffc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d4ffc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4ffc-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d4ffc-123">Authorization</span></span>|<span data-ttu-id="d4ffc-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d4ffc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4ffc-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d4ffc-125">Accept</span></span>|<span data-ttu-id="d4ffc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4ffc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4ffc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d4ffc-127">Request body</span></span>
<span data-ttu-id="d4ffc-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-128">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="d4ffc-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-129">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="d4ffc-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4ffc-130">Property</span></span>|<span data-ttu-id="d4ffc-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d4ffc-131">Type</span></span>|<span data-ttu-id="d4ffc-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4ffc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4ffc-133">id</span><span class="sxs-lookup"><span data-stu-id="d4ffc-133">id</span></span>|<span data-ttu-id="d4ffc-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-134">String</span></span>|<span data-ttu-id="d4ffc-135">Eindeutiger Bezeichner für das Gerät Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-135">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-136">userId</span><span class="sxs-lookup"><span data-stu-id="d4ffc-136">userId</span></span>|<span data-ttu-id="d4ffc-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-137">String</span></span>|<span data-ttu-id="d4ffc-138">Eindeutiger Bezeichner für den Benutzer mit dem Gerät Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-138">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="d4ffc-139">deviceName</span></span>|<span data-ttu-id="d4ffc-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-140">String</span></span>|<span data-ttu-id="d4ffc-141">Name des Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-141">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="d4ffc-142">hardwareInformation</span></span>|[<span data-ttu-id="d4ffc-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="d4ffc-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="d4ffc-144">Die Hardward Details für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-144">The hardward details for the device.</span></span>  <span data-ttu-id="d4ffc-145">Enthält Informationen, wie Speicherplatz, Hersteller, Seriennummer. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-145">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-146">Besitzertyp</span><span class="sxs-lookup"><span data-stu-id="d4ffc-146">ownerType</span></span>|[<span data-ttu-id="d4ffc-147">Besitzertyp</span><span class="sxs-lookup"><span data-stu-id="d4ffc-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="d4ffc-148">Besitz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-148">Ownership of the device.</span></span> <span data-ttu-id="d4ffc-149">"Unternehmen" oder "personal" Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md)möglich.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-149">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d4ffc-150">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="d4ffc-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d4ffc-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="d4ffc-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="d4ffc-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="d4ffc-153">Besitz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-153">Ownership of the device.</span></span> <span data-ttu-id="d4ffc-154">"Unternehmen" oder "personal" Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md)möglich.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-154">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d4ffc-155">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="d4ffc-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="d4ffc-156">deviceActionResults</span></span>|<span data-ttu-id="d4ffc-157">Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="d4ffc-158">Liste von Objekten des Typs „ComplexType deviceActionResult“.
</span><span class="sxs-lookup"><span data-stu-id="d4ffc-158">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="d4ffc-159">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-159">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-160">managementState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-160">managementState</span></span>|[<span data-ttu-id="d4ffc-161">managementState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-161">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="d4ffc-162">Verwaltungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-162">Management state of the device.</span></span> <span data-ttu-id="d4ffc-163">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d4ffc-163">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d4ffc-164">Mögliche Werte sind: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled` und `discovered`.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-164">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="d4ffc-165">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="d4ffc-165">enrolledDateTime</span></span>|<span data-ttu-id="d4ffc-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4ffc-166">DateTimeOffset</span></span>|<span data-ttu-id="d4ffc-167">Datum und Uhrzeit der Geräteregistrierung.
</span><span class="sxs-lookup"><span data-stu-id="d4ffc-167">Enrollment time of the device.</span></span> <span data-ttu-id="d4ffc-168">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-168">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-169">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d4ffc-169">lastSyncDateTime</span></span>|<span data-ttu-id="d4ffc-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4ffc-170">DateTimeOffset</span></span>|<span data-ttu-id="d4ffc-171">Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
</span><span class="sxs-lookup"><span data-stu-id="d4ffc-171">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="d4ffc-172">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="d4ffc-173">chassisType</span></span>|[<span data-ttu-id="d4ffc-174">chassisType</span><span class="sxs-lookup"><span data-stu-id="d4ffc-174">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="d4ffc-175">Chassistyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-175">Chassis type of the device.</span></span> <span data-ttu-id="d4ffc-176">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d4ffc-176">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d4ffc-177">Mögliche Werte: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-177">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="d4ffc-178">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="d4ffc-178">operatingSystem</span></span>|<span data-ttu-id="d4ffc-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-179">String</span></span>|<span data-ttu-id="d4ffc-180">Betriebssystem des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-180">Operating system of the device.</span></span> <span data-ttu-id="d4ffc-181">Windows iOS usw.. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-181">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="d4ffc-182">deviceType</span></span>|[<span data-ttu-id="d4ffc-183">deviceType</span><span class="sxs-lookup"><span data-stu-id="d4ffc-183">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="d4ffc-184">Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-184">Platform of the device.</span></span> <span data-ttu-id="d4ffc-185">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d4ffc-185">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d4ffc-186">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-186">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="d4ffc-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-187">complianceState</span></span>|[<span data-ttu-id="d4ffc-188">complianceState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-188">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="d4ffc-189">Konformitätsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-189">Compliance state of the device.</span></span> <span data-ttu-id="d4ffc-190">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d4ffc-190">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d4ffc-191">Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-191">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="d4ffc-192">jailBroken</span><span class="sxs-lookup"><span data-stu-id="d4ffc-192">jailBroken</span></span>|<span data-ttu-id="d4ffc-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-193">String</span></span>|<span data-ttu-id="d4ffc-194">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-194">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="d4ffc-195">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-195">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-196">managementAgent</span><span class="sxs-lookup"><span data-stu-id="d4ffc-196">managementAgent</span></span>|[<span data-ttu-id="d4ffc-197">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="d4ffc-197">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="d4ffc-198">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-198">Management channel of the device.</span></span> <span data-ttu-id="d4ffc-199">Intune, EAS usw. Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d4ffc-199">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d4ffc-200">Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController` und `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-200">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="d4ffc-201">osVersion</span><span class="sxs-lookup"><span data-stu-id="d4ffc-201">osVersion</span></span>|<span data-ttu-id="d4ffc-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-202">String</span></span>|<span data-ttu-id="d4ffc-203">Auf dem Gerät installierte Betriebssystemversion.
</span><span class="sxs-lookup"><span data-stu-id="d4ffc-203">Operating system version of the device.</span></span> <span data-ttu-id="d4ffc-204">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-205">easActivated</span><span class="sxs-lookup"><span data-stu-id="d4ffc-205">easActivated</span></span>|<span data-ttu-id="d4ffc-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4ffc-206">Boolean</span></span>|<span data-ttu-id="d4ffc-207">Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-207">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="d4ffc-208">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-208">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-209">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="d4ffc-209">easDeviceId</span></span>|<span data-ttu-id="d4ffc-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-210">String</span></span>|<span data-ttu-id="d4ffc-211">Exchange ActiveSync-ID des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="d4ffc-211">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="d4ffc-212">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-212">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-213">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="d4ffc-213">easActivationDateTime</span></span>|<span data-ttu-id="d4ffc-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4ffc-214">DateTimeOffset</span></span>|<span data-ttu-id="d4ffc-215">Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="d4ffc-215">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="d4ffc-216">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-217">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="d4ffc-217">aadRegistered</span></span>|<span data-ttu-id="d4ffc-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4ffc-218">Boolean</span></span>|<span data-ttu-id="d4ffc-219">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-219">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="d4ffc-220">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-220">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-221">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="d4ffc-221">azureADRegistered</span></span>|<span data-ttu-id="d4ffc-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4ffc-222">Boolean</span></span>|<span data-ttu-id="d4ffc-223">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-223">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="d4ffc-224">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-224">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d4ffc-225">deviceEnrollmentType</span></span>|[<span data-ttu-id="d4ffc-226">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d4ffc-226">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="d4ffc-227">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-227">Enrollment type of the device.</span></span> <span data-ttu-id="d4ffc-228">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d4ffc-228">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d4ffc-229">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-229">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="d4ffc-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-230">lostModeState</span></span>|[<span data-ttu-id="d4ffc-231">lostModeState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-231">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="d4ffc-232">Gibt an, ob verloren Modus aktiviert ist oder Inherited aus [ManagedDevice deaktiviert](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d4ffc-232">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d4ffc-233">Mögliche Werte sind: `disabled` und `enabled`.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-233">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="d4ffc-234">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="d4ffc-234">activationLockBypassCode</span></span>|<span data-ttu-id="d4ffc-235">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-235">String</span></span>|<span data-ttu-id="d4ffc-236">Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht</span><span class="sxs-lookup"><span data-stu-id="d4ffc-236">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="d4ffc-237">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-238">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d4ffc-238">emailAddress</span></span>|<span data-ttu-id="d4ffc-239">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-239">String</span></span>|<span data-ttu-id="d4ffc-240">Email(s) für den Benutzer mit dem Gerät Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-240">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-241">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="d4ffc-241">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="d4ffc-242">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-242">String</span></span>|<span data-ttu-id="d4ffc-243">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-243">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="d4ffc-244">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-244">Read only.</span></span> <span data-ttu-id="d4ffc-245">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-245">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-246">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="d4ffc-246">azureADDeviceId</span></span>|<span data-ttu-id="d4ffc-247">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-247">String</span></span>|<span data-ttu-id="d4ffc-248">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="d4ffc-249">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-249">Read only.</span></span> <span data-ttu-id="d4ffc-250">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-250">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-251">deviceRegistrationState</span></span>|[<span data-ttu-id="d4ffc-252">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-252">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="d4ffc-253">Registrierungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-253">Device registration state.</span></span> <span data-ttu-id="d4ffc-254">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d4ffc-254">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d4ffc-255">Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-255">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="d4ffc-256">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="d4ffc-256">deviceCategoryDisplayName</span></span>|<span data-ttu-id="d4ffc-257">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-257">String</span></span>|<span data-ttu-id="d4ffc-258">Gerät Kategorie Anzeigenamen Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-258">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-259">isSupervised</span><span class="sxs-lookup"><span data-stu-id="d4ffc-259">isSupervised</span></span>|<span data-ttu-id="d4ffc-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4ffc-260">Boolean</span></span>|<span data-ttu-id="d4ffc-261">Überwacht Gerätestatus Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-261">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-262">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d4ffc-262">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="d4ffc-263">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4ffc-263">DateTimeOffset</span></span>|<span data-ttu-id="d4ffc-264">Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange</span><span class="sxs-lookup"><span data-stu-id="d4ffc-264">Last time the device contacted Exchange.</span></span> <span data-ttu-id="d4ffc-265">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-265">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-266">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-266">exchangeAccessState</span></span>|[<span data-ttu-id="d4ffc-267">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-267">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="d4ffc-268">Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-268">The Access State of the device in Exchange.</span></span> <span data-ttu-id="d4ffc-269">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d4ffc-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d4ffc-270">Mögliche Werte sind: `none`, `unknown`, `allowed`, `blocked` und `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-270">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="d4ffc-271">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d4ffc-271">exchangeAccessStateReason</span></span>|[<span data-ttu-id="d4ffc-272">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d4ffc-272">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="d4ffc-273">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-273">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="d4ffc-274">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d4ffc-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d4ffc-275">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-275">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="d4ffc-276">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="d4ffc-276">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="d4ffc-277">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-277">String</span></span>|<span data-ttu-id="d4ffc-278">URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
</span><span class="sxs-lookup"><span data-stu-id="d4ffc-278">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="d4ffc-279">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-279">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-280">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="d4ffc-280">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="d4ffc-281">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-281">String</span></span>|<span data-ttu-id="d4ffc-282">Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
</span><span class="sxs-lookup"><span data-stu-id="d4ffc-282">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="d4ffc-283">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-283">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-284">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="d4ffc-284">isEncrypted</span></span>|<span data-ttu-id="d4ffc-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4ffc-285">Boolean</span></span>|<span data-ttu-id="d4ffc-286">Verschlüsselung Gerätestatus Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-286">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-287">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d4ffc-287">userPrincipalName</span></span>|<span data-ttu-id="d4ffc-288">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-288">String</span></span>|<span data-ttu-id="d4ffc-289">Gerät Benutzerprinzipalnamen Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-289">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-290">model</span><span class="sxs-lookup"><span data-stu-id="d4ffc-290">model</span></span>|<span data-ttu-id="d4ffc-291">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-291">String</span></span>|<span data-ttu-id="d4ffc-292">Modell des Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-292">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-293">manufacturer</span><span class="sxs-lookup"><span data-stu-id="d4ffc-293">manufacturer</span></span>|<span data-ttu-id="d4ffc-294">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-294">String</span></span>|<span data-ttu-id="d4ffc-295">Hersteller des Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-295">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-296">imei</span><span class="sxs-lookup"><span data-stu-id="d4ffc-296">imei</span></span>|<span data-ttu-id="d4ffc-297">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-297">String</span></span>|<span data-ttu-id="d4ffc-298">IMEI von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="d4ffc-298">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-299">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d4ffc-299">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d4ffc-300">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4ffc-300">DateTimeOffset</span></span>|<span data-ttu-id="d4ffc-301">Die DateTime beim Gerät Compliance Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md) Aktivierungszeitraums</span><span class="sxs-lookup"><span data-stu-id="d4ffc-301">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-302">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d4ffc-302">serialNumber</span></span>|<span data-ttu-id="d4ffc-303">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-303">String</span></span>|<span data-ttu-id="d4ffc-304">SerialNumber von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="d4ffc-304">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-305">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="d4ffc-305">phoneNumber</span></span>|<span data-ttu-id="d4ffc-306">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-306">String</span></span>|<span data-ttu-id="d4ffc-307">Rufnummer des Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-307">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-308">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="d4ffc-308">androidSecurityPatchLevel</span></span>|<span data-ttu-id="d4ffc-309">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-309">String</span></span>|<span data-ttu-id="d4ffc-310">Android Patch Sicherheitsstufe Inherited von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-310">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-311">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d4ffc-311">userDisplayName</span></span>|<span data-ttu-id="d4ffc-312">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-312">String</span></span>|<span data-ttu-id="d4ffc-313">Anzeigename des Benutzers Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-313">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d4ffc-314">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="d4ffc-315">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="d4ffc-315">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="d4ffc-316">ConfigrMgr-Client aktiviert Inherited-Funktionen, [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-316">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-317">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="d4ffc-317">wiFiMacAddress</span></span>|<span data-ttu-id="d4ffc-318">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-318">String</span></span>|<span data-ttu-id="d4ffc-319">Wi-Fi MAC von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-319">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-320">deviceHealthAttestationState</span></span>|[<span data-ttu-id="d4ffc-321">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-321">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="d4ffc-322">Status des Integritätsnachweises für Geräte.
</span><span class="sxs-lookup"><span data-stu-id="d4ffc-322">The device health attestation state.</span></span> <span data-ttu-id="d4ffc-323">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-324">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="d4ffc-324">subscriberCarrier</span></span>|<span data-ttu-id="d4ffc-325">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-325">String</span></span>|<span data-ttu-id="d4ffc-326">Abonnenten des Netzbetreibers von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-326">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-327">meid</span><span class="sxs-lookup"><span data-stu-id="d4ffc-327">meid</span></span>|<span data-ttu-id="d4ffc-328">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-328">String</span></span>|<span data-ttu-id="d4ffc-329">MEID von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="d4ffc-329">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-330">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d4ffc-330">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="d4ffc-331">Int64</span><span class="sxs-lookup"><span data-stu-id="d4ffc-331">Int64</span></span>|<span data-ttu-id="d4ffc-332">Gesamtspeicher in Bytes von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="d4ffc-332">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-333">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="d4ffc-333">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="d4ffc-334">Int64</span><span class="sxs-lookup"><span data-stu-id="d4ffc-334">Int64</span></span>|<span data-ttu-id="d4ffc-335">Freien Speicher in Bytes von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="d4ffc-335">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-336">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="d4ffc-336">managedDeviceName</span></span>|<span data-ttu-id="d4ffc-337">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-337">String</span></span>|<span data-ttu-id="d4ffc-338">Automatisch generierter Name zur Identifizierung des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-338">Automatically generated name to identify a device.</span></span> <span data-ttu-id="d4ffc-339">Kann mit einem benutzerfreundlichen Namen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-339">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="d4ffc-340">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-340">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-341">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-341">partnerReportedThreatState</span></span>|[<span data-ttu-id="d4ffc-342">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-342">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="d4ffc-343">Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-343">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="d4ffc-344">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-344">Read Only.</span></span> <span data-ttu-id="d4ffc-345">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="d4ffc-345">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="d4ffc-346">Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-346">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="d4ffc-347">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="d4ffc-347">usersLoggedOn</span></span>|<span data-ttu-id="d4ffc-348">[LoggedOnUser](../resources/intune-devices-loggedonuser.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d4ffc-348">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="d4ffc-349">Gibt das letzte angemeldete Benutzer eines Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-349">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-350">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4ffc-350">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="d4ffc-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4ffc-351">DateTimeOffset</span></span>|<span data-ttu-id="d4ffc-352">Meldet den DateTime-Wert die Einstellung PreferMdmOverGroupPolicy festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-352">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="d4ffc-353">Wenn festgelegt ist, werden die Intune MDM Einstellungen Group Policy Settings außer Kraft setzen, wenn ein Konflikt vorliegt.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-353">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="d4ffc-354">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-354">Read Only.</span></span> <span data-ttu-id="d4ffc-355">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-355">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-356">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="d4ffc-356">autopilotEnrolled</span></span>|<span data-ttu-id="d4ffc-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4ffc-357">Boolean</span></span>|<span data-ttu-id="d4ffc-358">Gibt an, ob das verwaltete Geräte über den Auto-Pilot registriert ist.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-358">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="d4ffc-359">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-360">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="d4ffc-360">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="d4ffc-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4ffc-361">Boolean</span></span>|<span data-ttu-id="d4ffc-362">Gibt an, ob das Gerät verwalteten iOS Benutzer Genehmigung Registrierung wird.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-362">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="d4ffc-363">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-364">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="d4ffc-364">managementCertificateExpirationDate</span></span>|<span data-ttu-id="d4ffc-365">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4ffc-365">DateTimeOffset</span></span>|<span data-ttu-id="d4ffc-366">Gerät Management Ablaufdatum des Zertifikats Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md) -Berichte</span><span class="sxs-lookup"><span data-stu-id="d4ffc-366">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-367">iccid</span><span class="sxs-lookup"><span data-stu-id="d4ffc-367">iccid</span></span>|<span data-ttu-id="d4ffc-368">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-368">String</span></span>|<span data-ttu-id="d4ffc-369">Chip Karte Bezeichner, ist es eine SIM-Karte eindeutige ID-Nummer.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-369">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="d4ffc-370">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-370">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-371">UDID</span><span class="sxs-lookup"><span data-stu-id="d4ffc-371">udid</span></span>|<span data-ttu-id="d4ffc-372">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-372">String</span></span>|<span data-ttu-id="d4ffc-373">Eindeutige Geräte-ID für iOS und Mac OS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-373">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="d4ffc-374">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-375">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d4ffc-375">roleScopeTagIds</span></span>|<span data-ttu-id="d4ffc-376">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="d4ffc-376">String collection</span></span>|<span data-ttu-id="d4ffc-377">Liste der Bereichs-Tag-IDs für diese Instanz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-377">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="d4ffc-378">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-379">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="d4ffc-379">windowsActiveMalwareCount</span></span>|<span data-ttu-id="d4ffc-380">Int32</span><span class="sxs-lookup"><span data-stu-id="d4ffc-380">Int32</span></span>|<span data-ttu-id="d4ffc-381">Anzahl von aktiven Malware für dieses Windows-Gerät Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d4ffc-381">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-382">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="d4ffc-382">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="d4ffc-383">Int32</span><span class="sxs-lookup"><span data-stu-id="d4ffc-383">Int32</span></span>|<span data-ttu-id="d4ffc-384">Anzahl der für das Windows-Gerät Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md) für gewartete Schadsoftware</span><span class="sxs-lookup"><span data-stu-id="d4ffc-384">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-385">notes</span><span class="sxs-lookup"><span data-stu-id="d4ffc-385">notes</span></span>|<span data-ttu-id="d4ffc-386">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4ffc-386">String</span></span>|<span data-ttu-id="d4ffc-387">Notes auf dem Gerät von IT Admin geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md) erstellt</span><span class="sxs-lookup"><span data-stu-id="d4ffc-387">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="d4ffc-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-388">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="d4ffc-389">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d4ffc-389">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="d4ffc-390">Konfigurations-Manager-Client Integritätsstatus, gilt nur für Geräte, die von MDM/Configuration Manager-Agent geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md) verwaltet</span><span class="sxs-lookup"><span data-stu-id="d4ffc-390">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d4ffc-391">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4ffc-391">Response</span></span>
<span data-ttu-id="d4ffc-392">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-392">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4ffc-393">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d4ffc-393">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4ffc-394">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4ffc-394">Request</span></span>
<span data-ttu-id="d4ffc-395">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-395">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7173

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

### <a name="response"></a><span data-ttu-id="d4ffc-396">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4ffc-396">Response</span></span>
<span data-ttu-id="d4ffc-p142">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4ffc-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7222

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




