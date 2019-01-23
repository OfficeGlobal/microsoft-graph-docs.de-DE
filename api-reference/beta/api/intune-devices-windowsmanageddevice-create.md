---
title: Erstellen von windowsManagedDevice
description: Erstellen eines neuen WindowsManagedDevice-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a9d68fdd768f4084609b12d65b189b6b2961dfe2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398674"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="9844e-103">Erstellen von windowsManagedDevice</span><span class="sxs-lookup"><span data-stu-id="9844e-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="9844e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9844e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9844e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9844e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9844e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9844e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9844e-107">Erstellen eines neuen [WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9844e-107">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9844e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9844e-108">Prerequisites</span></span>
<span data-ttu-id="9844e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9844e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9844e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9844e-111">Permission type</span></span>|<span data-ttu-id="9844e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9844e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9844e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9844e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9844e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9844e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9844e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9844e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9844e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9844e-116">Not supported.</span></span>|
|<span data-ttu-id="9844e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9844e-117">Application</span></span>|<span data-ttu-id="9844e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9844e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9844e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9844e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="9844e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9844e-120">Request headers</span></span>
|<span data-ttu-id="9844e-121">Header</span><span class="sxs-lookup"><span data-stu-id="9844e-121">Header</span></span>|<span data-ttu-id="9844e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9844e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9844e-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9844e-123">Authorization</span></span>|<span data-ttu-id="9844e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9844e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9844e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9844e-125">Accept</span></span>|<span data-ttu-id="9844e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9844e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9844e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9844e-127">Request body</span></span>
<span data-ttu-id="9844e-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsManagedDevice eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="9844e-128">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="9844e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsManagedDevice erstellen.</span><span class="sxs-lookup"><span data-stu-id="9844e-129">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="9844e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9844e-130">Property</span></span>|<span data-ttu-id="9844e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9844e-131">Type</span></span>|<span data-ttu-id="9844e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9844e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9844e-133">id</span><span class="sxs-lookup"><span data-stu-id="9844e-133">id</span></span>|<span data-ttu-id="9844e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-134">String</span></span>|<span data-ttu-id="9844e-135">Eindeutiger Bezeichner für das Gerät Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-135">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-136">userId</span><span class="sxs-lookup"><span data-stu-id="9844e-136">userId</span></span>|<span data-ttu-id="9844e-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-137">String</span></span>|<span data-ttu-id="9844e-138">Eindeutiger Bezeichner für den Benutzer mit dem Gerät Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-138">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="9844e-139">deviceName</span></span>|<span data-ttu-id="9844e-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-140">String</span></span>|<span data-ttu-id="9844e-141">Name des Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-141">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="9844e-142">hardwareInformation</span></span>|[<span data-ttu-id="9844e-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="9844e-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="9844e-144">Die Hardward Details für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="9844e-144">The hardward details for the device.</span></span>  <span data-ttu-id="9844e-145">Enthält Informationen, wie Speicherplatz, Hersteller, Seriennummer. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-145">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-146">Besitzertyp</span><span class="sxs-lookup"><span data-stu-id="9844e-146">ownerType</span></span>|[<span data-ttu-id="9844e-147">Besitzertyp</span><span class="sxs-lookup"><span data-stu-id="9844e-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="9844e-148">Besitz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-148">Ownership of the device.</span></span> <span data-ttu-id="9844e-149">"Unternehmen" oder "personal" Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md)möglich.</span><span class="sxs-lookup"><span data-stu-id="9844e-149">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9844e-150">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="9844e-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="9844e-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="9844e-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="9844e-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="9844e-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="9844e-153">Besitz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-153">Ownership of the device.</span></span> <span data-ttu-id="9844e-154">"Unternehmen" oder "personal" Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md)möglich.</span><span class="sxs-lookup"><span data-stu-id="9844e-154">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9844e-155">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="9844e-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="9844e-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="9844e-156">deviceActionResults</span></span>|<span data-ttu-id="9844e-157">Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="9844e-158">Liste von Objekten des Typs „ComplexType deviceActionResult“.
</span><span class="sxs-lookup"><span data-stu-id="9844e-158">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="9844e-159">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-159">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-160">managementState</span><span class="sxs-lookup"><span data-stu-id="9844e-160">managementState</span></span>|[<span data-ttu-id="9844e-161">managementState</span><span class="sxs-lookup"><span data-stu-id="9844e-161">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="9844e-162">Verwaltungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-162">Management state of the device.</span></span> <span data-ttu-id="9844e-163">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="9844e-163">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9844e-164">Mögliche Werte sind: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled` und `discovered`.</span><span class="sxs-lookup"><span data-stu-id="9844e-164">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="9844e-165">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="9844e-165">enrolledDateTime</span></span>|<span data-ttu-id="9844e-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9844e-166">DateTimeOffset</span></span>|<span data-ttu-id="9844e-167">Datum und Uhrzeit der Geräteregistrierung.
</span><span class="sxs-lookup"><span data-stu-id="9844e-167">Enrollment time of the device.</span></span> <span data-ttu-id="9844e-168">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-168">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-169">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9844e-169">lastSyncDateTime</span></span>|<span data-ttu-id="9844e-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9844e-170">DateTimeOffset</span></span>|<span data-ttu-id="9844e-171">Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
</span><span class="sxs-lookup"><span data-stu-id="9844e-171">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="9844e-172">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="9844e-173">chassisType</span></span>|[<span data-ttu-id="9844e-174">chassisType</span><span class="sxs-lookup"><span data-stu-id="9844e-174">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="9844e-175">Chassistyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-175">Chassis type of the device.</span></span> <span data-ttu-id="9844e-176">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="9844e-176">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9844e-177">Mögliche Werte: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="9844e-177">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="9844e-178">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="9844e-178">operatingSystem</span></span>|<span data-ttu-id="9844e-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-179">String</span></span>|<span data-ttu-id="9844e-180">Betriebssystem des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-180">Operating system of the device.</span></span> <span data-ttu-id="9844e-181">Windows iOS usw.. Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-181">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="9844e-182">deviceType</span></span>|[<span data-ttu-id="9844e-183">deviceType</span><span class="sxs-lookup"><span data-stu-id="9844e-183">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="9844e-184">Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-184">Platform of the device.</span></span> <span data-ttu-id="9844e-185">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="9844e-185">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9844e-186">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="9844e-186">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="9844e-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="9844e-187">complianceState</span></span>|[<span data-ttu-id="9844e-188">complianceState</span><span class="sxs-lookup"><span data-stu-id="9844e-188">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="9844e-189">Konformitätsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-189">Compliance state of the device.</span></span> <span data-ttu-id="9844e-190">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="9844e-190">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9844e-191">Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.</span><span class="sxs-lookup"><span data-stu-id="9844e-191">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="9844e-192">jailBroken</span><span class="sxs-lookup"><span data-stu-id="9844e-192">jailBroken</span></span>|<span data-ttu-id="9844e-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-193">String</span></span>|<span data-ttu-id="9844e-194">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="9844e-194">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="9844e-195">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-195">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-196">managementAgent</span><span class="sxs-lookup"><span data-stu-id="9844e-196">managementAgent</span></span>|[<span data-ttu-id="9844e-197">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="9844e-197">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="9844e-198">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-198">Management channel of the device.</span></span> <span data-ttu-id="9844e-199">Intune, EAS usw. Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="9844e-199">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9844e-200">Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController` und `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="9844e-200">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="9844e-201">osVersion</span><span class="sxs-lookup"><span data-stu-id="9844e-201">osVersion</span></span>|<span data-ttu-id="9844e-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-202">String</span></span>|<span data-ttu-id="9844e-203">Auf dem Gerät installierte Betriebssystemversion.
</span><span class="sxs-lookup"><span data-stu-id="9844e-203">Operating system version of the device.</span></span> <span data-ttu-id="9844e-204">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-205">easActivated</span><span class="sxs-lookup"><span data-stu-id="9844e-205">easActivated</span></span>|<span data-ttu-id="9844e-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="9844e-206">Boolean</span></span>|<span data-ttu-id="9844e-207">Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="9844e-207">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="9844e-208">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-208">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-209">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="9844e-209">easDeviceId</span></span>|<span data-ttu-id="9844e-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-210">String</span></span>|<span data-ttu-id="9844e-211">Exchange ActiveSync-ID des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="9844e-211">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="9844e-212">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-212">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-213">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="9844e-213">easActivationDateTime</span></span>|<span data-ttu-id="9844e-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9844e-214">DateTimeOffset</span></span>|<span data-ttu-id="9844e-215">Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="9844e-215">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="9844e-216">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-217">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="9844e-217">aadRegistered</span></span>|<span data-ttu-id="9844e-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="9844e-218">Boolean</span></span>|<span data-ttu-id="9844e-219">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="9844e-219">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="9844e-220">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-220">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-221">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="9844e-221">azureADRegistered</span></span>|<span data-ttu-id="9844e-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9844e-222">Boolean</span></span>|<span data-ttu-id="9844e-223">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="9844e-223">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="9844e-224">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-224">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="9844e-225">deviceEnrollmentType</span></span>|[<span data-ttu-id="9844e-226">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="9844e-226">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="9844e-227">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-227">Enrollment type of the device.</span></span> <span data-ttu-id="9844e-228">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="9844e-228">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9844e-229">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="9844e-229">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="9844e-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="9844e-230">lostModeState</span></span>|[<span data-ttu-id="9844e-231">lostModeState</span><span class="sxs-lookup"><span data-stu-id="9844e-231">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="9844e-232">Gibt an, ob verloren Modus aktiviert ist oder Inherited aus [ManagedDevice deaktiviert](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="9844e-232">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9844e-233">Mögliche Werte sind: `disabled` und `enabled`.</span><span class="sxs-lookup"><span data-stu-id="9844e-233">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="9844e-234">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="9844e-234">activationLockBypassCode</span></span>|<span data-ttu-id="9844e-235">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-235">String</span></span>|<span data-ttu-id="9844e-236">Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht</span><span class="sxs-lookup"><span data-stu-id="9844e-236">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="9844e-237">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-238">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9844e-238">emailAddress</span></span>|<span data-ttu-id="9844e-239">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-239">String</span></span>|<span data-ttu-id="9844e-240">Email(s) für den Benutzer mit dem Gerät Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-240">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-241">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="9844e-241">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="9844e-242">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-242">String</span></span>|<span data-ttu-id="9844e-243">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-243">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="9844e-244">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9844e-244">Read only.</span></span> <span data-ttu-id="9844e-245">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-245">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-246">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="9844e-246">azureADDeviceId</span></span>|<span data-ttu-id="9844e-247">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-247">String</span></span>|<span data-ttu-id="9844e-248">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="9844e-249">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9844e-249">Read only.</span></span> <span data-ttu-id="9844e-250">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-250">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="9844e-251">deviceRegistrationState</span></span>|[<span data-ttu-id="9844e-252">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="9844e-252">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="9844e-253">Registrierungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-253">Device registration state.</span></span> <span data-ttu-id="9844e-254">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="9844e-254">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9844e-255">Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="9844e-255">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="9844e-256">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="9844e-256">deviceCategoryDisplayName</span></span>|<span data-ttu-id="9844e-257">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-257">String</span></span>|<span data-ttu-id="9844e-258">Gerät Kategorie Anzeigenamen Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-258">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-259">isSupervised</span><span class="sxs-lookup"><span data-stu-id="9844e-259">isSupervised</span></span>|<span data-ttu-id="9844e-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="9844e-260">Boolean</span></span>|<span data-ttu-id="9844e-261">Überwacht Gerätestatus Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-261">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-262">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9844e-262">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="9844e-263">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9844e-263">DateTimeOffset</span></span>|<span data-ttu-id="9844e-264">Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange</span><span class="sxs-lookup"><span data-stu-id="9844e-264">Last time the device contacted Exchange.</span></span> <span data-ttu-id="9844e-265">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-265">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-266">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="9844e-266">exchangeAccessState</span></span>|[<span data-ttu-id="9844e-267">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="9844e-267">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="9844e-268">Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="9844e-268">The Access State of the device in Exchange.</span></span> <span data-ttu-id="9844e-269">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="9844e-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9844e-270">Mögliche Werte sind: `none`, `unknown`, `allowed`, `blocked` und `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="9844e-270">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="9844e-271">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="9844e-271">exchangeAccessStateReason</span></span>|[<span data-ttu-id="9844e-272">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="9844e-272">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="9844e-273">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="9844e-273">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="9844e-274">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="9844e-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9844e-275">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="9844e-275">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="9844e-276">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="9844e-276">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="9844e-277">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-277">String</span></span>|<span data-ttu-id="9844e-278">URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
</span><span class="sxs-lookup"><span data-stu-id="9844e-278">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="9844e-279">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-279">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-280">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="9844e-280">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="9844e-281">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-281">String</span></span>|<span data-ttu-id="9844e-282">Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
</span><span class="sxs-lookup"><span data-stu-id="9844e-282">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="9844e-283">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-283">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-284">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="9844e-284">isEncrypted</span></span>|<span data-ttu-id="9844e-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="9844e-285">Boolean</span></span>|<span data-ttu-id="9844e-286">Verschlüsselung Gerätestatus Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-286">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-287">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9844e-287">userPrincipalName</span></span>|<span data-ttu-id="9844e-288">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-288">String</span></span>|<span data-ttu-id="9844e-289">Gerät Benutzerprinzipalnamen Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-289">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-290">model</span><span class="sxs-lookup"><span data-stu-id="9844e-290">model</span></span>|<span data-ttu-id="9844e-291">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-291">String</span></span>|<span data-ttu-id="9844e-292">Modell des Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-292">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-293">manufacturer</span><span class="sxs-lookup"><span data-stu-id="9844e-293">manufacturer</span></span>|<span data-ttu-id="9844e-294">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-294">String</span></span>|<span data-ttu-id="9844e-295">Hersteller des Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-295">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-296">imei</span><span class="sxs-lookup"><span data-stu-id="9844e-296">imei</span></span>|<span data-ttu-id="9844e-297">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-297">String</span></span>|<span data-ttu-id="9844e-298">IMEI von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="9844e-298">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-299">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9844e-299">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9844e-300">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9844e-300">DateTimeOffset</span></span>|<span data-ttu-id="9844e-301">Die DateTime beim Gerät Compliance Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md) Aktivierungszeitraums</span><span class="sxs-lookup"><span data-stu-id="9844e-301">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-302">serialNumber</span><span class="sxs-lookup"><span data-stu-id="9844e-302">serialNumber</span></span>|<span data-ttu-id="9844e-303">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-303">String</span></span>|<span data-ttu-id="9844e-304">SerialNumber von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="9844e-304">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-305">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="9844e-305">phoneNumber</span></span>|<span data-ttu-id="9844e-306">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-306">String</span></span>|<span data-ttu-id="9844e-307">Rufnummer des Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-307">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-308">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="9844e-308">androidSecurityPatchLevel</span></span>|<span data-ttu-id="9844e-309">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-309">String</span></span>|<span data-ttu-id="9844e-310">Android Patch Sicherheitsstufe Inherited von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-310">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-311">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="9844e-311">userDisplayName</span></span>|<span data-ttu-id="9844e-312">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-312">String</span></span>|<span data-ttu-id="9844e-313">Anzeigename des Benutzers Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-313">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="9844e-314">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="9844e-315">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="9844e-315">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="9844e-316">ConfigrMgr-Client aktiviert Inherited-Funktionen, [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-316">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-317">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="9844e-317">wiFiMacAddress</span></span>|<span data-ttu-id="9844e-318">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-318">String</span></span>|<span data-ttu-id="9844e-319">Wi-Fi MAC von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt.</span><span class="sxs-lookup"><span data-stu-id="9844e-319">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="9844e-320">deviceHealthAttestationState</span></span>|[<span data-ttu-id="9844e-321">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="9844e-321">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="9844e-322">Status des Integritätsnachweises für Geräte.
</span><span class="sxs-lookup"><span data-stu-id="9844e-322">The device health attestation state.</span></span> <span data-ttu-id="9844e-323">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-324">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="9844e-324">subscriberCarrier</span></span>|<span data-ttu-id="9844e-325">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-325">String</span></span>|<span data-ttu-id="9844e-326">Abonnenten des Netzbetreibers von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt.</span><span class="sxs-lookup"><span data-stu-id="9844e-326">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-327">meid</span><span class="sxs-lookup"><span data-stu-id="9844e-327">meid</span></span>|<span data-ttu-id="9844e-328">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-328">String</span></span>|<span data-ttu-id="9844e-329">MEID von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="9844e-329">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-330">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="9844e-330">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="9844e-331">Int64</span><span class="sxs-lookup"><span data-stu-id="9844e-331">Int64</span></span>|<span data-ttu-id="9844e-332">Gesamtspeicher in Bytes von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="9844e-332">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-333">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="9844e-333">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="9844e-334">Int64</span><span class="sxs-lookup"><span data-stu-id="9844e-334">Int64</span></span>|<span data-ttu-id="9844e-335">Freien Speicher in Bytes von [ManagedDevice](../resources/intune-devices-manageddevice.md) geerbt</span><span class="sxs-lookup"><span data-stu-id="9844e-335">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-336">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="9844e-336">managedDeviceName</span></span>|<span data-ttu-id="9844e-337">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-337">String</span></span>|<span data-ttu-id="9844e-338">Automatisch generierter Name zur Identifizierung des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-338">Automatically generated name to identify a device.</span></span> <span data-ttu-id="9844e-339">Kann mit einem benutzerfreundlichen Namen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="9844e-339">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="9844e-340">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-340">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-341">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="9844e-341">partnerReportedThreatState</span></span>|[<span data-ttu-id="9844e-342">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="9844e-342">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="9844e-343">Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen.</span><span class="sxs-lookup"><span data-stu-id="9844e-343">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="9844e-344">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9844e-344">Read Only.</span></span> <span data-ttu-id="9844e-345">Geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="9844e-345">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="9844e-346">Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="9844e-346">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="9844e-347">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="9844e-347">usersLoggedOn</span></span>|<span data-ttu-id="9844e-348">[LoggedOnUser](../resources/intune-devices-loggedonuser.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9844e-348">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="9844e-349">Gibt das letzte angemeldete Benutzer eines Geräts Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-349">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-350">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="9844e-350">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="9844e-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9844e-351">DateTimeOffset</span></span>|<span data-ttu-id="9844e-352">Meldet den DateTime-Wert die Einstellung PreferMdmOverGroupPolicy festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="9844e-352">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="9844e-353">Wenn festgelegt ist, werden die Intune MDM Einstellungen Group Policy Settings außer Kraft setzen, wenn ein Konflikt vorliegt.</span><span class="sxs-lookup"><span data-stu-id="9844e-353">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="9844e-354">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9844e-354">Read Only.</span></span> <span data-ttu-id="9844e-355">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-355">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-356">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="9844e-356">autopilotEnrolled</span></span>|<span data-ttu-id="9844e-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="9844e-357">Boolean</span></span>|<span data-ttu-id="9844e-358">Gibt an, ob das verwaltete Geräte über den Auto-Pilot registriert ist.</span><span class="sxs-lookup"><span data-stu-id="9844e-358">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="9844e-359">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-360">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="9844e-360">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="9844e-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="9844e-361">Boolean</span></span>|<span data-ttu-id="9844e-362">Gibt an, ob das Gerät verwalteten iOS Benutzer Genehmigung Registrierung wird.</span><span class="sxs-lookup"><span data-stu-id="9844e-362">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="9844e-363">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-364">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="9844e-364">managementCertificateExpirationDate</span></span>|<span data-ttu-id="9844e-365">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9844e-365">DateTimeOffset</span></span>|<span data-ttu-id="9844e-366">Gerät Management Ablaufdatum des Zertifikats Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md) -Berichte</span><span class="sxs-lookup"><span data-stu-id="9844e-366">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-367">iccid</span><span class="sxs-lookup"><span data-stu-id="9844e-367">iccid</span></span>|<span data-ttu-id="9844e-368">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-368">String</span></span>|<span data-ttu-id="9844e-369">Chip Karte Bezeichner, ist es eine SIM-Karte eindeutige ID-Nummer.</span><span class="sxs-lookup"><span data-stu-id="9844e-369">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="9844e-370">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-370">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-371">UDID</span><span class="sxs-lookup"><span data-stu-id="9844e-371">udid</span></span>|<span data-ttu-id="9844e-372">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-372">String</span></span>|<span data-ttu-id="9844e-373">Eindeutige Geräte-ID für iOS und Mac OS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="9844e-373">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="9844e-374">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-375">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9844e-375">roleScopeTagIds</span></span>|<span data-ttu-id="9844e-376">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="9844e-376">String collection</span></span>|<span data-ttu-id="9844e-377">Liste der Bereichs-Tag-IDs für diese Instanz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9844e-377">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="9844e-378">Geerbt von [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-379">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="9844e-379">windowsActiveMalwareCount</span></span>|<span data-ttu-id="9844e-380">Int32</span><span class="sxs-lookup"><span data-stu-id="9844e-380">Int32</span></span>|<span data-ttu-id="9844e-381">Anzahl von aktiven Malware für dieses Windows-Gerät Inherited aus [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="9844e-381">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-382">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="9844e-382">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="9844e-383">Int32</span><span class="sxs-lookup"><span data-stu-id="9844e-383">Int32</span></span>|<span data-ttu-id="9844e-384">Anzahl der für das Windows-Gerät Inherited aus [ManagedDevice](../resources/intune-devices-manageddevice.md) für gewartete Schadsoftware</span><span class="sxs-lookup"><span data-stu-id="9844e-384">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-385">notes</span><span class="sxs-lookup"><span data-stu-id="9844e-385">notes</span></span>|<span data-ttu-id="9844e-386">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9844e-386">String</span></span>|<span data-ttu-id="9844e-387">Notes auf dem Gerät von IT Admin geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md) erstellt</span><span class="sxs-lookup"><span data-stu-id="9844e-387">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="9844e-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="9844e-388">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="9844e-389">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="9844e-389">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="9844e-390">Konfigurations-Manager-Client Integritätsstatus, gilt nur für Geräte, die von MDM/Configuration Manager-Agent geerbt von [ManagedDevice](../resources/intune-devices-manageddevice.md) verwaltet</span><span class="sxs-lookup"><span data-stu-id="9844e-390">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9844e-391">Antwort</span><span class="sxs-lookup"><span data-stu-id="9844e-391">Response</span></span>
<span data-ttu-id="9844e-392">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9844e-392">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9844e-393">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9844e-393">Example</span></span>

### <a name="request"></a><span data-ttu-id="9844e-394">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9844e-394">Request</span></span>
<span data-ttu-id="9844e-395">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9844e-395">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices
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

### <a name="response"></a><span data-ttu-id="9844e-396">Antwort</span><span class="sxs-lookup"><span data-stu-id="9844e-396">Response</span></span>
<span data-ttu-id="9844e-p142">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9844e-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




