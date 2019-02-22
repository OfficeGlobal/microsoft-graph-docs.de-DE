---
title: managedDevice-Ressourcentyp
description: Über Intune verwaltete oder vorab registrierte Geräte
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 274c0000dbdae3b886241d628f4d03e944b61d5d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162510"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="13384-103">managedDevice-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="13384-103">managedDevice resource type</span></span>

> <span data-ttu-id="13384-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13384-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13384-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="13384-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13384-106">Über Intune verwaltete oder vorab registrierte Geräte</span><span class="sxs-lookup"><span data-stu-id="13384-106">Devices that are managed or pre-enrolled through Intune</span></span>

## <a name="methods"></a><span data-ttu-id="13384-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="13384-107">Methods</span></span>
|<span data-ttu-id="13384-108">Methode</span><span class="sxs-lookup"><span data-stu-id="13384-108">Method</span></span>|<span data-ttu-id="13384-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="13384-109">Return Type</span></span>|<span data-ttu-id="13384-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13384-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13384-111">managedDevice abrufen</span><span class="sxs-lookup"><span data-stu-id="13384-111">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="13384-112">managedDevice</span><span class="sxs-lookup"><span data-stu-id="13384-112">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="13384-113">Lesen von Eigenschaften und Beziehungen des [managedDevice](../resources/intune-devices-manageddevice.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="13384-113">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="13384-114">managedDevice aktualisieren</span><span class="sxs-lookup"><span data-stu-id="13384-114">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="13384-115">managedDevice</span><span class="sxs-lookup"><span data-stu-id="13384-115">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="13384-116">Aktualisieren der Eigenschaften eines [managedDeviceOverview](../resources/intune-devices-manageddevice.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="13384-116">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="13384-117">executeAction-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-117">executeAction action</span></span>](../api/intune-devices-manageddevice-executeaction.md)|[<span data-ttu-id="13384-118">bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="13384-118">bulkManagedDeviceActionResult</span></span>](../resources/intune-devices-bulkmanageddeviceactionresult.md)|<span data-ttu-id="13384-119">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="13384-119">Not yet documented</span></span>|
|[<span data-ttu-id="13384-120">enableLostMode-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-120">enableLostMode action</span></span>](../api/intune-devices-manageddevice-enablelostmode.md)|<span data-ttu-id="13384-121">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-121">None</span></span>|<span data-ttu-id="13384-122">Modus "verloren" aktivieren</span><span class="sxs-lookup"><span data-stu-id="13384-122">Enable lost mode</span></span>|
|[<span data-ttu-id="13384-123">playLostModeSound-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-123">playLostModeSound action</span></span>](../api/intune-devices-manageddevice-playlostmodesound.md)|<span data-ttu-id="13384-124">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-124">None</span></span>|<span data-ttu-id="13384-125">Remotesperre</span><span class="sxs-lookup"><span data-stu-id="13384-125">Remote lock</span></span>|
|[<span data-ttu-id="13384-126">setDeviceName-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-126">setDeviceName action</span></span>](../api/intune-devices-manageddevice-setdevicename.md)|<span data-ttu-id="13384-127">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-127">None</span></span>|<span data-ttu-id="13384-128">Legen Sie den Gerätenamen des Geräts fest.</span><span class="sxs-lookup"><span data-stu-id="13384-128">Set device name of the device.</span></span>|
|[<span data-ttu-id="13384-129">retire-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-129">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="13384-130">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-130">None</span></span>|<span data-ttu-id="13384-131">Zurückziehen eines Geräts</span><span class="sxs-lookup"><span data-stu-id="13384-131">Retire a device</span></span>|
|[<span data-ttu-id="13384-132">wipe-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-132">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="13384-133">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-133">None</span></span>|<span data-ttu-id="13384-134">Zurücksetzen eines Geräts</span><span class="sxs-lookup"><span data-stu-id="13384-134">Wipe a device</span></span>|
|[<span data-ttu-id="13384-135">resetPasscode-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-135">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="13384-136">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-136">None</span></span>|<span data-ttu-id="13384-137">Kennung zurücksetzen</span><span class="sxs-lookup"><span data-stu-id="13384-137">Reset passcode</span></span>|
|[<span data-ttu-id="13384-138">remoteLock-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-138">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="13384-139">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-139">None</span></span>|<span data-ttu-id="13384-140">Remotesperre</span><span class="sxs-lookup"><span data-stu-id="13384-140">Remote lock</span></span>|
|[<span data-ttu-id="13384-141">requestRemoteAssistance-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-141">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="13384-142">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-142">None</span></span>|<span data-ttu-id="13384-143">Remoteunterstützung anfordern</span><span class="sxs-lookup"><span data-stu-id="13384-143">Request remote assistance</span></span>|
|[<span data-ttu-id="13384-144">disableLostMode-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-144">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="13384-145">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-145">None</span></span>|<span data-ttu-id="13384-146">Modus für verlorene Geräte deaktivieren</span><span class="sxs-lookup"><span data-stu-id="13384-146">Disable lost mode</span></span>|
|[<span data-ttu-id="13384-147">locateDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-147">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="13384-148">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-148">None</span></span>|<span data-ttu-id="13384-149">Suchen eines Geräts</span><span class="sxs-lookup"><span data-stu-id="13384-149">Locate a device</span></span>|
|[<span data-ttu-id="13384-150">bypassActivationLock-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-150">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="13384-151">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-151">None</span></span>|<span data-ttu-id="13384-152">Aktivierungssperre umgehen</span><span class="sxs-lookup"><span data-stu-id="13384-152">Bypass activation lock</span></span>|
|[<span data-ttu-id="13384-153">rebootNow-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-153">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="13384-154">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-154">None</span></span>|<span data-ttu-id="13384-155">Gerät neu starten</span><span class="sxs-lookup"><span data-stu-id="13384-155">Reboot device</span></span>|
|[<span data-ttu-id="13384-156">shutDown-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-156">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="13384-157">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-157">None</span></span>|<span data-ttu-id="13384-158">Gerät abschalten</span><span class="sxs-lookup"><span data-stu-id="13384-158">Shut down device</span></span>|
|[<span data-ttu-id="13384-159">recoverPasscode-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-159">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="13384-160">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-160">None</span></span>|<span data-ttu-id="13384-161">Kennung wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="13384-161">Recover passcode</span></span>|
|[<span data-ttu-id="13384-162">cleanWindowsDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-162">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="13384-163">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-163">None</span></span>|<span data-ttu-id="13384-164">Windows-Gerät bereinigen</span><span class="sxs-lookup"><span data-stu-id="13384-164">Clean Windows device</span></span>|
|[<span data-ttu-id="13384-165">logoutSharedAppleDeviceActiveUser-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-165">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="13384-166">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-166">None</span></span>|<span data-ttu-id="13384-167">Aktiven Benutzer von freigegebenem Apple-Gerät abmelden</span><span class="sxs-lookup"><span data-stu-id="13384-167">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="13384-168">deleteUserFromSharedAppleDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-168">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="13384-169">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-169">None</span></span>|<span data-ttu-id="13384-170">Benutzer von freigegebenem Apple-Gerät löschen</span><span class="sxs-lookup"><span data-stu-id="13384-170">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="13384-171">syncDevice-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-171">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="13384-172">Keiner</span><span class="sxs-lookup"><span data-stu-id="13384-172">None</span></span>|<span data-ttu-id="13384-173">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="13384-173">Not yet documented</span></span>|
|[<span data-ttu-id="13384-174">windowsDefenderScan-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-174">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="13384-175">Keiner</span><span class="sxs-lookup"><span data-stu-id="13384-175">None</span></span>|<span data-ttu-id="13384-176">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="13384-176">Not yet documented</span></span>|
|[<span data-ttu-id="13384-177">windowsDefenderUpdateSignatures-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-177">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="13384-178">Keiner</span><span class="sxs-lookup"><span data-stu-id="13384-178">None</span></span>|<span data-ttu-id="13384-179">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="13384-179">Not yet documented</span></span>|
|[<span data-ttu-id="13384-180">updateWindowsDeviceAccount-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-180">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="13384-181">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-181">None</span></span>|<span data-ttu-id="13384-182">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="13384-182">Not yet documented</span></span>|
|[<span data-ttu-id="13384-183">revokeAppleVppLicenses-Aktion</span><span class="sxs-lookup"><span data-stu-id="13384-183">revokeAppleVppLicenses action</span></span>](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|<span data-ttu-id="13384-184">Keine</span><span class="sxs-lookup"><span data-stu-id="13384-184">None</span></span>|<span data-ttu-id="13384-185">Alle Apple VPP-Lizenzen für ein Gerät widerrufen</span><span class="sxs-lookup"><span data-stu-id="13384-185">Revoke all Apple Vpp licenses for a device</span></span>|

## <a name="properties"></a><span data-ttu-id="13384-186">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="13384-186">Properties</span></span>
|<span data-ttu-id="13384-187">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13384-187">Property</span></span>|<span data-ttu-id="13384-188">Typ</span><span class="sxs-lookup"><span data-stu-id="13384-188">Type</span></span>|<span data-ttu-id="13384-189">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13384-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13384-190">id</span><span class="sxs-lookup"><span data-stu-id="13384-190">id</span></span>|<span data-ttu-id="13384-191">string</span><span class="sxs-lookup"><span data-stu-id="13384-191">String</span></span>|<span data-ttu-id="13384-192">Eindeutiger Bezeichner für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="13384-192">Unique Identifier for the device</span></span>|
|<span data-ttu-id="13384-193">userId</span><span class="sxs-lookup"><span data-stu-id="13384-193">userId</span></span>|<span data-ttu-id="13384-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-194">String</span></span>|<span data-ttu-id="13384-195">Eindeutiger Bezeichner des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="13384-195">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="13384-196">deviceName</span><span class="sxs-lookup"><span data-stu-id="13384-196">deviceName</span></span>|<span data-ttu-id="13384-197">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-197">String</span></span>|<span data-ttu-id="13384-198">Name des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="13384-198">Name of the device</span></span>|
|<span data-ttu-id="13384-199">Dem</span><span class="sxs-lookup"><span data-stu-id="13384-199">hardwareInformation</span></span>|[<span data-ttu-id="13384-200">Dem</span><span class="sxs-lookup"><span data-stu-id="13384-200">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="13384-201">Die hardward-Details für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="13384-201">The hardward details for the device.</span></span>  <span data-ttu-id="13384-202">Enthält Informationen wie Speicherplatz, Hersteller, Seriennummer usw.</span><span class="sxs-lookup"><span data-stu-id="13384-202">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="13384-203">ownerType</span><span class="sxs-lookup"><span data-stu-id="13384-203">ownerType</span></span>|[<span data-ttu-id="13384-204">ownerType</span><span class="sxs-lookup"><span data-stu-id="13384-204">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="13384-205">Der Besitzer des Geräts.</span><span class="sxs-lookup"><span data-stu-id="13384-205">Ownership of the device.</span></span> <span data-ttu-id="13384-206">Kann "Company" oder "Personal" sein.</span><span class="sxs-lookup"><span data-stu-id="13384-206">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="13384-207">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="13384-207">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="13384-208">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="13384-208">managedDeviceOwnerType</span></span>|[<span data-ttu-id="13384-209">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="13384-209">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="13384-210">Der Besitzer des Geräts.</span><span class="sxs-lookup"><span data-stu-id="13384-210">Ownership of the device.</span></span> <span data-ttu-id="13384-211">Kann "Company" oder "Personal" sein.</span><span class="sxs-lookup"><span data-stu-id="13384-211">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="13384-212">Mögliche Werte sind: `unknown`, `company` und `personal`.</span><span class="sxs-lookup"><span data-stu-id="13384-212">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="13384-213">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="13384-213">deviceActionResults</span></span>|<span data-ttu-id="13384-214">Collection von Objekten des Typs [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="13384-214">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="13384-215">Liste von Objekten des Typs „ComplexType deviceActionResult“.
</span><span class="sxs-lookup"><span data-stu-id="13384-215">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="13384-216">managementState</span><span class="sxs-lookup"><span data-stu-id="13384-216">managementState</span></span>|[<span data-ttu-id="13384-217">managementState</span><span class="sxs-lookup"><span data-stu-id="13384-217">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="13384-218">Verwaltungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="13384-218">Management state of the device.</span></span> <span data-ttu-id="13384-219">Mögliche Werte sind: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled` und `discovered`.</span><span class="sxs-lookup"><span data-stu-id="13384-219">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="13384-220">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="13384-220">enrolledDateTime</span></span>|<span data-ttu-id="13384-221">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13384-221">DateTimeOffset</span></span>|<span data-ttu-id="13384-222">Datum und Uhrzeit der Geräteregistrierung.
</span><span class="sxs-lookup"><span data-stu-id="13384-222">Enrollment time of the device.</span></span>|
|<span data-ttu-id="13384-223">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="13384-223">lastSyncDateTime</span></span>|<span data-ttu-id="13384-224">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13384-224">DateTimeOffset</span></span>|<span data-ttu-id="13384-225">Datum und Uhrzeit der letzten erfolgreichen Synchronisierung des Geräts mit Intune.
</span><span class="sxs-lookup"><span data-stu-id="13384-225">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="13384-226">chassitype</span><span class="sxs-lookup"><span data-stu-id="13384-226">chassisType</span></span>|[<span data-ttu-id="13384-227">chassitype</span><span class="sxs-lookup"><span data-stu-id="13384-227">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="13384-228">Gehäusetyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="13384-228">Chassis type of the device.</span></span> <span data-ttu-id="13384-229">Mögliche Werte: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span><span class="sxs-lookup"><span data-stu-id="13384-229">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="13384-230">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="13384-230">operatingSystem</span></span>|<span data-ttu-id="13384-231">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-231">String</span></span>|<span data-ttu-id="13384-232">Betriebssystem des Geräts.</span><span class="sxs-lookup"><span data-stu-id="13384-232">Operating system of the device.</span></span> <span data-ttu-id="13384-233">Windows, iOS usw.</span><span class="sxs-lookup"><span data-stu-id="13384-233">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="13384-234">deviceType</span><span class="sxs-lookup"><span data-stu-id="13384-234">deviceType</span></span>|[<span data-ttu-id="13384-235">deviceType</span><span class="sxs-lookup"><span data-stu-id="13384-235">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="13384-236">Plattform des Geräts.</span><span class="sxs-lookup"><span data-stu-id="13384-236">Platform of the device.</span></span> <span data-ttu-id="13384-237">Mögliche Werte sind: `desktop`, `windowsRT`, `winMO6` `nokia` `windowsPhone` `mac` `winCE` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM`,,,,,,,, `holoLens`,, `androidEnterprise` ,,,,,, `surfaceHub` `androidForWork` `winEmbedded` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="13384-237">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="13384-238">complianceState</span><span class="sxs-lookup"><span data-stu-id="13384-238">complianceState</span></span>|[<span data-ttu-id="13384-239">complianceState</span><span class="sxs-lookup"><span data-stu-id="13384-239">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="13384-240">Konformitätsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="13384-240">Compliance state of the device.</span></span> <span data-ttu-id="13384-241">Mögliche Werte sind: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod` und `configManager`.</span><span class="sxs-lookup"><span data-stu-id="13384-241">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="13384-242">jailBroken</span><span class="sxs-lookup"><span data-stu-id="13384-242">jailBroken</span></span>|<span data-ttu-id="13384-243">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-243">String</span></span>|<span data-ttu-id="13384-244">Gibt an, ob es sich um ein Gerät mit Jailbreak oder Rootzugriff handelt.</span><span class="sxs-lookup"><span data-stu-id="13384-244">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="13384-245">managementAgent</span><span class="sxs-lookup"><span data-stu-id="13384-245">managementAgent</span></span>|[<span data-ttu-id="13384-246">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="13384-246">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="13384-247">Verwaltungskanal des Geräts.</span><span class="sxs-lookup"><span data-stu-id="13384-247">Management channel of the device.</span></span> <span data-ttu-id="13384-248">InTune, EAS usw. Mögliche Werte sind: `eas`, `mdm`, `easMdm` `intuneClient`,, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm` `configurationManagerClientMdmEas`,, `unknown`, `jamf` `googleCloudDevicePolicyController`,, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="13384-248">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="13384-249">osVersion</span><span class="sxs-lookup"><span data-stu-id="13384-249">osVersion</span></span>|<span data-ttu-id="13384-250">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-250">String</span></span>|<span data-ttu-id="13384-251">Auf dem Gerät installierte Betriebssystemversion.
</span><span class="sxs-lookup"><span data-stu-id="13384-251">Operating system version of the device.</span></span>|
|<span data-ttu-id="13384-252">easActivated</span><span class="sxs-lookup"><span data-stu-id="13384-252">easActivated</span></span>|<span data-ttu-id="13384-253">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13384-253">Boolean</span></span>|<span data-ttu-id="13384-254">Gibt an, ob für das Gerät Exchange ActiveSync aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="13384-254">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="13384-255">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="13384-255">easDeviceId</span></span>|<span data-ttu-id="13384-256">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-256">String</span></span>|<span data-ttu-id="13384-257">Exchange ActiveSync-ID des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="13384-257">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="13384-258">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="13384-258">easActivationDateTime</span></span>|<span data-ttu-id="13384-259">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13384-259">DateTimeOffset</span></span>|<span data-ttu-id="13384-260">Datum und Uhrzeit der Exchange ActiveSync-Aktivierung für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="13384-260">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="13384-261">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="13384-261">aadRegistered</span></span>|<span data-ttu-id="13384-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="13384-262">Boolean</span></span>|<span data-ttu-id="13384-263">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="13384-263">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="13384-264">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="13384-264">azureADRegistered</span></span>|<span data-ttu-id="13384-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="13384-265">Boolean</span></span>|<span data-ttu-id="13384-266">Gibt an, ob das Gerät in Azure Active Directory registriert ist.</span><span class="sxs-lookup"><span data-stu-id="13384-266">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="13384-267">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="13384-267">deviceEnrollmentType</span></span>|[<span data-ttu-id="13384-268">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="13384-268">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="13384-269">Registrierungstyp des Geräts.</span><span class="sxs-lookup"><span data-stu-id="13384-269">Enrollment type of the device.</span></span> <span data-ttu-id="13384-270">Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span><span class="sxs-lookup"><span data-stu-id="13384-270">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="13384-271">lostModeState</span><span class="sxs-lookup"><span data-stu-id="13384-271">lostModeState</span></span>|[<span data-ttu-id="13384-272">lostModeState</span><span class="sxs-lookup"><span data-stu-id="13384-272">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="13384-273">Gibt an, ob der Modus verloren aktiviert oder deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="13384-273">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="13384-274">Mögliche Werte sind: `disabled` und `enabled`.</span><span class="sxs-lookup"><span data-stu-id="13384-274">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="13384-275">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="13384-275">activationLockBypassCode</span></span>|<span data-ttu-id="13384-276">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-276">String</span></span>|<span data-ttu-id="13384-277">Code, der die Umgehung der Aktivierungssperre des Geräts ermöglicht</span><span class="sxs-lookup"><span data-stu-id="13384-277">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="13384-278">emailAddress</span><span class="sxs-lookup"><span data-stu-id="13384-278">emailAddress</span></span>|<span data-ttu-id="13384-279">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-279">String</span></span>|<span data-ttu-id="13384-280">E-Mail-Adressen des Benutzers, der dem Gerät zugeordnet ist.
</span><span class="sxs-lookup"><span data-stu-id="13384-280">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="13384-281">Eigenschaften azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="13384-281">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="13384-282">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-282">String</span></span>|<span data-ttu-id="13384-283">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="13384-283">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="13384-284">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="13384-284">Read only.</span></span>|
|<span data-ttu-id="13384-285">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="13384-285">azureADDeviceId</span></span>|<span data-ttu-id="13384-286">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-286">String</span></span>|<span data-ttu-id="13384-287">Eindeutiger Bezeichner des Azure Active Directory-Geräts.</span><span class="sxs-lookup"><span data-stu-id="13384-287">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="13384-288">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="13384-288">Read only.</span></span>|
|<span data-ttu-id="13384-289">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="13384-289">deviceRegistrationState</span></span>|[<span data-ttu-id="13384-290">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="13384-290">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="13384-291">Registrierungsstatus des Geräts.</span><span class="sxs-lookup"><span data-stu-id="13384-291">Device registration state.</span></span> <span data-ttu-id="13384-292">Mögliche Werte sind: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset` und `notRegisteredPendingEnrollment`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="13384-292">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="13384-293">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="13384-293">deviceCategoryDisplayName</span></span>|<span data-ttu-id="13384-294">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-294">String</span></span>|<span data-ttu-id="13384-295">Anzeigename der Gerätekategorie.
</span><span class="sxs-lookup"><span data-stu-id="13384-295">Device category display name</span></span>|
|<span data-ttu-id="13384-296">isSupervised</span><span class="sxs-lookup"><span data-stu-id="13384-296">isSupervised</span></span>|<span data-ttu-id="13384-297">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13384-297">Boolean</span></span>|<span data-ttu-id="13384-298">Überwachungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="13384-298">Device supervised status</span></span>|
|<span data-ttu-id="13384-299">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="13384-299">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="13384-300">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13384-300">DateTimeOffset</span></span>|<span data-ttu-id="13384-301">Datum und Uhrzeit der letzten Verbindung des Geräts mit Exchange</span><span class="sxs-lookup"><span data-stu-id="13384-301">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="13384-302">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="13384-302">exchangeAccessState</span></span>|[<span data-ttu-id="13384-303">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="13384-303">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="13384-304">Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="13384-304">The Access State of the device in Exchange.</span></span> <span data-ttu-id="13384-305">Mögliche Werte: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span><span class="sxs-lookup"><span data-stu-id="13384-305">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="13384-306">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="13384-306">exchangeAccessStateReason</span></span>|[<span data-ttu-id="13384-307">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="13384-307">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="13384-308">Grund für den Zugriffsstatus des Geräts in Exchange.</span><span class="sxs-lookup"><span data-stu-id="13384-308">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="13384-309">Mögliche Werte sind: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword` und `deviceNotKnownWithManagedApp`.</span><span class="sxs-lookup"><span data-stu-id="13384-309">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="13384-310">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="13384-310">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="13384-311">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-311">String</span></span>|<span data-ttu-id="13384-312">URL zur Einrichtung einer Remoteunterstützungssitzung mit dem Gerät.
</span><span class="sxs-lookup"><span data-stu-id="13384-312">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="13384-313">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="13384-313">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="13384-314">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-314">String</span></span>|<span data-ttu-id="13384-315">Fehlerzeichenfolge zur Beschreibung von Fehlern beim Erstellen von Objekten für Remoteunterstützungssitzungen.
</span><span class="sxs-lookup"><span data-stu-id="13384-315">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="13384-316">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="13384-316">isEncrypted</span></span>|<span data-ttu-id="13384-317">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13384-317">Boolean</span></span>|<span data-ttu-id="13384-318">Verschlüsselungsstatus des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="13384-318">Device encryption status</span></span>|
|<span data-ttu-id="13384-319">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="13384-319">userPrincipalName</span></span>|<span data-ttu-id="13384-320">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-320">String</span></span>|<span data-ttu-id="13384-321">Benutzerprinzipalname für das Gerät.
</span><span class="sxs-lookup"><span data-stu-id="13384-321">Device user principal name</span></span>|
|<span data-ttu-id="13384-322">model</span><span class="sxs-lookup"><span data-stu-id="13384-322">model</span></span>|<span data-ttu-id="13384-323">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-323">String</span></span>|<span data-ttu-id="13384-324">Modell des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="13384-324">Model of the device</span></span>|
|<span data-ttu-id="13384-325">manufacturer</span><span class="sxs-lookup"><span data-stu-id="13384-325">manufacturer</span></span>|<span data-ttu-id="13384-326">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-326">String</span></span>|<span data-ttu-id="13384-327">Hersteller des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="13384-327">Manufacturer of the device</span></span>|
|<span data-ttu-id="13384-328">imei</span><span class="sxs-lookup"><span data-stu-id="13384-328">imei</span></span>|<span data-ttu-id="13384-329">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-329">String</span></span>|<span data-ttu-id="13384-330">IMEI</span><span class="sxs-lookup"><span data-stu-id="13384-330">IMEI</span></span>|
|<span data-ttu-id="13384-331">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="13384-331">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="13384-332">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13384-332">DateTimeOffset</span></span>|<span data-ttu-id="13384-333">Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität.
</span><span class="sxs-lookup"><span data-stu-id="13384-333">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="13384-334">serialNumber</span><span class="sxs-lookup"><span data-stu-id="13384-334">serialNumber</span></span>|<span data-ttu-id="13384-335">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-335">String</span></span>|<span data-ttu-id="13384-336">Seriennummer.
</span><span class="sxs-lookup"><span data-stu-id="13384-336">SerialNumber</span></span>|
|<span data-ttu-id="13384-337">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="13384-337">phoneNumber</span></span>|<span data-ttu-id="13384-338">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-338">String</span></span>|<span data-ttu-id="13384-339">Telefonnummer des Geräts.
</span><span class="sxs-lookup"><span data-stu-id="13384-339">Phone number of the device</span></span>|
|<span data-ttu-id="13384-340">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="13384-340">androidSecurityPatchLevel</span></span>|<span data-ttu-id="13384-341">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-341">String</span></span>|<span data-ttu-id="13384-342">Android-Sicherheitspatchlevel.
</span><span class="sxs-lookup"><span data-stu-id="13384-342">Android security patch level</span></span>|
|<span data-ttu-id="13384-343">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="13384-343">userDisplayName</span></span>|<span data-ttu-id="13384-344">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-344">String</span></span>|<span data-ttu-id="13384-345">Anzeigename des Benutzers.
</span><span class="sxs-lookup"><span data-stu-id="13384-345">User display name</span></span>|
|<span data-ttu-id="13384-346">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="13384-346">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="13384-347">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="13384-347">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="13384-348">Aktivierte Funktionen des Konfigurations-Manager-Clients.
</span><span class="sxs-lookup"><span data-stu-id="13384-348">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="13384-349">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="13384-349">wiFiMacAddress</span></span>|<span data-ttu-id="13384-350">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-350">String</span></span>|<span data-ttu-id="13384-351">WLAN-MAC</span><span class="sxs-lookup"><span data-stu-id="13384-351">Wi-Fi MAC</span></span>|
|<span data-ttu-id="13384-352">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="13384-352">deviceHealthAttestationState</span></span>|[<span data-ttu-id="13384-353">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="13384-353">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="13384-354">Status des Integritätsnachweises für Geräte.
</span><span class="sxs-lookup"><span data-stu-id="13384-354">The device health attestation state.</span></span>|
|<span data-ttu-id="13384-355">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="13384-355">subscriberCarrier</span></span>|<span data-ttu-id="13384-356">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-356">String</span></span>|<span data-ttu-id="13384-357">Netzbetreiber des Abonnenten.
</span><span class="sxs-lookup"><span data-stu-id="13384-357">Subscriber Carrier</span></span>|
|<span data-ttu-id="13384-358">meid</span><span class="sxs-lookup"><span data-stu-id="13384-358">meid</span></span>|<span data-ttu-id="13384-359">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-359">String</span></span>|<span data-ttu-id="13384-360">MEID</span><span class="sxs-lookup"><span data-stu-id="13384-360">MEID</span></span>|
|<span data-ttu-id="13384-361">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="13384-361">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="13384-362">Int64</span><span class="sxs-lookup"><span data-stu-id="13384-362">Int64</span></span>|<span data-ttu-id="13384-363">Gesamtspeicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="13384-363">Total Storage in Bytes</span></span>|
|<span data-ttu-id="13384-364">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="13384-364">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="13384-365">Int64</span><span class="sxs-lookup"><span data-stu-id="13384-365">Int64</span></span>|<span data-ttu-id="13384-366">Freier Speicher in Byte.
</span><span class="sxs-lookup"><span data-stu-id="13384-366">Free Storage in Bytes</span></span>|
|<span data-ttu-id="13384-367">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="13384-367">managedDeviceName</span></span>|<span data-ttu-id="13384-368">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-368">String</span></span>|<span data-ttu-id="13384-369">Automatisch generierter Name zur Identifizierung des Geräts.</span><span class="sxs-lookup"><span data-stu-id="13384-369">Automatically generated name to identify a device.</span></span> <span data-ttu-id="13384-370">Kann mit einem benutzerfreundlichen Namen überschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="13384-370">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="13384-371">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="13384-371">partnerReportedThreatState</span></span>|[<span data-ttu-id="13384-372">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="13384-372">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="13384-373">Gibt den Bedrohungsstatus eines Geräts an, wenn das Konto und das Gerät einen Mobile Threat Defense-Partner nutzen.</span><span class="sxs-lookup"><span data-stu-id="13384-373">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="13384-374">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="13384-374">Read Only.</span></span> <span data-ttu-id="13384-375">Mögliche Werte: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span><span class="sxs-lookup"><span data-stu-id="13384-375">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="13384-376">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="13384-376">usersLoggedOn</span></span>|<span data-ttu-id="13384-377">[loggedOnUser](../resources/intune-devices-loggedonuser.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="13384-377">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="13384-378">Gibt die zuletzt angemeldeten Benutzer eines Geräts an.</span><span class="sxs-lookup"><span data-stu-id="13384-378">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="13384-379">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="13384-379">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="13384-380">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13384-380">DateTimeOffset</span></span>|<span data-ttu-id="13384-381">Meldet den DateTime-Wert für die Einstellung preferMdmOverGroupPolicy.</span><span class="sxs-lookup"><span data-stu-id="13384-381">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="13384-382">Ist diese Einstellung festgelegt, überschreiben die Intune-MDM-Einstellungen Gruppenrichtlinieneinstellungen bei einem Konflikt.</span><span class="sxs-lookup"><span data-stu-id="13384-382">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="13384-383">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="13384-383">Read Only.</span></span>|
|<span data-ttu-id="13384-384">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="13384-384">autopilotEnrolled</span></span>|<span data-ttu-id="13384-385">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13384-385">Boolean</span></span>|<span data-ttu-id="13384-386">Meldet, ob das verwaltete Gerät über Auto-Pilot registriert wird.</span><span class="sxs-lookup"><span data-stu-id="13384-386">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="13384-387">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="13384-387">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="13384-388">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="13384-388">Boolean</span></span>|<span data-ttu-id="13384-389">Meldet, ob das verwaltete iOS-Gerät Benutzer Genehmigungs Registrierung ist.</span><span class="sxs-lookup"><span data-stu-id="13384-389">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="13384-390">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="13384-390">managementCertificateExpirationDate</span></span>|<span data-ttu-id="13384-391">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13384-391">DateTimeOffset</span></span>|<span data-ttu-id="13384-392">Meldet Ablaufdatum für das Geräte Verwaltungszertifikat</span><span class="sxs-lookup"><span data-stu-id="13384-392">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="13384-393">ICCID</span><span class="sxs-lookup"><span data-stu-id="13384-393">iccid</span></span>|<span data-ttu-id="13384-394">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-394">String</span></span>|<span data-ttu-id="13384-395">Integrated Circuit Card Identifier, es ist die eindeutige Identifikationsnummer einer SIM-Karte.</span><span class="sxs-lookup"><span data-stu-id="13384-395">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="13384-396">UDID</span><span class="sxs-lookup"><span data-stu-id="13384-396">udid</span></span>|<span data-ttu-id="13384-397">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-397">String</span></span>|<span data-ttu-id="13384-398">Eindeutige Gerätekennung für iOS-und macOS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="13384-398">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="13384-399">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="13384-399">roleScopeTagIds</span></span>|<span data-ttu-id="13384-400">String collection</span><span class="sxs-lookup"><span data-stu-id="13384-400">String collection</span></span>|<span data-ttu-id="13384-401">Liste der Bereichstag-IDs für diese Geräteinstanz.</span><span class="sxs-lookup"><span data-stu-id="13384-401">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="13384-402">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="13384-402">windowsActiveMalwareCount</span></span>|<span data-ttu-id="13384-403">Int32</span><span class="sxs-lookup"><span data-stu-id="13384-403">Int32</span></span>|<span data-ttu-id="13384-404">Anzahl der aktiven Schadsoftware für dieses Windows-Gerät</span><span class="sxs-lookup"><span data-stu-id="13384-404">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="13384-405">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="13384-405">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="13384-406">Int32</span><span class="sxs-lookup"><span data-stu-id="13384-406">Int32</span></span>|<span data-ttu-id="13384-407">Anzahl der korrigierten Schadsoftware für dieses Windows-Gerät</span><span class="sxs-lookup"><span data-stu-id="13384-407">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="13384-408">notes</span><span class="sxs-lookup"><span data-stu-id="13384-408">notes</span></span>|<span data-ttu-id="13384-409">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13384-409">String</span></span>|<span data-ttu-id="13384-410">Hinweise zu dem von IT-Administrator erstellten Gerät</span><span class="sxs-lookup"><span data-stu-id="13384-410">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="13384-411">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="13384-411">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="13384-412">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="13384-412">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="13384-413">Configuration Manager-Clientintegritätsstatus, nur gültig für Geräte, die vom MDM/ConfigMgr-Agent verwaltet werden</span><span class="sxs-lookup"><span data-stu-id="13384-413">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|

## <a name="relationships"></a><span data-ttu-id="13384-414">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="13384-414">Relationships</span></span>
|<span data-ttu-id="13384-415">Beziehung</span><span class="sxs-lookup"><span data-stu-id="13384-415">Relationship</span></span>|<span data-ttu-id="13384-416">Typ</span><span class="sxs-lookup"><span data-stu-id="13384-416">Type</span></span>|<span data-ttu-id="13384-417">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13384-417">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13384-418">detectedApps</span><span class="sxs-lookup"><span data-stu-id="13384-418">detectedApps</span></span>|<span data-ttu-id="13384-419">[detectedApp](../resources/intune-devices-detectedapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="13384-419">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="13384-420">Alle Anwendungen, die derzeit auf dem Gerät installiert sind</span><span class="sxs-lookup"><span data-stu-id="13384-420">All applications currently installed on the device</span></span>|
|<span data-ttu-id="13384-421">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="13384-421">deviceCategory</span></span>|[<span data-ttu-id="13384-422">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="13384-422">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="13384-423">Gerätekategorie</span><span class="sxs-lookup"><span data-stu-id="13384-423">Device category</span></span>|
|<span data-ttu-id="13384-424">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="13384-424">windowsProtectionState</span></span>|[<span data-ttu-id="13384-425">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="13384-425">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="13384-426">Der Status des Geräteschutzes.</span><span class="sxs-lookup"><span data-stu-id="13384-426">The device protection status.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13384-427">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="13384-427">JSON Representation</span></span>
<span data-ttu-id="13384-428">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="13384-428">Here is a JSON representation of the resource.</span></span>
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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




