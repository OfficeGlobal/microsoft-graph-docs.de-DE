---
title: managedDevice-Ressourcentyp
description: Über Intune verwaltete oder vorab registrierte Geräte
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d08b0559065b3977978621004b290a87879cdc70
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869216"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="ca304-103">managedDevice-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ca304-103">managedDevice resource type</span></span>

> <span data-ttu-id="ca304-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ca304-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca304-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ca304-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca304-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ca304-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca304-107">Über Intune verwaltete oder vorab registrierte Geräte</span><span class="sxs-lookup"><span data-stu-id="ca304-107">Devices that are managed or pre-enrolled through Intune</span></span>
## <a name="methods"></a><span data-ttu-id="ca304-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="ca304-108">Methods</span></span>
|<span data-ttu-id="ca304-109">Methode</span><span class="sxs-lookup"><span data-stu-id="ca304-109">Method</span></span>|<span data-ttu-id="ca304-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ca304-110">Return Type</span></span>|<span data-ttu-id="ca304-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ca304-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ca304-112">managedDevice abrufen</span><span class="sxs-lookup"><span data-stu-id="ca304-112">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="ca304-113">managedDevice</span><span class="sxs-lookup"><span data-stu-id="ca304-113">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="ca304-114">Lesen von Eigenschaften und Beziehungen des [managedDevice](../resources/intune-devices-manageddevice.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ca304-114">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="ca304-115">managedDevice aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ca304-115">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="ca304-116">managedDevice</span><span class="sxs-lookup"><span data-stu-id="ca304-116">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="ca304-117">Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune-devices-manageddevice.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ca304-117">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="ca304-118">ExecuteAction-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-118">executeAction action</span></span>](../api/intune-devices-manageddevice-executeaction.md)|[<span data-ttu-id="ca304-119">bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="ca304-119">bulkManagedDeviceActionResult</span></span>](../resources/intune-devices-bulkmanageddeviceactionresult.md)|<span data-ttu-id="ca304-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ca304-120">Not yet documented</span></span>|
|[<span data-ttu-id="ca304-121">EnableLostMode Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-121">enableLostMode action</span></span>](../api/intune-devices-manageddevice-enablelostmode.md)|<span data-ttu-id="ca304-122">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-122">None</span></span>|<span data-ttu-id="ca304-123">Verloren-Modus aktivieren</span><span class="sxs-lookup"><span data-stu-id="ca304-123">Enable lost mode</span></span>|
|[<span data-ttu-id="ca304-124">PlayLostModeSound Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-124">playLostModeSound action</span></span>](../api/intune-devices-manageddevice-playlostmodesound.md)|<span data-ttu-id="ca304-125">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-125">None</span></span>|<span data-ttu-id="ca304-126">Remotesperre</span><span class="sxs-lookup"><span data-stu-id="ca304-126">Remote lock</span></span>|
|[<span data-ttu-id="ca304-127">SetDeviceName Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-127">setDeviceName action</span></span>](../api/intune-devices-manageddevice-setdevicename.md)|<span data-ttu-id="ca304-128">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-128">None</span></span>|<span data-ttu-id="ca304-129">Festlegen Sie Name des Aufnahmegeräts des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-129">Set device name of the device.</span></span>|
|[<span data-ttu-id="ca304-130">retire-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-130">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="ca304-131">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-131">None</span></span>|<span data-ttu-id="ca304-132">Zurückziehen eines Geräts</span><span class="sxs-lookup"><span data-stu-id="ca304-132">Retire a device</span></span>|
|[<span data-ttu-id="ca304-133">wipe-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-133">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="ca304-134">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-134">None</span></span>|<span data-ttu-id="ca304-135">Zurücksetzen eines Geräts</span><span class="sxs-lookup"><span data-stu-id="ca304-135">Wipe a device</span></span>|
|[<span data-ttu-id="ca304-136">resetPasscode-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-136">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="ca304-137">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-137">None</span></span>|<span data-ttu-id="ca304-138">Kennung zurücksetzen</span><span class="sxs-lookup"><span data-stu-id="ca304-138">Reset passcode</span></span>|
|[<span data-ttu-id="ca304-139">remoteLock-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-139">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="ca304-140">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-140">None</span></span>|<span data-ttu-id="ca304-141">Remotesperre</span><span class="sxs-lookup"><span data-stu-id="ca304-141">Remote lock</span></span>|
|[<span data-ttu-id="ca304-142">requestRemoteAssistance-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-142">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="ca304-143">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-143">None</span></span>|<span data-ttu-id="ca304-144">Remoteunterstützung anfordern</span><span class="sxs-lookup"><span data-stu-id="ca304-144">Request remote assistance</span></span>|
|[<span data-ttu-id="ca304-145">disableLostMode-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-145">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="ca304-146">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-146">None</span></span>|<span data-ttu-id="ca304-147">Modus für verlorene Geräte deaktivieren</span><span class="sxs-lookup"><span data-stu-id="ca304-147">Disable lost mode</span></span>|
|[<span data-ttu-id="ca304-148">locateDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-148">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="ca304-149">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-149">None</span></span>|<span data-ttu-id="ca304-150">Suchen eines Geräts</span><span class="sxs-lookup"><span data-stu-id="ca304-150">Locate a device</span></span>|
|[<span data-ttu-id="ca304-151">bypassActivationLock-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-151">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="ca304-152">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-152">None</span></span>|<span data-ttu-id="ca304-153">Aktivierungssperre umgehen</span><span class="sxs-lookup"><span data-stu-id="ca304-153">Bypass activation lock</span></span>|
|[<span data-ttu-id="ca304-154">rebootNow-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-154">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="ca304-155">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-155">None</span></span>|<span data-ttu-id="ca304-156">Gerät neu starten</span><span class="sxs-lookup"><span data-stu-id="ca304-156">Reboot device</span></span>|
|[<span data-ttu-id="ca304-157">shutDown-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-157">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="ca304-158">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-158">None</span></span>|<span data-ttu-id="ca304-159">Gerät abschalten</span><span class="sxs-lookup"><span data-stu-id="ca304-159">Shut down device</span></span>|
|[<span data-ttu-id="ca304-160">recoverPasscode-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-160">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="ca304-161">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-161">None</span></span>|<span data-ttu-id="ca304-162">Kennung wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="ca304-162">Recover passcode</span></span>|
|[<span data-ttu-id="ca304-163">cleanWindowsDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-163">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="ca304-164">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-164">None</span></span>|<span data-ttu-id="ca304-165">Windows-Gerät bereinigen</span><span class="sxs-lookup"><span data-stu-id="ca304-165">Clean Windows device</span></span>|
|[<span data-ttu-id="ca304-166">logoutSharedAppleDeviceActiveUser-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-166">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="ca304-167">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-167">None</span></span>|<span data-ttu-id="ca304-168">Aktiven Benutzer von freigegebenem Apple-Gerät abmelden</span><span class="sxs-lookup"><span data-stu-id="ca304-168">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="ca304-169">deleteUserFromSharedAppleDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-169">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="ca304-170">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-170">None</span></span>|<span data-ttu-id="ca304-171">Benutzer von freigegebenem Apple-Gerät löschen</span><span class="sxs-lookup"><span data-stu-id="ca304-171">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="ca304-172">syncDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-172">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="ca304-173">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-173">None</span></span>|<span data-ttu-id="ca304-174">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="ca304-174">Not yet documented</span></span>|
|[<span data-ttu-id="ca304-175">windowsDefenderScan-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-175">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="ca304-176">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-176">None</span></span>|<span data-ttu-id="ca304-177">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="ca304-177">Not yet documented</span></span>|
|[<span data-ttu-id="ca304-178">windowsDefenderUpdateSignatures-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-178">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="ca304-179">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-179">None</span></span>|<span data-ttu-id="ca304-180">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="ca304-180">Not yet documented</span></span>|
|[<span data-ttu-id="ca304-181">updateWindowsDeviceAccount-Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-181">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="ca304-182">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-182">None</span></span>|<span data-ttu-id="ca304-183">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ca304-183">Not yet documented</span></span>|
|[<span data-ttu-id="ca304-184">RevokeAppleVppLicenses Aktion</span><span class="sxs-lookup"><span data-stu-id="ca304-184">revokeAppleVppLicenses action</span></span>](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|<span data-ttu-id="ca304-185">Keine</span><span class="sxs-lookup"><span data-stu-id="ca304-185">None</span></span>|<span data-ttu-id="ca304-186">Alle Apple Vpp Lizenzen für ein Gerät widerrufen</span><span class="sxs-lookup"><span data-stu-id="ca304-186">Revoke all Apple Vpp licenses for a device</span></span>|

## <a name="properties"></a><span data-ttu-id="ca304-187">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ca304-187">Properties</span></span>
|<span data-ttu-id="ca304-188">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ca304-188">Property</span></span>|<span data-ttu-id="ca304-189">Typ</span><span class="sxs-lookup"><span data-stu-id="ca304-189">Type</span></span>|<span data-ttu-id="ca304-190">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ca304-190">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca304-191">id</span><span class="sxs-lookup"><span data-stu-id="ca304-191">id</span></span>|<span data-ttu-id="ca304-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-192">String</span></span>|<span data-ttu-id="ca304-193">Eindeutiger Bezeichner für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="ca304-193">Unique Identifier for the device</span></span>|
|<span data-ttu-id="ca304-194">userId</span><span class="sxs-lookup"><span data-stu-id="ca304-194">userId</span></span>|<span data-ttu-id="ca304-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-195">String</span></span>|<span data-ttu-id="ca304-196">Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="ca304-196">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="ca304-197">deviceName</span><span class="sxs-lookup"><span data-stu-id="ca304-197">deviceName</span></span>|<span data-ttu-id="ca304-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-198">String</span></span>|<span data-ttu-id="ca304-199">Name des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="ca304-199">Name of the device</span></span>|
|<span data-ttu-id="ca304-200">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="ca304-200">hardwareInformation</span></span>|[<span data-ttu-id="ca304-201">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="ca304-201">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="ca304-202">Die Hardward Details für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="ca304-202">The hardward details for the device.</span></span>  <span data-ttu-id="ca304-203">Enthält Informationen, wie Speicherplatz, Hersteller, Seriennummer.</span><span class="sxs-lookup"><span data-stu-id="ca304-203">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="ca304-204">Besitzertyp</span><span class="sxs-lookup"><span data-stu-id="ca304-204">ownerType</span></span>|[<span data-ttu-id="ca304-205">Besitzertyp</span><span class="sxs-lookup"><span data-stu-id="ca304-205">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="ca304-206">Besitz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-206">Ownership of the device.</span></span> <span data-ttu-id="ca304-207">'Company' oder 'Privat' kann sein.</span><span class="sxs-lookup"><span data-stu-id="ca304-207">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="ca304-208">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="ca304-208">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ca304-209">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ca304-209">managedDeviceOwnerType</span></span>|[<span data-ttu-id="ca304-210">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="ca304-210">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="ca304-211">Besitz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-211">Ownership of the device.</span></span> <span data-ttu-id="ca304-212">'Company' oder 'Privat' kann sein.</span><span class="sxs-lookup"><span data-stu-id="ca304-212">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="ca304-213">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="ca304-213">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="ca304-214">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="ca304-214">deviceActionResults</span></span>|<span data-ttu-id="ca304-215">Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ca304-215">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="ca304-216">Liste von Objekten des Typs „ComplexType deviceActionResult“.
</span><span class="sxs-lookup"><span data-stu-id="ca304-216">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="ca304-217">managementState</span><span class="sxs-lookup"><span data-stu-id="ca304-217">managementState</span></span>|[<span data-ttu-id="ca304-218">managementState</span><span class="sxs-lookup"><span data-stu-id="ca304-218">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="ca304-219">Verwaltungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-219">Management state of the device.</span></span> <span data-ttu-id="ca304-220">Mögliche Werte sind: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled` und `discovered`.</span><span class="sxs-lookup"><span data-stu-id="ca304-220">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="ca304-221">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="ca304-221">enrolledDateTime</span></span>|<span data-ttu-id="ca304-222">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca304-222">DateTimeOffset</span></span>|<span data-ttu-id="ca304-223">Datum und Uhrzeit der Geräteregistrierung.
</span><span class="sxs-lookup"><span data-stu-id="ca304-223">Enrollment time of the device.</span></span>|
|<span data-ttu-id="ca304-224">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ca304-224">lastSyncDateTime</span></span>|<span data-ttu-id="ca304-225">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca304-225">DateTimeOffset</span></span>|<span data-ttu-id="ca304-226">Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
</span><span class="sxs-lookup"><span data-stu-id="ca304-226">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="ca304-227">chassisType</span><span class="sxs-lookup"><span data-stu-id="ca304-227">chassisType</span></span>|[<span data-ttu-id="ca304-228">chassisType</span><span class="sxs-lookup"><span data-stu-id="ca304-228">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="ca304-229">Chassistyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-229">Chassis type of the device.</span></span> <span data-ttu-id="ca304-230">Mögliche Werte: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="ca304-230">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="ca304-231">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="ca304-231">operatingSystem</span></span>|<span data-ttu-id="ca304-232">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-232">String</span></span>|<span data-ttu-id="ca304-233">Betriebssystem des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-233">Operating system of the device.</span></span> <span data-ttu-id="ca304-234">Windows, iOS usw.</span><span class="sxs-lookup"><span data-stu-id="ca304-234">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="ca304-235">deviceType</span><span class="sxs-lookup"><span data-stu-id="ca304-235">deviceType</span></span>|[<span data-ttu-id="ca304-236">deviceType</span><span class="sxs-lookup"><span data-stu-id="ca304-236">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="ca304-237">Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-237">Platform of the device.</span></span> <span data-ttu-id="ca304-238">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ca304-238">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="ca304-239">complianceState</span><span class="sxs-lookup"><span data-stu-id="ca304-239">complianceState</span></span>|[<span data-ttu-id="ca304-240">complianceState</span><span class="sxs-lookup"><span data-stu-id="ca304-240">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="ca304-241">Konformitätsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-241">Compliance state of the device.</span></span> <span data-ttu-id="ca304-242">Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.</span><span class="sxs-lookup"><span data-stu-id="ca304-242">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="ca304-243">jailBroken</span><span class="sxs-lookup"><span data-stu-id="ca304-243">jailBroken</span></span>|<span data-ttu-id="ca304-244">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-244">String</span></span>|<span data-ttu-id="ca304-245">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="ca304-245">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="ca304-246">managementAgent</span><span class="sxs-lookup"><span data-stu-id="ca304-246">managementAgent</span></span>|[<span data-ttu-id="ca304-247">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="ca304-247">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="ca304-248">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-248">Management channel of the device.</span></span> <span data-ttu-id="ca304-249">Intune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="ca304-249">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="ca304-250">osVersion</span><span class="sxs-lookup"><span data-stu-id="ca304-250">osVersion</span></span>|<span data-ttu-id="ca304-251">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-251">String</span></span>|<span data-ttu-id="ca304-252">Auf dem Gerät installierte Betriebssystemversion.
</span><span class="sxs-lookup"><span data-stu-id="ca304-252">Operating system version of the device.</span></span>|
|<span data-ttu-id="ca304-253">easActivated</span><span class="sxs-lookup"><span data-stu-id="ca304-253">easActivated</span></span>|<span data-ttu-id="ca304-254">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ca304-254">Boolean</span></span>|<span data-ttu-id="ca304-255">Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="ca304-255">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="ca304-256">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="ca304-256">easDeviceId</span></span>|<span data-ttu-id="ca304-257">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-257">String</span></span>|<span data-ttu-id="ca304-258">Exchange ActiveSync-ID des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="ca304-258">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="ca304-259">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="ca304-259">easActivationDateTime</span></span>|<span data-ttu-id="ca304-260">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca304-260">DateTimeOffset</span></span>|<span data-ttu-id="ca304-261">Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="ca304-261">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="ca304-262">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="ca304-262">aadRegistered</span></span>|<span data-ttu-id="ca304-263">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ca304-263">Boolean</span></span>|<span data-ttu-id="ca304-264">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="ca304-264">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="ca304-265">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="ca304-265">azureADRegistered</span></span>|<span data-ttu-id="ca304-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca304-266">Boolean</span></span>|<span data-ttu-id="ca304-267">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="ca304-267">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="ca304-268">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ca304-268">deviceEnrollmentType</span></span>|[<span data-ttu-id="ca304-269">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ca304-269">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="ca304-270">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-270">Enrollment type of the device.</span></span> <span data-ttu-id="ca304-271">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="ca304-271">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="ca304-272">lostModeState</span><span class="sxs-lookup"><span data-stu-id="ca304-272">lostModeState</span></span>|[<span data-ttu-id="ca304-273">lostModeState</span><span class="sxs-lookup"><span data-stu-id="ca304-273">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="ca304-274">Gibt an, ob verloren-Modus aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="ca304-274">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="ca304-275">Mögliche Werte sind: `disabled` und `enabled`.</span><span class="sxs-lookup"><span data-stu-id="ca304-275">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="ca304-276">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="ca304-276">activationLockBypassCode</span></span>|<span data-ttu-id="ca304-277">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-277">String</span></span>|<span data-ttu-id="ca304-278">Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht</span><span class="sxs-lookup"><span data-stu-id="ca304-278">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="ca304-279">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ca304-279">emailAddress</span></span>|<span data-ttu-id="ca304-280">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-280">String</span></span>|<span data-ttu-id="ca304-281">E-Mail-Adressen des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="ca304-281">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="ca304-282">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="ca304-282">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="ca304-283">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-283">String</span></span>|<span data-ttu-id="ca304-284">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-284">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="ca304-285">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ca304-285">Read only.</span></span>|
|<span data-ttu-id="ca304-286">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="ca304-286">azureADDeviceId</span></span>|<span data-ttu-id="ca304-287">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-287">String</span></span>|<span data-ttu-id="ca304-288">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-288">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="ca304-289">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ca304-289">Read only.</span></span>|
|<span data-ttu-id="ca304-290">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ca304-290">deviceRegistrationState</span></span>|[<span data-ttu-id="ca304-291">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="ca304-291">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="ca304-292">Registrierungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-292">Device registration state.</span></span> <span data-ttu-id="ca304-293">Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ca304-293">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="ca304-294">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="ca304-294">deviceCategoryDisplayName</span></span>|<span data-ttu-id="ca304-295">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-295">String</span></span>|<span data-ttu-id="ca304-296">Anzeigename der Gerätekategorie.
</span><span class="sxs-lookup"><span data-stu-id="ca304-296">Device category display name</span></span>|
|<span data-ttu-id="ca304-297">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ca304-297">isSupervised</span></span>|<span data-ttu-id="ca304-298">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ca304-298">Boolean</span></span>|<span data-ttu-id="ca304-299">Überwachungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="ca304-299">Device supervised status</span></span>|
|<span data-ttu-id="ca304-300">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ca304-300">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="ca304-301">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca304-301">DateTimeOffset</span></span>|<span data-ttu-id="ca304-302">Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange</span><span class="sxs-lookup"><span data-stu-id="ca304-302">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="ca304-303">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ca304-303">exchangeAccessState</span></span>|[<span data-ttu-id="ca304-304">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="ca304-304">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="ca304-305">Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca304-305">The Access State of the device in Exchange.</span></span> <span data-ttu-id="ca304-306">Mögliche Werte sind: `none`, `unknown`, `allowed`, `blocked` und `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="ca304-306">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="ca304-307">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="ca304-307">exchangeAccessStateReason</span></span>|[<span data-ttu-id="ca304-308">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="ca304-308">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="ca304-309">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca304-309">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="ca304-310">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="ca304-310">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="ca304-311">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="ca304-311">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="ca304-312">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-312">String</span></span>|<span data-ttu-id="ca304-313">URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
</span><span class="sxs-lookup"><span data-stu-id="ca304-313">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="ca304-314">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ca304-314">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="ca304-315">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-315">String</span></span>|<span data-ttu-id="ca304-316">Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
</span><span class="sxs-lookup"><span data-stu-id="ca304-316">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="ca304-317">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ca304-317">isEncrypted</span></span>|<span data-ttu-id="ca304-318">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ca304-318">Boolean</span></span>|<span data-ttu-id="ca304-319">Verschlüsselungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="ca304-319">Device encryption status</span></span>|
|<span data-ttu-id="ca304-320">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ca304-320">userPrincipalName</span></span>|<span data-ttu-id="ca304-321">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-321">String</span></span>|<span data-ttu-id="ca304-322">Benutzerprinzipalname für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="ca304-322">Device user principal name</span></span>|
|<span data-ttu-id="ca304-323">model</span><span class="sxs-lookup"><span data-stu-id="ca304-323">model</span></span>|<span data-ttu-id="ca304-324">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-324">String</span></span>|<span data-ttu-id="ca304-325">Modell des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="ca304-325">Model of the device</span></span>|
|<span data-ttu-id="ca304-326">manufacturer</span><span class="sxs-lookup"><span data-stu-id="ca304-326">manufacturer</span></span>|<span data-ttu-id="ca304-327">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-327">String</span></span>|<span data-ttu-id="ca304-328">Hersteller des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="ca304-328">Manufacturer of the device</span></span>|
|<span data-ttu-id="ca304-329">imei</span><span class="sxs-lookup"><span data-stu-id="ca304-329">imei</span></span>|<span data-ttu-id="ca304-330">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-330">String</span></span>|<span data-ttu-id="ca304-331">IMEI</span><span class="sxs-lookup"><span data-stu-id="ca304-331">IMEI</span></span>|
|<span data-ttu-id="ca304-332">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ca304-332">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ca304-333">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca304-333">DateTimeOffset</span></span>|<span data-ttu-id="ca304-334">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität.
</span><span class="sxs-lookup"><span data-stu-id="ca304-334">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="ca304-335">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ca304-335">serialNumber</span></span>|<span data-ttu-id="ca304-336">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-336">String</span></span>|<span data-ttu-id="ca304-337">Seriennummer.
</span><span class="sxs-lookup"><span data-stu-id="ca304-337">SerialNumber</span></span>|
|<span data-ttu-id="ca304-338">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ca304-338">phoneNumber</span></span>|<span data-ttu-id="ca304-339">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-339">String</span></span>|<span data-ttu-id="ca304-340">Telefonnummer des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="ca304-340">Phone number of the device</span></span>|
|<span data-ttu-id="ca304-341">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="ca304-341">androidSecurityPatchLevel</span></span>|<span data-ttu-id="ca304-342">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-342">String</span></span>|<span data-ttu-id="ca304-343">Android-Sicherheitspatchlevel.
</span><span class="sxs-lookup"><span data-stu-id="ca304-343">Android security patch level</span></span>|
|<span data-ttu-id="ca304-344">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ca304-344">userDisplayName</span></span>|<span data-ttu-id="ca304-345">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-345">String</span></span>|<span data-ttu-id="ca304-346">Anzeigename des Benutzers.
</span><span class="sxs-lookup"><span data-stu-id="ca304-346">User display name</span></span>|
|<span data-ttu-id="ca304-347">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ca304-347">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="ca304-348">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ca304-348">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="ca304-349">Aktivierte Funktionen des Konfigurations-Manager-Clients.
</span><span class="sxs-lookup"><span data-stu-id="ca304-349">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="ca304-350">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="ca304-350">wiFiMacAddress</span></span>|<span data-ttu-id="ca304-351">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-351">String</span></span>|<span data-ttu-id="ca304-352">WLAN-MAC</span><span class="sxs-lookup"><span data-stu-id="ca304-352">Wi-Fi MAC</span></span>|
|<span data-ttu-id="ca304-353">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ca304-353">deviceHealthAttestationState</span></span>|[<span data-ttu-id="ca304-354">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="ca304-354">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="ca304-355">Status des Integritätsnachweises für Geräte.
</span><span class="sxs-lookup"><span data-stu-id="ca304-355">The device health attestation state.</span></span>|
|<span data-ttu-id="ca304-356">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="ca304-356">subscriberCarrier</span></span>|<span data-ttu-id="ca304-357">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-357">String</span></span>|<span data-ttu-id="ca304-358">Netzbetreiber des Abonnenten.
</span><span class="sxs-lookup"><span data-stu-id="ca304-358">Subscriber Carrier</span></span>|
|<span data-ttu-id="ca304-359">meid</span><span class="sxs-lookup"><span data-stu-id="ca304-359">meid</span></span>|<span data-ttu-id="ca304-360">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-360">String</span></span>|<span data-ttu-id="ca304-361">MEID</span><span class="sxs-lookup"><span data-stu-id="ca304-361">MEID</span></span>|
|<span data-ttu-id="ca304-362">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ca304-362">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="ca304-363">Int64</span><span class="sxs-lookup"><span data-stu-id="ca304-363">Int64</span></span>|<span data-ttu-id="ca304-364">Gesamtspeicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="ca304-364">Total Storage in Bytes</span></span>|
|<span data-ttu-id="ca304-365">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="ca304-365">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="ca304-366">Int64</span><span class="sxs-lookup"><span data-stu-id="ca304-366">Int64</span></span>|<span data-ttu-id="ca304-367">Freier Speicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="ca304-367">Free Storage in Bytes</span></span>|
|<span data-ttu-id="ca304-368">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="ca304-368">managedDeviceName</span></span>|<span data-ttu-id="ca304-369">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-369">String</span></span>|<span data-ttu-id="ca304-370">Automatisch generierter Name zur Identifizierung des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-370">Automatically generated name to identify a device.</span></span> <span data-ttu-id="ca304-371">Kann mit einem benutzerfreundlichen Namen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="ca304-371">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="ca304-372">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="ca304-372">partnerReportedThreatState</span></span>|[<span data-ttu-id="ca304-373">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="ca304-373">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="ca304-374">Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen.</span><span class="sxs-lookup"><span data-stu-id="ca304-374">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="ca304-375">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ca304-375">Read Only.</span></span> <span data-ttu-id="ca304-376">Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="ca304-376">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="ca304-377">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="ca304-377">usersLoggedOn</span></span>|<span data-ttu-id="ca304-378">[LoggedOnUser](../resources/intune-devices-loggedonuser.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ca304-378">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="ca304-379">Gibt das letzte angemeldete Benutzer eines Geräts</span><span class="sxs-lookup"><span data-stu-id="ca304-379">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="ca304-380">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca304-380">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="ca304-381">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca304-381">DateTimeOffset</span></span>|<span data-ttu-id="ca304-382">Meldet den DateTime-Wert die Einstellung PreferMdmOverGroupPolicy festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="ca304-382">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="ca304-383">Wenn festgelegt ist, werden die Intune MDM Einstellungen Group Policy Settings außer Kraft setzen, wenn ein Konflikt vorliegt.</span><span class="sxs-lookup"><span data-stu-id="ca304-383">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="ca304-384">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ca304-384">Read Only.</span></span>|
|<span data-ttu-id="ca304-385">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="ca304-385">autopilotEnrolled</span></span>|<span data-ttu-id="ca304-386">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ca304-386">Boolean</span></span>|<span data-ttu-id="ca304-387">Gibt an, ob das verwaltete Geräte über den Auto-Pilot registriert ist.</span><span class="sxs-lookup"><span data-stu-id="ca304-387">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="ca304-388">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="ca304-388">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="ca304-389">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ca304-389">Boolean</span></span>|<span data-ttu-id="ca304-390">Gibt an, ob das Gerät verwalteten iOS Benutzer Genehmigung Registrierung wird.</span><span class="sxs-lookup"><span data-stu-id="ca304-390">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="ca304-391">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="ca304-391">managementCertificateExpirationDate</span></span>|<span data-ttu-id="ca304-392">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca304-392">DateTimeOffset</span></span>|<span data-ttu-id="ca304-393">Ablaufdatum des Zertifikats Berichte Gerät management</span><span class="sxs-lookup"><span data-stu-id="ca304-393">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="ca304-394">iccid</span><span class="sxs-lookup"><span data-stu-id="ca304-394">iccid</span></span>|<span data-ttu-id="ca304-395">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-395">String</span></span>|<span data-ttu-id="ca304-396">Chip Karte Bezeichner, ist es eine SIM-Karte eindeutige ID-Nummer.</span><span class="sxs-lookup"><span data-stu-id="ca304-396">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="ca304-397">UDID</span><span class="sxs-lookup"><span data-stu-id="ca304-397">udid</span></span>|<span data-ttu-id="ca304-398">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-398">String</span></span>|<span data-ttu-id="ca304-399">Eindeutige Geräte-ID für iOS und Mac OS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="ca304-399">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="ca304-400">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca304-400">roleScopeTagIds</span></span>|<span data-ttu-id="ca304-401">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="ca304-401">String collection</span></span>|<span data-ttu-id="ca304-402">Liste der Bereichs-Tag-IDs für diese Instanz des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ca304-402">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="ca304-403">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="ca304-403">windowsActiveMalwareCount</span></span>|<span data-ttu-id="ca304-404">Int32</span><span class="sxs-lookup"><span data-stu-id="ca304-404">Int32</span></span>|<span data-ttu-id="ca304-405">Anzahl von aktiven Malware für dieses Windows-Gerät</span><span class="sxs-lookup"><span data-stu-id="ca304-405">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="ca304-406">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="ca304-406">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="ca304-407">Int32</span><span class="sxs-lookup"><span data-stu-id="ca304-407">Int32</span></span>|<span data-ttu-id="ca304-408">Anzahl der für gewartete Malware für dieses Windows-Gerät</span><span class="sxs-lookup"><span data-stu-id="ca304-408">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="ca304-409">notes</span><span class="sxs-lookup"><span data-stu-id="ca304-409">notes</span></span>|<span data-ttu-id="ca304-410">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca304-410">String</span></span>|<span data-ttu-id="ca304-411">Notes auf dem Gerät durch den IT-Administrator erstellt</span><span class="sxs-lookup"><span data-stu-id="ca304-411">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="ca304-412">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="ca304-412">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="ca304-413">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="ca304-413">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="ca304-414">Konfigurations-Manager-Client Integritätsstatus, gilt nur für Geräte verwaltet von MDM/Configuration Manager-Agent</span><span class="sxs-lookup"><span data-stu-id="ca304-414">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca304-415">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ca304-415">Relationships</span></span>
|<span data-ttu-id="ca304-416">Beziehung</span><span class="sxs-lookup"><span data-stu-id="ca304-416">Relationship</span></span>|<span data-ttu-id="ca304-417">Typ</span><span class="sxs-lookup"><span data-stu-id="ca304-417">Type</span></span>|<span data-ttu-id="ca304-418">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ca304-418">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca304-419">detectedApps</span><span class="sxs-lookup"><span data-stu-id="ca304-419">detectedApps</span></span>|<span data-ttu-id="ca304-420">[detectedApp](../resources/intune-devices-detectedapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ca304-420">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="ca304-421">Alle Programme, die derzeit auf dem Gerät installiert.</span><span class="sxs-lookup"><span data-stu-id="ca304-421">All applications currently installed on the device</span></span>|
|<span data-ttu-id="ca304-422">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="ca304-422">deviceCategory</span></span>|[<span data-ttu-id="ca304-423">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="ca304-423">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="ca304-424">Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="ca304-424">Device category</span></span>|
|<span data-ttu-id="ca304-425">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="ca304-425">windowsProtectionState</span></span>|[<span data-ttu-id="ca304-426">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="ca304-426">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="ca304-427">Das Gerät Sicherheitsstatus.</span><span class="sxs-lookup"><span data-stu-id="ca304-427">The device protection status.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca304-428">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ca304-428">JSON Representation</span></span>
<span data-ttu-id="ca304-429">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ca304-429">Here is a JSON representation of the resource.</span></span>
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





