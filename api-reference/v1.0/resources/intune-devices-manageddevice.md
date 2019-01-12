---
title: managedDevice-Ressourcentyp
description: Über Intune verwaltete oder vorab registrierte Geräte
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3643ec5020ea088b2da423ed44d0a1596e53e6a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955730"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="90243-103">managedDevice-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="90243-103">managedDevice resource type</span></span>

> <span data-ttu-id="90243-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="90243-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90243-105">Über Intune verwaltete oder vorab registrierte Geräte</span><span class="sxs-lookup"><span data-stu-id="90243-105">Devices that are managed or pre-enrolled through Intune</span></span>
## <a name="methods"></a><span data-ttu-id="90243-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="90243-106">Methods</span></span>
|<span data-ttu-id="90243-107">Methode</span><span class="sxs-lookup"><span data-stu-id="90243-107">Method</span></span>|<span data-ttu-id="90243-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="90243-108">Return Type</span></span>|<span data-ttu-id="90243-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90243-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="90243-110">managedDevices auflisten</span><span class="sxs-lookup"><span data-stu-id="90243-110">List managedDevices</span></span>](../api/intune-devices-manageddevice-list.md)|<span data-ttu-id="90243-111">[managedDevice](../resources/intune-devices-manageddevice.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="90243-111">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="90243-112">Auflisten von Eigenschaften und Beziehungen der [managedDevice](../resources/intune-devices-manageddevice.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="90243-112">List properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) objects.</span></span>|
|[<span data-ttu-id="90243-113">managedDevice abrufen</span><span class="sxs-lookup"><span data-stu-id="90243-113">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="90243-114">managedDevice</span><span class="sxs-lookup"><span data-stu-id="90243-114">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="90243-115">Lesen von Eigenschaften und Beziehungen des [managedDevice](../resources/intune-devices-manageddevice.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="90243-115">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="90243-116">managedDevice erstellen</span><span class="sxs-lookup"><span data-stu-id="90243-116">Create managedDevice</span></span>](../api/intune-devices-manageddevice-create.md)|[<span data-ttu-id="90243-117">managedDevice</span><span class="sxs-lookup"><span data-stu-id="90243-117">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="90243-118">Erstellen eines neuen [managedDevice](../resources/intune-devices-manageddevice.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="90243-118">Create a new [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="90243-119">managedDevice löschen</span><span class="sxs-lookup"><span data-stu-id="90243-119">Delete managedDevice</span></span>](../api/intune-devices-manageddevice-delete.md)|<span data-ttu-id="90243-120">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-120">None</span></span>|<span data-ttu-id="90243-121">Löscht ein [managedDevice löschen](../resources/intune-devices-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="90243-121">Deletes a [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>|
|[<span data-ttu-id="90243-122">managedDevice aktualisieren</span><span class="sxs-lookup"><span data-stu-id="90243-122">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="90243-123">managedDevice</span><span class="sxs-lookup"><span data-stu-id="90243-123">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="90243-124">Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune-devices-manageddevice.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="90243-124">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="90243-125">retire-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-125">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="90243-126">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-126">None</span></span>|<span data-ttu-id="90243-127">Zurückziehen eines Geräts</span><span class="sxs-lookup"><span data-stu-id="90243-127">Retire a device</span></span>|
|[<span data-ttu-id="90243-128">wipe-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-128">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="90243-129">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-129">None</span></span>|<span data-ttu-id="90243-130">Zurücksetzen eines Geräts</span><span class="sxs-lookup"><span data-stu-id="90243-130">Wipe a device</span></span>|
|[<span data-ttu-id="90243-131">resetPasscode-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-131">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="90243-132">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-132">None</span></span>|<span data-ttu-id="90243-133">Kennung zurücksetzen</span><span class="sxs-lookup"><span data-stu-id="90243-133">Reset passcode</span></span>|
|[<span data-ttu-id="90243-134">remoteLock-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-134">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="90243-135">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-135">None</span></span>|<span data-ttu-id="90243-136">Remotesperre</span><span class="sxs-lookup"><span data-stu-id="90243-136">Remote lock</span></span>|
|[<span data-ttu-id="90243-137">requestRemoteAssistance-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-137">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="90243-138">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-138">None</span></span>|<span data-ttu-id="90243-139">Remoteunterstützung anfordern</span><span class="sxs-lookup"><span data-stu-id="90243-139">Request remote assistance</span></span>|
|[<span data-ttu-id="90243-140">disableLostMode-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-140">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="90243-141">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-141">None</span></span>|<span data-ttu-id="90243-142">Modus für verlorene Geräte deaktivieren</span><span class="sxs-lookup"><span data-stu-id="90243-142">Disable lost mode</span></span>|
|[<span data-ttu-id="90243-143">locateDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-143">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="90243-144">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-144">None</span></span>|<span data-ttu-id="90243-145">Suchen eines Geräts</span><span class="sxs-lookup"><span data-stu-id="90243-145">Locate a device</span></span>|
|[<span data-ttu-id="90243-146">bypassActivationLock-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-146">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="90243-147">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-147">None</span></span>|<span data-ttu-id="90243-148">Aktivierungssperre umgehen</span><span class="sxs-lookup"><span data-stu-id="90243-148">Bypass activation lock</span></span>|
|[<span data-ttu-id="90243-149">rebootNow-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-149">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="90243-150">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-150">None</span></span>|<span data-ttu-id="90243-151">Gerät neu starten</span><span class="sxs-lookup"><span data-stu-id="90243-151">Reboot device</span></span>|
|[<span data-ttu-id="90243-152">shutDown-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-152">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="90243-153">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-153">None</span></span>|<span data-ttu-id="90243-154">Gerät abschalten</span><span class="sxs-lookup"><span data-stu-id="90243-154">Shut down device</span></span>|
|[<span data-ttu-id="90243-155">recoverPasscode-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-155">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="90243-156">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-156">None</span></span>|<span data-ttu-id="90243-157">Kennung wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="90243-157">Recover passcode</span></span>|
|[<span data-ttu-id="90243-158">cleanWindowsDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-158">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="90243-159">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-159">None</span></span>|<span data-ttu-id="90243-160">Windows-Gerät bereinigen</span><span class="sxs-lookup"><span data-stu-id="90243-160">Clean Windows device</span></span>|
|[<span data-ttu-id="90243-161">logoutSharedAppleDeviceActiveUser-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-161">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="90243-162">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-162">None</span></span>|<span data-ttu-id="90243-163">Aktiven Benutzer von freigegebenem Apple-Gerät abmelden</span><span class="sxs-lookup"><span data-stu-id="90243-163">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="90243-164">deleteUserFromSharedAppleDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-164">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="90243-165">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-165">None</span></span>|<span data-ttu-id="90243-166">Benutzer von freigegebenem Apple-Gerät löschen</span><span class="sxs-lookup"><span data-stu-id="90243-166">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="90243-167">syncDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-167">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="90243-168">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-168">None</span></span>|<span data-ttu-id="90243-169">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="90243-169">Not yet documented</span></span>|
|[<span data-ttu-id="90243-170">windowsDefenderScan-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-170">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="90243-171">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-171">None</span></span>|<span data-ttu-id="90243-172">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="90243-172">Not yet documented</span></span>|
|[<span data-ttu-id="90243-173">windowsDefenderUpdateSignatures-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-173">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="90243-174">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-174">None</span></span>|<span data-ttu-id="90243-175">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="90243-175">Not yet documented</span></span>|
|[<span data-ttu-id="90243-176">updateWindowsDeviceAccount-Aktion</span><span class="sxs-lookup"><span data-stu-id="90243-176">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="90243-177">Keine</span><span class="sxs-lookup"><span data-stu-id="90243-177">None</span></span>|<span data-ttu-id="90243-178">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="90243-178">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="90243-179">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="90243-179">Properties</span></span>
|<span data-ttu-id="90243-180">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="90243-180">Property</span></span>|<span data-ttu-id="90243-181">Typ</span><span class="sxs-lookup"><span data-stu-id="90243-181">Type</span></span>|<span data-ttu-id="90243-182">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90243-182">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90243-183">id</span><span class="sxs-lookup"><span data-stu-id="90243-183">id</span></span>|<span data-ttu-id="90243-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-184">String</span></span>|<span data-ttu-id="90243-185">Eindeutiger Bezeichner für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="90243-185">Unique Identifier for the device</span></span>|
|<span data-ttu-id="90243-186">userId</span><span class="sxs-lookup"><span data-stu-id="90243-186">userId</span></span>|<span data-ttu-id="90243-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-187">String</span></span>|<span data-ttu-id="90243-188">Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="90243-188">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="90243-189">deviceName</span><span class="sxs-lookup"><span data-stu-id="90243-189">deviceName</span></span>|<span data-ttu-id="90243-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-190">String</span></span>|<span data-ttu-id="90243-191">Name des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="90243-191">Name of the device</span></span>|
|<span data-ttu-id="90243-192">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="90243-192">managedDeviceOwnerType</span></span>|[<span data-ttu-id="90243-193">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="90243-193">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="90243-194">Besitz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="90243-194">Ownership of the device.</span></span> <span data-ttu-id="90243-195">'Company' oder 'Privat' kann sein.</span><span class="sxs-lookup"><span data-stu-id="90243-195">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="90243-196">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="90243-196">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="90243-197">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="90243-197">deviceActionResults</span></span>|<span data-ttu-id="90243-198">Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="90243-198">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="90243-199">Liste von Objekten des Typs „ComplexType deviceActionResult“.
</span><span class="sxs-lookup"><span data-stu-id="90243-199">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="90243-200">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="90243-200">enrolledDateTime</span></span>|<span data-ttu-id="90243-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90243-201">DateTimeOffset</span></span>|<span data-ttu-id="90243-202">Datum und Uhrzeit der Geräteregistrierung.
</span><span class="sxs-lookup"><span data-stu-id="90243-202">Enrollment time of the device.</span></span>|
|<span data-ttu-id="90243-203">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="90243-203">lastSyncDateTime</span></span>|<span data-ttu-id="90243-204">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90243-204">DateTimeOffset</span></span>|<span data-ttu-id="90243-205">Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
</span><span class="sxs-lookup"><span data-stu-id="90243-205">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="90243-206">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="90243-206">operatingSystem</span></span>|<span data-ttu-id="90243-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-207">String</span></span>|<span data-ttu-id="90243-208">Betriebssystem des Geräts.</span><span class="sxs-lookup"><span data-stu-id="90243-208">Operating system of the device.</span></span> <span data-ttu-id="90243-209">Windows, iOS usw.</span><span class="sxs-lookup"><span data-stu-id="90243-209">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="90243-210">complianceState</span><span class="sxs-lookup"><span data-stu-id="90243-210">complianceState</span></span>|[<span data-ttu-id="90243-211">complianceState</span><span class="sxs-lookup"><span data-stu-id="90243-211">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="90243-212">Konformitätsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="90243-212">Compliance state of the device.</span></span> <span data-ttu-id="90243-213">Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.</span><span class="sxs-lookup"><span data-stu-id="90243-213">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="90243-214">jailBroken</span><span class="sxs-lookup"><span data-stu-id="90243-214">jailBroken</span></span>|<span data-ttu-id="90243-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-215">String</span></span>|<span data-ttu-id="90243-216">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="90243-216">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="90243-217">managementAgent</span><span class="sxs-lookup"><span data-stu-id="90243-217">managementAgent</span></span>|[<span data-ttu-id="90243-218">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="90243-218">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="90243-219">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="90243-219">Management channel of the device.</span></span> <span data-ttu-id="90243-220">Intune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf` und `googleCloudDevicePolicyController`.</span><span class="sxs-lookup"><span data-stu-id="90243-220">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="90243-221">osVersion</span><span class="sxs-lookup"><span data-stu-id="90243-221">osVersion</span></span>|<span data-ttu-id="90243-222">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-222">String</span></span>|<span data-ttu-id="90243-223">Auf dem Gerät installierte Betriebssystemversion.
</span><span class="sxs-lookup"><span data-stu-id="90243-223">Operating system version of the device.</span></span>|
|<span data-ttu-id="90243-224">easActivated</span><span class="sxs-lookup"><span data-stu-id="90243-224">easActivated</span></span>|<span data-ttu-id="90243-225">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="90243-225">Boolean</span></span>|<span data-ttu-id="90243-226">Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="90243-226">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="90243-227">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="90243-227">easDeviceId</span></span>|<span data-ttu-id="90243-228">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-228">String</span></span>|<span data-ttu-id="90243-229">Exchange ActiveSync-ID des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="90243-229">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="90243-230">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="90243-230">easActivationDateTime</span></span>|<span data-ttu-id="90243-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90243-231">DateTimeOffset</span></span>|<span data-ttu-id="90243-232">Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="90243-232">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="90243-233">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="90243-233">azureADRegistered</span></span>|<span data-ttu-id="90243-234">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="90243-234">Boolean</span></span>|<span data-ttu-id="90243-235">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="90243-235">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="90243-236">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="90243-236">deviceEnrollmentType</span></span>|[<span data-ttu-id="90243-237">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="90243-237">deviceEnrollmentType</span></span>](../resources/intune-devices-deviceenrollmenttype.md)|<span data-ttu-id="90243-238">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="90243-238">Enrollment type of the device.</span></span> <span data-ttu-id="90243-239">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="90243-239">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="90243-240">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="90243-240">activationLockBypassCode</span></span>|<span data-ttu-id="90243-241">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-241">String</span></span>|<span data-ttu-id="90243-242">Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht</span><span class="sxs-lookup"><span data-stu-id="90243-242">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="90243-243">emailAddress</span><span class="sxs-lookup"><span data-stu-id="90243-243">emailAddress</span></span>|<span data-ttu-id="90243-244">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-244">String</span></span>|<span data-ttu-id="90243-245">E-Mail-Adressen des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="90243-245">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="90243-246">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="90243-246">azureADDeviceId</span></span>|<span data-ttu-id="90243-247">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-247">String</span></span>|<span data-ttu-id="90243-248">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="90243-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="90243-249">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="90243-249">Read only.</span></span>|
|<span data-ttu-id="90243-250">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="90243-250">deviceRegistrationState</span></span>|[<span data-ttu-id="90243-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="90243-251">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="90243-252">Registrierungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="90243-252">Device registration state.</span></span> <span data-ttu-id="90243-253">Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="90243-253">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="90243-254">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="90243-254">deviceCategoryDisplayName</span></span>|<span data-ttu-id="90243-255">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-255">String</span></span>|<span data-ttu-id="90243-256">Anzeigename der Gerätekategorie.
</span><span class="sxs-lookup"><span data-stu-id="90243-256">Device category display name</span></span>|
|<span data-ttu-id="90243-257">isSupervised</span><span class="sxs-lookup"><span data-stu-id="90243-257">isSupervised</span></span>|<span data-ttu-id="90243-258">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="90243-258">Boolean</span></span>|<span data-ttu-id="90243-259">Überwachungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="90243-259">Device supervised status</span></span>|
|<span data-ttu-id="90243-260">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="90243-260">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="90243-261">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90243-261">DateTimeOffset</span></span>|<span data-ttu-id="90243-262">Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange</span><span class="sxs-lookup"><span data-stu-id="90243-262">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="90243-263">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="90243-263">exchangeAccessState</span></span>|[<span data-ttu-id="90243-264">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="90243-264">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="90243-265">Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="90243-265">The Access State of the device in Exchange.</span></span> <span data-ttu-id="90243-266">Mögliche Werte sind: `none`, `unknown`, `allowed`, `blocked` und `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="90243-266">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="90243-267">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="90243-267">exchangeAccessStateReason</span></span>|[<span data-ttu-id="90243-268">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="90243-268">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="90243-269">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="90243-269">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="90243-270">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="90243-270">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="90243-271">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="90243-271">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="90243-272">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-272">String</span></span>|<span data-ttu-id="90243-273">URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
</span><span class="sxs-lookup"><span data-stu-id="90243-273">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="90243-274">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="90243-274">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="90243-275">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-275">String</span></span>|<span data-ttu-id="90243-276">Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
</span><span class="sxs-lookup"><span data-stu-id="90243-276">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="90243-277">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="90243-277">isEncrypted</span></span>|<span data-ttu-id="90243-278">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="90243-278">Boolean</span></span>|<span data-ttu-id="90243-279">Verschlüsselungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="90243-279">Device encryption status</span></span>|
|<span data-ttu-id="90243-280">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="90243-280">userPrincipalName</span></span>|<span data-ttu-id="90243-281">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-281">String</span></span>|<span data-ttu-id="90243-282">Benutzerprinzipalname für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="90243-282">Device user principal name</span></span>|
|<span data-ttu-id="90243-283">model</span><span class="sxs-lookup"><span data-stu-id="90243-283">model</span></span>|<span data-ttu-id="90243-284">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-284">String</span></span>|<span data-ttu-id="90243-285">Modell des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="90243-285">Model of the device</span></span>|
|<span data-ttu-id="90243-286">manufacturer</span><span class="sxs-lookup"><span data-stu-id="90243-286">manufacturer</span></span>|<span data-ttu-id="90243-287">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-287">String</span></span>|<span data-ttu-id="90243-288">Hersteller des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="90243-288">Manufacturer of the device</span></span>|
|<span data-ttu-id="90243-289">imei</span><span class="sxs-lookup"><span data-stu-id="90243-289">imei</span></span>|<span data-ttu-id="90243-290">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-290">String</span></span>|<span data-ttu-id="90243-291">IMEI</span><span class="sxs-lookup"><span data-stu-id="90243-291">IMEI</span></span>|
|<span data-ttu-id="90243-292">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="90243-292">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="90243-293">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90243-293">DateTimeOffset</span></span>|<span data-ttu-id="90243-294">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität.
</span><span class="sxs-lookup"><span data-stu-id="90243-294">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="90243-295">serialNumber</span><span class="sxs-lookup"><span data-stu-id="90243-295">serialNumber</span></span>|<span data-ttu-id="90243-296">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-296">String</span></span>|<span data-ttu-id="90243-297">Seriennummer.
</span><span class="sxs-lookup"><span data-stu-id="90243-297">SerialNumber</span></span>|
|<span data-ttu-id="90243-298">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="90243-298">phoneNumber</span></span>|<span data-ttu-id="90243-299">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-299">String</span></span>|<span data-ttu-id="90243-300">Telefonnummer des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="90243-300">Phone number of the device</span></span>|
|<span data-ttu-id="90243-301">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="90243-301">androidSecurityPatchLevel</span></span>|<span data-ttu-id="90243-302">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-302">String</span></span>|<span data-ttu-id="90243-303">Android-Sicherheitspatchlevel.
</span><span class="sxs-lookup"><span data-stu-id="90243-303">Android security patch level</span></span>|
|<span data-ttu-id="90243-304">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="90243-304">userDisplayName</span></span>|<span data-ttu-id="90243-305">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-305">String</span></span>|<span data-ttu-id="90243-306">Anzeigename des Benutzers.
</span><span class="sxs-lookup"><span data-stu-id="90243-306">User display name</span></span>|
|<span data-ttu-id="90243-307">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="90243-307">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="90243-308">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="90243-308">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="90243-309">Aktivierte Funktionen des Konfigurations-Manager-Clients.
</span><span class="sxs-lookup"><span data-stu-id="90243-309">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="90243-310">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="90243-310">wiFiMacAddress</span></span>|<span data-ttu-id="90243-311">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-311">String</span></span>|<span data-ttu-id="90243-312">WLAN-MAC</span><span class="sxs-lookup"><span data-stu-id="90243-312">Wi-Fi MAC</span></span>|
|<span data-ttu-id="90243-313">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="90243-313">deviceHealthAttestationState</span></span>|[<span data-ttu-id="90243-314">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="90243-314">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="90243-315">Status des Integritätsnachweises für Geräte.
</span><span class="sxs-lookup"><span data-stu-id="90243-315">The device health attestation state.</span></span>|
|<span data-ttu-id="90243-316">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="90243-316">subscriberCarrier</span></span>|<span data-ttu-id="90243-317">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-317">String</span></span>|<span data-ttu-id="90243-318">Netzbetreiber des Abonnenten.
</span><span class="sxs-lookup"><span data-stu-id="90243-318">Subscriber Carrier</span></span>|
|<span data-ttu-id="90243-319">meid</span><span class="sxs-lookup"><span data-stu-id="90243-319">meid</span></span>|<span data-ttu-id="90243-320">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-320">String</span></span>|<span data-ttu-id="90243-321">MEID</span><span class="sxs-lookup"><span data-stu-id="90243-321">MEID</span></span>|
|<span data-ttu-id="90243-322">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="90243-322">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="90243-323">Int64</span><span class="sxs-lookup"><span data-stu-id="90243-323">Int64</span></span>|<span data-ttu-id="90243-324">Gesamtspeicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="90243-324">Total Storage in Bytes</span></span>|
|<span data-ttu-id="90243-325">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="90243-325">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="90243-326">Int64</span><span class="sxs-lookup"><span data-stu-id="90243-326">Int64</span></span>|<span data-ttu-id="90243-327">Freier Speicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="90243-327">Free Storage in Bytes</span></span>|
|<span data-ttu-id="90243-328">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="90243-328">managedDeviceName</span></span>|<span data-ttu-id="90243-329">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="90243-329">String</span></span>|<span data-ttu-id="90243-330">Automatisch generierter Name zur Identifizierung des Geräts.</span><span class="sxs-lookup"><span data-stu-id="90243-330">Automatically generated name to identify a device.</span></span> <span data-ttu-id="90243-331">Kann mit einem benutzerfreundlichen Namen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="90243-331">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="90243-332">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="90243-332">partnerReportedThreatState</span></span>|[<span data-ttu-id="90243-333">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="90243-333">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="90243-334">Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen.</span><span class="sxs-lookup"><span data-stu-id="90243-334">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="90243-335">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="90243-335">Read Only.</span></span> <span data-ttu-id="90243-336">Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="90243-336">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90243-337">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="90243-337">Relationships</span></span>
|<span data-ttu-id="90243-338">Beziehung</span><span class="sxs-lookup"><span data-stu-id="90243-338">Relationship</span></span>|<span data-ttu-id="90243-339">Typ</span><span class="sxs-lookup"><span data-stu-id="90243-339">Type</span></span>|<span data-ttu-id="90243-340">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90243-340">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90243-341">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="90243-341">deviceCategory</span></span>|[<span data-ttu-id="90243-342">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="90243-342">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="90243-343">Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="90243-343">Device category</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90243-344">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="90243-344">JSON Representation</span></span>
<span data-ttu-id="90243-345">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="90243-345">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "operatingSystem": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": true,
  "userPrincipalName": "String",
  "model": "String",
  "manufacturer": "String",
  "imei": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "serialNumber": "String",
  "phoneNumber": "String",
  "androidSecurityPatchLevel": "String",
  "userDisplayName": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "String",
    "contentNamespaceUrl": "String",
    "deviceHealthAttestationStatus": "String",
    "contentVersion": "String",
    "issuedDateTime": "String (timestamp)",
    "attestationIdentityKey": "String",
    "resetCount": 1024,
    "restartCount": 1024,
    "dataExcutionPolicy": "String",
    "bitLockerStatus": "String",
    "bootManagerVersion": "String",
    "codeIntegrityCheckVersion": "String",
    "secureBoot": "String",
    "bootDebugging": "String",
    "operatingSystemKernelDebugging": "String",
    "codeIntegrity": "String",
    "testSigning": "String",
    "safeMode": "String",
    "windowsPE": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "virtualSecureMode": "String",
    "pcrHashAlgorithm": "String",
    "bootAppSecurityVersion": "String",
    "bootManagerSecurityVersion": "String",
    "tpmVersion": "String",
    "pcr0": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "codeIntegrityPolicy": "String",
    "bootRevisionListInfo": "String",
    "operatingSystemRevListInfo": "String",
    "healthStatusMismatchInfo": "String",
    "healthAttestationSupportedStatus": "String"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": 1024,
  "freeStorageSpaceInBytes": 1024,
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String"
}
```



