---
title: managedDevice-Ressourcentyp
description: Über Intune verwaltete oder vorab registrierte Geräte
ms.openlocfilehash: eaca9444df77c2f95f6a6f9845c9383cd53cd99f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063524"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="67bb5-103">managedDevice-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="67bb5-103">managedDevice resource type</span></span>

> <span data-ttu-id="67bb5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="67bb5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67bb5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="67bb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67bb5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="67bb5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67bb5-107">Über Intune verwaltete oder vorab registrierte Geräte</span><span class="sxs-lookup"><span data-stu-id="67bb5-107">Devices that are managed or pre-enrolled through Intune</span></span>
## <a name="methods"></a><span data-ttu-id="67bb5-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="67bb5-108">Methods</span></span>
|<span data-ttu-id="67bb5-109">Methode</span><span class="sxs-lookup"><span data-stu-id="67bb5-109">Method</span></span>|<span data-ttu-id="67bb5-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="67bb5-110">Return Type</span></span>|<span data-ttu-id="67bb5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67bb5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="67bb5-112">managedDevice abrufen</span><span class="sxs-lookup"><span data-stu-id="67bb5-112">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="67bb5-113">managedDevice</span><span class="sxs-lookup"><span data-stu-id="67bb5-113">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="67bb5-114">Lesen von Eigenschaften und Beziehungen des [managedDevice](../resources/intune-devices-manageddevice.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-114">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="67bb5-115">managedDevice aktualisieren</span><span class="sxs-lookup"><span data-stu-id="67bb5-115">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="67bb5-116">managedDevice</span><span class="sxs-lookup"><span data-stu-id="67bb5-116">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="67bb5-117">Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune-devices-manageddevice.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-117">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="67bb5-118">ExecuteAction-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-118">executeAction action</span></span>](../api/intune-devices-manageddevice-executeaction.md)|[<span data-ttu-id="67bb5-119">bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="67bb5-119">bulkManagedDeviceActionResult</span></span>](../resources/intune-devices-bulkmanageddeviceactionresult.md)|<span data-ttu-id="67bb5-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="67bb5-120">Not yet documented</span></span>|
|[<span data-ttu-id="67bb5-121">EnableLostMode Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-121">enableLostMode action</span></span>](../api/intune-devices-manageddevice-enablelostmode.md)|<span data-ttu-id="67bb5-122">Keines</span><span class="sxs-lookup"><span data-stu-id="67bb5-122">None</span></span>|<span data-ttu-id="67bb5-123">Verloren-Modus aktivieren</span><span class="sxs-lookup"><span data-stu-id="67bb5-123">Enable lost mode</span></span>|
|[<span data-ttu-id="67bb5-124">PlayLostModeSound Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-124">playLostModeSound action</span></span>](../api/intune-devices-manageddevice-playlostmodesound.md)|<span data-ttu-id="67bb5-125">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-125">None</span></span>|<span data-ttu-id="67bb5-126">Remotesperre</span><span class="sxs-lookup"><span data-stu-id="67bb5-126">Remote lock</span></span>|
|[<span data-ttu-id="67bb5-127">SetDeviceName Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-127">setDeviceName action</span></span>](../api/intune-devices-manageddevice-setdevicename.md)|<span data-ttu-id="67bb5-128">Keines</span><span class="sxs-lookup"><span data-stu-id="67bb5-128">None</span></span>|<span data-ttu-id="67bb5-129">Festlegen Sie Name des Aufnahmegeräts des Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-129">Set device name of the device.</span></span>|
|[<span data-ttu-id="67bb5-130">retire-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-130">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="67bb5-131">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-131">None</span></span>|<span data-ttu-id="67bb5-132">Zurückziehen eines Geräts</span><span class="sxs-lookup"><span data-stu-id="67bb5-132">Retire a device</span></span>|
|[<span data-ttu-id="67bb5-133">wipe-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-133">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="67bb5-134">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-134">None</span></span>|<span data-ttu-id="67bb5-135">Zurücksetzen eines Geräts</span><span class="sxs-lookup"><span data-stu-id="67bb5-135">Wipe a device</span></span>|
|[<span data-ttu-id="67bb5-136">resetPasscode-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-136">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="67bb5-137">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-137">None</span></span>|<span data-ttu-id="67bb5-138">Kennung zurücksetzen</span><span class="sxs-lookup"><span data-stu-id="67bb5-138">Reset passcode</span></span>|
|[<span data-ttu-id="67bb5-139">remoteLock-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-139">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="67bb5-140">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-140">None</span></span>|<span data-ttu-id="67bb5-141">Remotesperre</span><span class="sxs-lookup"><span data-stu-id="67bb5-141">Remote lock</span></span>|
|[<span data-ttu-id="67bb5-142">requestRemoteAssistance-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-142">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="67bb5-143">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-143">None</span></span>|<span data-ttu-id="67bb5-144">Remoteunterstützung anfordern</span><span class="sxs-lookup"><span data-stu-id="67bb5-144">Request remote assistance</span></span>|
|[<span data-ttu-id="67bb5-145">disableLostMode-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-145">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="67bb5-146">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-146">None</span></span>|<span data-ttu-id="67bb5-147">Modus für verlorene Geräte deaktivieren</span><span class="sxs-lookup"><span data-stu-id="67bb5-147">Disable lost mode</span></span>|
|[<span data-ttu-id="67bb5-148">locateDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-148">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="67bb5-149">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-149">None</span></span>|<span data-ttu-id="67bb5-150">Suchen eines Geräts</span><span class="sxs-lookup"><span data-stu-id="67bb5-150">Locate a device</span></span>|
|[<span data-ttu-id="67bb5-151">bypassActivationLock-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-151">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="67bb5-152">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-152">None</span></span>|<span data-ttu-id="67bb5-153">Aktivierungssperre umgehen</span><span class="sxs-lookup"><span data-stu-id="67bb5-153">Bypass activation lock</span></span>|
|[<span data-ttu-id="67bb5-154">rebootNow-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-154">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="67bb5-155">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-155">None</span></span>|<span data-ttu-id="67bb5-156">Gerät neu starten</span><span class="sxs-lookup"><span data-stu-id="67bb5-156">Reboot device</span></span>|
|[<span data-ttu-id="67bb5-157">shutDown-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-157">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="67bb5-158">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-158">None</span></span>|<span data-ttu-id="67bb5-159">Gerät abschalten</span><span class="sxs-lookup"><span data-stu-id="67bb5-159">Shut down device</span></span>|
|[<span data-ttu-id="67bb5-160">recoverPasscode-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-160">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="67bb5-161">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-161">None</span></span>|<span data-ttu-id="67bb5-162">Kennung wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="67bb5-162">Recover passcode</span></span>|
|[<span data-ttu-id="67bb5-163">cleanWindowsDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-163">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="67bb5-164">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-164">None</span></span>|<span data-ttu-id="67bb5-165">Windows-Gerät bereinigen</span><span class="sxs-lookup"><span data-stu-id="67bb5-165">Clean Windows device</span></span>|
|[<span data-ttu-id="67bb5-166">logoutSharedAppleDeviceActiveUser-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-166">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="67bb5-167">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-167">None</span></span>|<span data-ttu-id="67bb5-168">Aktiven Benutzer von freigegebenem Apple-Gerät abmelden</span><span class="sxs-lookup"><span data-stu-id="67bb5-168">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="67bb5-169">deleteUserFromSharedAppleDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-169">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="67bb5-170">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-170">None</span></span>|<span data-ttu-id="67bb5-171">Benutzer von freigegebenem Apple-Gerät löschen</span><span class="sxs-lookup"><span data-stu-id="67bb5-171">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="67bb5-172">syncDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-172">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="67bb5-173">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-173">None</span></span>|<span data-ttu-id="67bb5-174">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="67bb5-174">Not yet documented</span></span>|
|[<span data-ttu-id="67bb5-175">windowsDefenderScan-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-175">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="67bb5-176">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-176">None</span></span>|<span data-ttu-id="67bb5-177">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="67bb5-177">Not yet documented</span></span>|
|[<span data-ttu-id="67bb5-178">windowsDefenderUpdateSignatures-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-178">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="67bb5-179">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-179">None</span></span>|<span data-ttu-id="67bb5-180">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="67bb5-180">Not yet documented</span></span>|
|[<span data-ttu-id="67bb5-181">updateWindowsDeviceAccount-Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-181">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="67bb5-182">Keine</span><span class="sxs-lookup"><span data-stu-id="67bb5-182">None</span></span>|<span data-ttu-id="67bb5-183">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="67bb5-183">Not yet documented</span></span>|
|[<span data-ttu-id="67bb5-184">RevokeAppleVppLicenses Aktion</span><span class="sxs-lookup"><span data-stu-id="67bb5-184">revokeAppleVppLicenses action</span></span>](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|<span data-ttu-id="67bb5-185">Keines</span><span class="sxs-lookup"><span data-stu-id="67bb5-185">None</span></span>|<span data-ttu-id="67bb5-186">Alle Apple Vpp Lizenzen für ein Gerät widerrufen</span><span class="sxs-lookup"><span data-stu-id="67bb5-186">Revoke all Apple Vpp licenses for a device</span></span>|

## <a name="properties"></a><span data-ttu-id="67bb5-187">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="67bb5-187">Properties</span></span>
|<span data-ttu-id="67bb5-188">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="67bb5-188">Property</span></span>|<span data-ttu-id="67bb5-189">Typ</span><span class="sxs-lookup"><span data-stu-id="67bb5-189">Type</span></span>|<span data-ttu-id="67bb5-190">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67bb5-190">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67bb5-191">id</span><span class="sxs-lookup"><span data-stu-id="67bb5-191">id</span></span>|<span data-ttu-id="67bb5-192">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-192">String</span></span>|<span data-ttu-id="67bb5-193">Eindeutiger Bezeichner für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-193">Unique Identifier for the device</span></span>|
|<span data-ttu-id="67bb5-194">userId</span><span class="sxs-lookup"><span data-stu-id="67bb5-194">userId</span></span>|<span data-ttu-id="67bb5-195">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-195">String</span></span>|<span data-ttu-id="67bb5-196">Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-196">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="67bb5-197">deviceName</span><span class="sxs-lookup"><span data-stu-id="67bb5-197">deviceName</span></span>|<span data-ttu-id="67bb5-198">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-198">String</span></span>|<span data-ttu-id="67bb5-199">Name des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-199">Name of the device</span></span>|
|<span data-ttu-id="67bb5-200">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="67bb5-200">hardwareInformation</span></span>|[<span data-ttu-id="67bb5-201">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="67bb5-201">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="67bb5-202">Die Hardward Details für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="67bb5-202">The hardward details for the device.</span></span>  <span data-ttu-id="67bb5-203">Enthält Informationen, wie Speicherplatz, Hersteller, Seriennummer.</span><span class="sxs-lookup"><span data-stu-id="67bb5-203">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="67bb5-204">Besitzertyp</span><span class="sxs-lookup"><span data-stu-id="67bb5-204">ownerType</span></span>|[<span data-ttu-id="67bb5-205">Besitzertyp</span><span class="sxs-lookup"><span data-stu-id="67bb5-205">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="67bb5-206">Besitz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-206">Ownership of the device.</span></span> <span data-ttu-id="67bb5-207">'Company' oder 'Privat' kann sein.</span><span class="sxs-lookup"><span data-stu-id="67bb5-207">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="67bb5-208">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="67bb5-208">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="67bb5-209">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="67bb5-209">managedDeviceOwnerType</span></span>|[<span data-ttu-id="67bb5-210">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="67bb5-210">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="67bb5-211">Besitz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-211">Ownership of the device.</span></span> <span data-ttu-id="67bb5-212">'Company' oder 'Privat' kann sein.</span><span class="sxs-lookup"><span data-stu-id="67bb5-212">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="67bb5-213">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="67bb5-213">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="67bb5-214">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="67bb5-214">deviceActionResults</span></span>|<span data-ttu-id="67bb5-215">Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="67bb5-215">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="67bb5-216">Liste von Objekten des Typs „ComplexType deviceActionResult“.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-216">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="67bb5-217">managementState</span><span class="sxs-lookup"><span data-stu-id="67bb5-217">managementState</span></span>|[<span data-ttu-id="67bb5-218">managementState</span><span class="sxs-lookup"><span data-stu-id="67bb5-218">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="67bb5-219">Verwaltungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-219">Management state of the device.</span></span> <span data-ttu-id="67bb5-220">Mögliche Werte sind: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled` und `discovered`.</span><span class="sxs-lookup"><span data-stu-id="67bb5-220">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="67bb5-221">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="67bb5-221">enrolledDateTime</span></span>|<span data-ttu-id="67bb5-222">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bb5-222">DateTimeOffset</span></span>|<span data-ttu-id="67bb5-223">Datum und Uhrzeit der Geräteregistrierung.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-223">Enrollment time of the device.</span></span>|
|<span data-ttu-id="67bb5-224">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="67bb5-224">lastSyncDateTime</span></span>|<span data-ttu-id="67bb5-225">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bb5-225">DateTimeOffset</span></span>|<span data-ttu-id="67bb5-226">Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-226">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="67bb5-227">chassisType</span><span class="sxs-lookup"><span data-stu-id="67bb5-227">chassisType</span></span>|[<span data-ttu-id="67bb5-228">chassisType</span><span class="sxs-lookup"><span data-stu-id="67bb5-228">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="67bb5-229">Chassistyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-229">Chassis type of the device.</span></span> <span data-ttu-id="67bb5-230">Mögliche Werte: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="67bb5-230">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="67bb5-231">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="67bb5-231">operatingSystem</span></span>|<span data-ttu-id="67bb5-232">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-232">String</span></span>|<span data-ttu-id="67bb5-233">Betriebssystem des Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-233">Operating system of the device.</span></span> <span data-ttu-id="67bb5-234">Windows, iOS usw.</span><span class="sxs-lookup"><span data-stu-id="67bb5-234">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="67bb5-235">deviceType</span><span class="sxs-lookup"><span data-stu-id="67bb5-235">deviceType</span></span>|[<span data-ttu-id="67bb5-236">deviceType</span><span class="sxs-lookup"><span data-stu-id="67bb5-236">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="67bb5-237">Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-237">Platform of the device.</span></span> <span data-ttu-id="67bb5-238">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="67bb5-238">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="67bb5-239">complianceState</span><span class="sxs-lookup"><span data-stu-id="67bb5-239">complianceState</span></span>|[<span data-ttu-id="67bb5-240">complianceState</span><span class="sxs-lookup"><span data-stu-id="67bb5-240">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="67bb5-241">Konformitätsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-241">Compliance state of the device.</span></span> <span data-ttu-id="67bb5-242">Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.</span><span class="sxs-lookup"><span data-stu-id="67bb5-242">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="67bb5-243">jailBroken</span><span class="sxs-lookup"><span data-stu-id="67bb5-243">jailBroken</span></span>|<span data-ttu-id="67bb5-244">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-244">String</span></span>|<span data-ttu-id="67bb5-245">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="67bb5-245">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="67bb5-246">managementAgent</span><span class="sxs-lookup"><span data-stu-id="67bb5-246">managementAgent</span></span>|[<span data-ttu-id="67bb5-247">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="67bb5-247">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="67bb5-248">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-248">Management channel of the device.</span></span> <span data-ttu-id="67bb5-249">Intune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="67bb5-249">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="67bb5-250">osVersion</span><span class="sxs-lookup"><span data-stu-id="67bb5-250">osVersion</span></span>|<span data-ttu-id="67bb5-251">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-251">String</span></span>|<span data-ttu-id="67bb5-252">Auf dem Gerät installierte Betriebssystemversion.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-252">Operating system version of the device.</span></span>|
|<span data-ttu-id="67bb5-253">easActivated</span><span class="sxs-lookup"><span data-stu-id="67bb5-253">easActivated</span></span>|<span data-ttu-id="67bb5-254">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="67bb5-254">Boolean</span></span>|<span data-ttu-id="67bb5-255">Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="67bb5-255">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="67bb5-256">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="67bb5-256">easDeviceId</span></span>|<span data-ttu-id="67bb5-257">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-257">String</span></span>|<span data-ttu-id="67bb5-258">Exchange ActiveSync-ID des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-258">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="67bb5-259">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="67bb5-259">easActivationDateTime</span></span>|<span data-ttu-id="67bb5-260">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bb5-260">DateTimeOffset</span></span>|<span data-ttu-id="67bb5-261">Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-261">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="67bb5-262">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="67bb5-262">aadRegistered</span></span>|<span data-ttu-id="67bb5-263">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="67bb5-263">Boolean</span></span>|<span data-ttu-id="67bb5-264">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="67bb5-264">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="67bb5-265">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="67bb5-265">azureADRegistered</span></span>|<span data-ttu-id="67bb5-266">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="67bb5-266">Boolean</span></span>|<span data-ttu-id="67bb5-267">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="67bb5-267">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="67bb5-268">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="67bb5-268">deviceEnrollmentType</span></span>|[<span data-ttu-id="67bb5-269">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="67bb5-269">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="67bb5-270">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-270">Enrollment type of the device.</span></span> <span data-ttu-id="67bb5-271">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="67bb5-271">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="67bb5-272">lostModeState</span><span class="sxs-lookup"><span data-stu-id="67bb5-272">lostModeState</span></span>|[<span data-ttu-id="67bb5-273">lostModeState</span><span class="sxs-lookup"><span data-stu-id="67bb5-273">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="67bb5-274">Gibt an, ob verloren-Modus aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="67bb5-274">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="67bb5-275">Mögliche Werte sind: `disabled` und `enabled`.</span><span class="sxs-lookup"><span data-stu-id="67bb5-275">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="67bb5-276">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="67bb5-276">activationLockBypassCode</span></span>|<span data-ttu-id="67bb5-277">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-277">String</span></span>|<span data-ttu-id="67bb5-278">Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht</span><span class="sxs-lookup"><span data-stu-id="67bb5-278">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="67bb5-279">emailAddress</span><span class="sxs-lookup"><span data-stu-id="67bb5-279">emailAddress</span></span>|<span data-ttu-id="67bb5-280">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-280">String</span></span>|<span data-ttu-id="67bb5-281">E-Mail-Adressen des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-281">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="67bb5-282">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="67bb5-282">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="67bb5-283">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-283">String</span></span>|<span data-ttu-id="67bb5-284">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-284">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="67bb5-285">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="67bb5-285">Read only.</span></span>|
|<span data-ttu-id="67bb5-286">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="67bb5-286">azureADDeviceId</span></span>|<span data-ttu-id="67bb5-287">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-287">String</span></span>|<span data-ttu-id="67bb5-288">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-288">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="67bb5-289">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="67bb5-289">Read only.</span></span>|
|<span data-ttu-id="67bb5-290">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="67bb5-290">deviceRegistrationState</span></span>|[<span data-ttu-id="67bb5-291">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="67bb5-291">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="67bb5-292">Registrierungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-292">Device registration state.</span></span> <span data-ttu-id="67bb5-293">Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="67bb5-293">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="67bb5-294">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="67bb5-294">deviceCategoryDisplayName</span></span>|<span data-ttu-id="67bb5-295">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-295">String</span></span>|<span data-ttu-id="67bb5-296">Anzeigename der Gerätekategorie.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-296">Device category display name</span></span>|
|<span data-ttu-id="67bb5-297">isSupervised</span><span class="sxs-lookup"><span data-stu-id="67bb5-297">isSupervised</span></span>|<span data-ttu-id="67bb5-298">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="67bb5-298">Boolean</span></span>|<span data-ttu-id="67bb5-299">Überwachungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-299">Device supervised status</span></span>|
|<span data-ttu-id="67bb5-300">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="67bb5-300">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="67bb5-301">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bb5-301">DateTimeOffset</span></span>|<span data-ttu-id="67bb5-302">Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange</span><span class="sxs-lookup"><span data-stu-id="67bb5-302">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="67bb5-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="67bb5-303">exchangeAccessState</span></span>|[<span data-ttu-id="67bb5-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="67bb5-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="67bb5-305">Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="67bb5-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="67bb5-306">Mögliche Werte sind: `none`, `unknown`, `allowed`, `blocked` und `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="67bb5-306">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="67bb5-307">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="67bb5-307">exchangeAccessStateReason</span></span>|[<span data-ttu-id="67bb5-308">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="67bb5-308">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="67bb5-309">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="67bb5-309">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="67bb5-310">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="67bb5-310">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="67bb5-311">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="67bb5-311">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="67bb5-312">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-312">String</span></span>|<span data-ttu-id="67bb5-313">URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-313">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="67bb5-314">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="67bb5-314">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="67bb5-315">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-315">String</span></span>|<span data-ttu-id="67bb5-316">Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-316">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="67bb5-317">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="67bb5-317">isEncrypted</span></span>|<span data-ttu-id="67bb5-318">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="67bb5-318">Boolean</span></span>|<span data-ttu-id="67bb5-319">Verschlüsselungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-319">Device encryption status</span></span>|
|<span data-ttu-id="67bb5-320">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="67bb5-320">userPrincipalName</span></span>|<span data-ttu-id="67bb5-321">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-321">String</span></span>|<span data-ttu-id="67bb5-322">Benutzerprinzipalname für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-322">Device user principal name</span></span>|
|<span data-ttu-id="67bb5-323">model</span><span class="sxs-lookup"><span data-stu-id="67bb5-323">model</span></span>|<span data-ttu-id="67bb5-324">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-324">String</span></span>|<span data-ttu-id="67bb5-325">Modell des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-325">Model of the device</span></span>|
|<span data-ttu-id="67bb5-326">manufacturer</span><span class="sxs-lookup"><span data-stu-id="67bb5-326">manufacturer</span></span>|<span data-ttu-id="67bb5-327">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-327">String</span></span>|<span data-ttu-id="67bb5-328">Hersteller des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-328">Manufacturer of the device</span></span>|
|<span data-ttu-id="67bb5-329">imei</span><span class="sxs-lookup"><span data-stu-id="67bb5-329">imei</span></span>|<span data-ttu-id="67bb5-330">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-330">String</span></span>|<span data-ttu-id="67bb5-331">IMEI</span><span class="sxs-lookup"><span data-stu-id="67bb5-331">IMEI</span></span>|
|<span data-ttu-id="67bb5-332">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="67bb5-332">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="67bb5-333">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bb5-333">DateTimeOffset</span></span>|<span data-ttu-id="67bb5-334">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-334">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="67bb5-335">serialNumber</span><span class="sxs-lookup"><span data-stu-id="67bb5-335">serialNumber</span></span>|<span data-ttu-id="67bb5-336">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-336">String</span></span>|<span data-ttu-id="67bb5-337">Seriennummer.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-337">SerialNumber</span></span>|
|<span data-ttu-id="67bb5-338">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="67bb5-338">phoneNumber</span></span>|<span data-ttu-id="67bb5-339">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-339">String</span></span>|<span data-ttu-id="67bb5-340">Telefonnummer des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-340">Phone number of the device</span></span>|
|<span data-ttu-id="67bb5-341">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="67bb5-341">androidSecurityPatchLevel</span></span>|<span data-ttu-id="67bb5-342">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-342">String</span></span>|<span data-ttu-id="67bb5-343">Android-Sicherheitspatchlevel.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-343">Android security patch level</span></span>|
|<span data-ttu-id="67bb5-344">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="67bb5-344">userDisplayName</span></span>|<span data-ttu-id="67bb5-345">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-345">String</span></span>|<span data-ttu-id="67bb5-346">Anzeigename des Benutzers.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-346">User display name</span></span>|
|<span data-ttu-id="67bb5-347">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="67bb5-347">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="67bb5-348">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="67bb5-348">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="67bb5-349">Aktivierte Funktionen des Konfigurations-Manager-Clients.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-349">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="67bb5-350">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="67bb5-350">wiFiMacAddress</span></span>|<span data-ttu-id="67bb5-351">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-351">String</span></span>|<span data-ttu-id="67bb5-352">WLAN-MAC</span><span class="sxs-lookup"><span data-stu-id="67bb5-352">Wi-Fi MAC</span></span>|
|<span data-ttu-id="67bb5-353">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="67bb5-353">deviceHealthAttestationState</span></span>|[<span data-ttu-id="67bb5-354">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="67bb5-354">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="67bb5-355">Status des Integritätsnachweises für Geräte.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-355">The device health attestation state.</span></span>|
|<span data-ttu-id="67bb5-356">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="67bb5-356">subscriberCarrier</span></span>|<span data-ttu-id="67bb5-357">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-357">String</span></span>|<span data-ttu-id="67bb5-358">Netzbetreiber des Abonnenten.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-358">Subscriber Carrier</span></span>|
|<span data-ttu-id="67bb5-359">meid</span><span class="sxs-lookup"><span data-stu-id="67bb5-359">meid</span></span>|<span data-ttu-id="67bb5-360">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-360">String</span></span>|<span data-ttu-id="67bb5-361">MEID</span><span class="sxs-lookup"><span data-stu-id="67bb5-361">MEID</span></span>|
|<span data-ttu-id="67bb5-362">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="67bb5-362">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="67bb5-363">Int64</span><span class="sxs-lookup"><span data-stu-id="67bb5-363">Int64</span></span>|<span data-ttu-id="67bb5-364">Gesamtspeicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-364">Total Storage in Bytes</span></span>|
|<span data-ttu-id="67bb5-365">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="67bb5-365">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="67bb5-366">Int64</span><span class="sxs-lookup"><span data-stu-id="67bb5-366">Int64</span></span>|<span data-ttu-id="67bb5-367">Freier Speicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="67bb5-367">Free Storage in Bytes</span></span>|
|<span data-ttu-id="67bb5-368">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="67bb5-368">managedDeviceName</span></span>|<span data-ttu-id="67bb5-369">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-369">String</span></span>|<span data-ttu-id="67bb5-370">Automatisch generierter Name zur Identifizierung des Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-370">Automatically generated name to identify a device.</span></span> <span data-ttu-id="67bb5-371">Kann mit einem benutzerfreundlichen Namen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="67bb5-371">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="67bb5-372">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="67bb5-372">partnerReportedThreatState</span></span>|[<span data-ttu-id="67bb5-373">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="67bb5-373">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="67bb5-374">Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen.</span><span class="sxs-lookup"><span data-stu-id="67bb5-374">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="67bb5-375">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="67bb5-375">Read Only.</span></span> <span data-ttu-id="67bb5-376">Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="67bb5-376">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="67bb5-377">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="67bb5-377">usersLoggedOn</span></span>|<span data-ttu-id="67bb5-378">[LoggedOnUser](../resources/intune-devices-loggedonuser.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="67bb5-378">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="67bb5-379">Gibt das letzte angemeldete Benutzer eines Geräts</span><span class="sxs-lookup"><span data-stu-id="67bb5-379">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="67bb5-380">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="67bb5-380">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="67bb5-381">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bb5-381">DateTimeOffset</span></span>|<span data-ttu-id="67bb5-382">Meldet den DateTime-Wert die Einstellung PreferMdmOverGroupPolicy festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="67bb5-382">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="67bb5-383">Wenn festgelegt ist, werden die Intune MDM Einstellungen Group Policy Settings außer Kraft setzen, wenn ein Konflikt vorliegt.</span><span class="sxs-lookup"><span data-stu-id="67bb5-383">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="67bb5-384">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="67bb5-384">Read Only.</span></span>|
|<span data-ttu-id="67bb5-385">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="67bb5-385">autopilotEnrolled</span></span>|<span data-ttu-id="67bb5-386">Boolesch</span><span class="sxs-lookup"><span data-stu-id="67bb5-386">Boolean</span></span>|<span data-ttu-id="67bb5-387">Gibt an, ob das verwaltete Geräte über den Auto-Pilot registriert ist.</span><span class="sxs-lookup"><span data-stu-id="67bb5-387">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="67bb5-388">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="67bb5-388">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="67bb5-389">Boolesch</span><span class="sxs-lookup"><span data-stu-id="67bb5-389">Boolean</span></span>|<span data-ttu-id="67bb5-390">Gibt an, ob das Gerät verwalteten iOS Benutzer Genehmigung Registrierung wird.</span><span class="sxs-lookup"><span data-stu-id="67bb5-390">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="67bb5-391">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="67bb5-391">managementCertificateExpirationDate</span></span>|<span data-ttu-id="67bb5-392">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bb5-392">DateTimeOffset</span></span>|<span data-ttu-id="67bb5-393">Ablaufdatum des Zertifikats Berichte Gerät management</span><span class="sxs-lookup"><span data-stu-id="67bb5-393">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="67bb5-394">iccid</span><span class="sxs-lookup"><span data-stu-id="67bb5-394">iccid</span></span>|<span data-ttu-id="67bb5-395">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-395">String</span></span>|<span data-ttu-id="67bb5-396">Chip Karte Bezeichner, ist es eine SIM-Karte eindeutige ID-Nummer.</span><span class="sxs-lookup"><span data-stu-id="67bb5-396">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="67bb5-397">UDID</span><span class="sxs-lookup"><span data-stu-id="67bb5-397">udid</span></span>|<span data-ttu-id="67bb5-398">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-398">String</span></span>|<span data-ttu-id="67bb5-399">Eindeutige Geräte-ID für iOS und Mac OS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="67bb5-399">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="67bb5-400">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="67bb5-400">roleScopeTagIds</span></span>|<span data-ttu-id="67bb5-401">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="67bb5-401">String collection</span></span>|<span data-ttu-id="67bb5-402">Liste der Bereichs-Tag-IDs für diese Instanz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="67bb5-402">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="67bb5-403">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="67bb5-403">windowsActiveMalwareCount</span></span>|<span data-ttu-id="67bb5-404">Int32</span><span class="sxs-lookup"><span data-stu-id="67bb5-404">Int32</span></span>|<span data-ttu-id="67bb5-405">Anzahl von aktiven Malware für dieses Windows-Gerät</span><span class="sxs-lookup"><span data-stu-id="67bb5-405">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="67bb5-406">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="67bb5-406">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="67bb5-407">Int32</span><span class="sxs-lookup"><span data-stu-id="67bb5-407">Int32</span></span>|<span data-ttu-id="67bb5-408">Anzahl der für gewartete Malware für dieses Windows-Gerät</span><span class="sxs-lookup"><span data-stu-id="67bb5-408">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="67bb5-409">notes</span><span class="sxs-lookup"><span data-stu-id="67bb5-409">notes</span></span>|<span data-ttu-id="67bb5-410">String</span><span class="sxs-lookup"><span data-stu-id="67bb5-410">String</span></span>|<span data-ttu-id="67bb5-411">Notes auf dem Gerät durch den IT-Administrator erstellt</span><span class="sxs-lookup"><span data-stu-id="67bb5-411">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="67bb5-412">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="67bb5-412">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="67bb5-413">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="67bb5-413">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="67bb5-414">Konfigurations-Manager-Client Integritätsstatus, gilt nur für Geräte verwaltet von MDM/Configuration Manager-Agent</span><span class="sxs-lookup"><span data-stu-id="67bb5-414">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|

## <a name="relationships"></a><span data-ttu-id="67bb5-415">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="67bb5-415">Relationships</span></span>
|<span data-ttu-id="67bb5-416">Beziehung</span><span class="sxs-lookup"><span data-stu-id="67bb5-416">Relationship</span></span>|<span data-ttu-id="67bb5-417">Typ</span><span class="sxs-lookup"><span data-stu-id="67bb5-417">Type</span></span>|<span data-ttu-id="67bb5-418">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67bb5-418">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67bb5-419">detectedApps</span><span class="sxs-lookup"><span data-stu-id="67bb5-419">detectedApps</span></span>|<span data-ttu-id="67bb5-420">[detectedApp](../resources/intune-devices-detectedapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="67bb5-420">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="67bb5-421">Alle Programme, die derzeit auf dem Gerät installiert.</span><span class="sxs-lookup"><span data-stu-id="67bb5-421">All applications currently installed on the device</span></span>|
|<span data-ttu-id="67bb5-422">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="67bb5-422">deviceCategory</span></span>|[<span data-ttu-id="67bb5-423">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="67bb5-423">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="67bb5-424">Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="67bb5-424">Device category</span></span>|
|<span data-ttu-id="67bb5-425">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="67bb5-425">windowsProtectionState</span></span>|[<span data-ttu-id="67bb5-426">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="67bb5-426">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="67bb5-427">Das Gerät Sicherheitsstatus.</span><span class="sxs-lookup"><span data-stu-id="67bb5-427">The device protection status.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67bb5-428">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="67bb5-428">JSON Representation</span></span>
<span data-ttu-id="67bb5-429">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="67bb5-429">Here is a JSON representation of the resource.</span></span>
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
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "String",
    "totalStorageSpace": 1024,
    "freeStorageSpace": 1024,
    "imei": "String",
    "meid": "String",
    "manufacturer": "String",
    "model": "String",
    "phoneNumber": "String",
    "subscriberCarrier": "String",
    "cellularTechnology": "String",
    "wifiMac": "String",
    "operatingSystemLanguage": "String",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "String",
        "dataToSync": true,
        "dataQuota": 1024,
        "dataUsed": 1024
      }
    ],
    "tpmSpecificationVersion": "String",
    "operatingSystemEdition": "String",
    "deviceFullQualifiedDomainName": "String",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
    "deviceGuardVirtualizationBasedSecurityState": "String",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
  },
  "ownerType": "String",
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
  "managementState": "String",
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "chassisType": "String",
  "operatingSystem": "String",
  "deviceType": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "lostModeState": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureActiveDirectoryDeviceId": "String",
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
  "partnerReportedThreatState": "String",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "String",
      "lastLogOnDateTime": "String (timestamp)"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "String (timestamp)",
  "iccid": "String",
  "udid": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "windowsActiveMalwareCount": 1024,
  "windowsRemediatedMalwareCount": 1024,
  "notes": "String",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "String",
    "errorCode": 1024,
    "lastSyncDateTime": "String (timestamp)"
  }
}
```





