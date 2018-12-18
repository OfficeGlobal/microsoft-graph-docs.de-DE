---
title: Aktualisieren von „androidGeneralDeviceConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs androidGeneralDeviceConfiguration.
author: tfitzmac
ms.openlocfilehash: bce3fa318ed7ff0e818c19a6907a34c26b804b35
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302443"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="30d2c-103">Aktualisieren von „androidGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="30d2c-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="30d2c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="30d2c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30d2c-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30d2c-105">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30d2c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="30d2c-106">Prerequisites</span></span>
<span data-ttu-id="30d2c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30d2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30d2c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="30d2c-109">Permission type</span></span>|<span data-ttu-id="30d2c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="30d2c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30d2c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="30d2c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="30d2c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30d2c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="30d2c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="30d2c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30d2c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30d2c-114">Not supported.</span></span>|
|<span data-ttu-id="30d2c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="30d2c-115">Application</span></span>|<span data-ttu-id="30d2c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30d2c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30d2c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="30d2c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="30d2c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="30d2c-118">Request headers</span></span>
|<span data-ttu-id="30d2c-119">Header</span><span class="sxs-lookup"><span data-stu-id="30d2c-119">Header</span></span>|<span data-ttu-id="30d2c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30d2c-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="30d2c-121">Authorization</span></span>|<span data-ttu-id="30d2c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="30d2c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30d2c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="30d2c-123">Accept</span></span>|<span data-ttu-id="30d2c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="30d2c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30d2c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="30d2c-125">Request body</span></span>
<span data-ttu-id="30d2c-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="30d2c-126">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="30d2c-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="30d2c-127">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="30d2c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="30d2c-128">Property</span></span>|<span data-ttu-id="30d2c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="30d2c-129">Type</span></span>|<span data-ttu-id="30d2c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30d2c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30d2c-131">id</span><span class="sxs-lookup"><span data-stu-id="30d2c-131">id</span></span>|<span data-ttu-id="30d2c-132">String</span><span class="sxs-lookup"><span data-stu-id="30d2c-132">String</span></span>|<span data-ttu-id="30d2c-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="30d2c-133">Key of the entity.</span></span> <span data-ttu-id="30d2c-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30d2c-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d2c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30d2c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="30d2c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30d2c-136">DateTimeOffset</span></span>|<span data-ttu-id="30d2c-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="30d2c-137">DateTime the object was last modified.</span></span> <span data-ttu-id="30d2c-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30d2c-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d2c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30d2c-139">createdDateTime</span></span>|<span data-ttu-id="30d2c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30d2c-140">DateTimeOffset</span></span>|<span data-ttu-id="30d2c-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="30d2c-141">DateTime the object was created.</span></span> <span data-ttu-id="30d2c-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30d2c-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d2c-143">description</span><span class="sxs-lookup"><span data-stu-id="30d2c-143">description</span></span>|<span data-ttu-id="30d2c-144">String</span><span class="sxs-lookup"><span data-stu-id="30d2c-144">String</span></span>|<span data-ttu-id="30d2c-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="30d2c-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="30d2c-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30d2c-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d2c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="30d2c-147">displayName</span></span>|<span data-ttu-id="30d2c-148">String</span><span class="sxs-lookup"><span data-stu-id="30d2c-148">String</span></span>|<span data-ttu-id="30d2c-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="30d2c-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="30d2c-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30d2c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d2c-151">Version</span><span class="sxs-lookup"><span data-stu-id="30d2c-151">version</span></span>|<span data-ttu-id="30d2c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="30d2c-152">Int32</span></span>|<span data-ttu-id="30d2c-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="30d2c-153">Version of the device configuration.</span></span> <span data-ttu-id="30d2c-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30d2c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d2c-155">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="30d2c-155">appsBlockClipboardSharing</span></span>|<span data-ttu-id="30d2c-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-156">Boolean</span></span>|<span data-ttu-id="30d2c-157">Gibt an, ob die gemeinsame Nutzung der Zwischenablage zum Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-157">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="30d2c-158">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="30d2c-158">appsBlockCopyPaste</span></span>|<span data-ttu-id="30d2c-159">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-159">Boolean</span></span>|<span data-ttu-id="30d2c-160">Gibt an, ob Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-160">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="30d2c-161">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="30d2c-161">appsBlockYouTube</span></span>|<span data-ttu-id="30d2c-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-162">Boolean</span></span>|<span data-ttu-id="30d2c-163">Gibt an, ob die YouTube-App blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-163">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="30d2c-164">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="30d2c-164">bluetoothBlocked</span></span>|<span data-ttu-id="30d2c-165">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-165">Boolean</span></span>|<span data-ttu-id="30d2c-166">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-166">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="30d2c-167">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="30d2c-167">cameraBlocked</span></span>|<span data-ttu-id="30d2c-168">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-168">Boolean</span></span>|<span data-ttu-id="30d2c-169">Gibt an, ob die Verwendung der Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-169">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="30d2c-170">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="30d2c-170">cellularBlockDataRoaming</span></span>|<span data-ttu-id="30d2c-171">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-171">Boolean</span></span>|<span data-ttu-id="30d2c-172">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-172">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="30d2c-173">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="30d2c-173">cellularBlockMessaging</span></span>|<span data-ttu-id="30d2c-174">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-174">Boolean</span></span>|<span data-ttu-id="30d2c-175">Gibt an, ob SMS-/MMS-Nachrichten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="30d2c-175">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="30d2c-176">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="30d2c-176">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="30d2c-177">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-177">Boolean</span></span>|<span data-ttu-id="30d2c-178">Gibt an, ob Sprachroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-178">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="30d2c-179">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="30d2c-179">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="30d2c-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-180">Boolean</span></span>|<span data-ttu-id="30d2c-181">Gibt an, ob die Synchronisierung von WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-181">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="30d2c-182">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="30d2c-182">compliantAppsList</span></span>|<span data-ttu-id="30d2c-183">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="30d2c-183">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="30d2c-184">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="30d2c-184">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="30d2c-185">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="30d2c-185">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="30d2c-186">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="30d2c-186">compliantAppListType</span></span>|[<span data-ttu-id="30d2c-187">appListType</span><span class="sxs-lookup"><span data-stu-id="30d2c-187">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="30d2c-188">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="30d2c-188">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="30d2c-189">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="30d2c-189">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="30d2c-190">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="30d2c-190">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="30d2c-191">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-191">Boolean</span></span>|<span data-ttu-id="30d2c-192">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-192">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="30d2c-193">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="30d2c-193">locationServicesBlocked</span></span>|<span data-ttu-id="30d2c-194">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-194">Boolean</span></span>|<span data-ttu-id="30d2c-195">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="30d2c-195">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="30d2c-196">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="30d2c-196">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="30d2c-197">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-197">Boolean</span></span>|<span data-ttu-id="30d2c-198">Gibt an, ob die automatische Synchronisierung von Google-Konten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-198">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="30d2c-199">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="30d2c-199">googlePlayStoreBlocked</span></span>|<span data-ttu-id="30d2c-200">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-200">Boolean</span></span>|<span data-ttu-id="30d2c-201">Gibt an, ob der Google Play-Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-201">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="30d2c-202">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="30d2c-202">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="30d2c-203">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-203">Boolean</span></span>|<span data-ttu-id="30d2c-204">Gibt an, ob die Standbytaste im Kioskmodus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-204">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="30d2c-205">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="30d2c-205">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="30d2c-206">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-206">Boolean</span></span>|<span data-ttu-id="30d2c-207">Gibt an, ob die Lautstärkeregler im Kioskmodus blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="30d2c-207">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="30d2c-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="30d2c-208">kioskModeApps</span></span>|<span data-ttu-id="30d2c-209">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="30d2c-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="30d2c-210">Eine Liste der Apps, die ausgeführt werden können, wenn sich das Gerät im Kioskmodus befindet.</span><span class="sxs-lookup"><span data-stu-id="30d2c-210">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="30d2c-211">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="30d2c-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="30d2c-212">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="30d2c-212">nfcBlocked</span></span>|<span data-ttu-id="30d2c-213">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-213">Boolean</span></span>|<span data-ttu-id="30d2c-214">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-214">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="30d2c-215">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="30d2c-215">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="30d2c-216">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-216">Boolean</span></span>|<span data-ttu-id="30d2c-217">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-217">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="30d2c-218">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="30d2c-218">passwordBlockTrustAgents</span></span>|<span data-ttu-id="30d2c-219">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-219">Boolean</span></span>|<span data-ttu-id="30d2c-220">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="30d2c-220">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="30d2c-221">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="30d2c-221">passwordExpirationDays</span></span>|<span data-ttu-id="30d2c-222">Int32</span><span class="sxs-lookup"><span data-stu-id="30d2c-222">Int32</span></span>|<span data-ttu-id="30d2c-223">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="30d2c-223">Number of days before the password expires.</span></span> <span data-ttu-id="30d2c-224">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="30d2c-224">Valid values 1 to 365</span></span>|
|<span data-ttu-id="30d2c-225">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="30d2c-225">passwordMinimumLength</span></span>|<span data-ttu-id="30d2c-226">Int32</span><span class="sxs-lookup"><span data-stu-id="30d2c-226">Int32</span></span>|<span data-ttu-id="30d2c-227">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="30d2c-227">Minimum length of passwords.</span></span> <span data-ttu-id="30d2c-228">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="30d2c-228">Valid values 4 to 16</span></span>|
|<span data-ttu-id="30d2c-229">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="30d2c-229">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="30d2c-230">Int32</span><span class="sxs-lookup"><span data-stu-id="30d2c-230">Int32</span></span>|<span data-ttu-id="30d2c-231">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="30d2c-231">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="30d2c-232">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="30d2c-232">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="30d2c-233">Int32</span><span class="sxs-lookup"><span data-stu-id="30d2c-233">Int32</span></span>|<span data-ttu-id="30d2c-234">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="30d2c-234">Number of previous passwords to block.</span></span> <span data-ttu-id="30d2c-235">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="30d2c-235">Valid values 0 to 24</span></span>|
|<span data-ttu-id="30d2c-236">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="30d2c-236">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="30d2c-237">Int32</span><span class="sxs-lookup"><span data-stu-id="30d2c-237">Int32</span></span>|<span data-ttu-id="30d2c-238">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="30d2c-238">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="30d2c-239">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="30d2c-239">Valid values 4 to 11</span></span>|
|<span data-ttu-id="30d2c-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="30d2c-240">passwordRequiredType</span></span>|[<span data-ttu-id="30d2c-241">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="30d2c-241">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="30d2c-242">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="30d2c-242">Type of password that is required.</span></span> <span data-ttu-id="30d2c-243">Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="30d2c-243">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="30d2c-244">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="30d2c-244">passwordRequired</span></span>|<span data-ttu-id="30d2c-245">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-245">Boolean</span></span>|<span data-ttu-id="30d2c-246">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="30d2c-246">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="30d2c-247">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="30d2c-247">powerOffBlocked</span></span>|<span data-ttu-id="30d2c-248">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-248">Boolean</span></span>|<span data-ttu-id="30d2c-249">Gibt an, ob das Ausschalten des Geräts blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-249">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="30d2c-250">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="30d2c-250">factoryResetBlocked</span></span>|<span data-ttu-id="30d2c-251">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-251">Boolean</span></span>|<span data-ttu-id="30d2c-252">Gibt an, ob verhindert werden soll, dass der Benutzer eine Zurücksetzung auf die Werkseinstellungen durchführt.</span><span class="sxs-lookup"><span data-stu-id="30d2c-252">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="30d2c-253">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="30d2c-253">screenCaptureBlocked</span></span>|<span data-ttu-id="30d2c-254">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-254">Boolean</span></span>|<span data-ttu-id="30d2c-255">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="30d2c-255">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="30d2c-256">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="30d2c-256">deviceSharingAllowed</span></span>|<span data-ttu-id="30d2c-257">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-257">Boolean</span></span>|<span data-ttu-id="30d2c-258">Gibt an, ob der Gerätefreigabemodus zugelassen wird.</span><span class="sxs-lookup"><span data-stu-id="30d2c-258">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="30d2c-259">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="30d2c-259">storageBlockGoogleBackup</span></span>|<span data-ttu-id="30d2c-260">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-260">Boolean</span></span>|<span data-ttu-id="30d2c-261">Gibt an, ob die Google-Sicherung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-261">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="30d2c-262">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="30d2c-262">storageBlockRemovableStorage</span></span>|<span data-ttu-id="30d2c-263">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-263">Boolean</span></span>|<span data-ttu-id="30d2c-264">Gibt an, ob die Verwendung von Wechselmedien blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-264">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="30d2c-265">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="30d2c-265">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="30d2c-266">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-266">Boolean</span></span>|<span data-ttu-id="30d2c-267">Gibt an, ob eine Geräteverschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="30d2c-267">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="30d2c-268">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="30d2c-268">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="30d2c-269">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-269">Boolean</span></span>|<span data-ttu-id="30d2c-270">Gibt an, ob die Verschlüsselung von Wechselmedien erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="30d2c-270">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="30d2c-271">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="30d2c-271">voiceAssistantBlocked</span></span>|<span data-ttu-id="30d2c-272">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-272">Boolean</span></span>|<span data-ttu-id="30d2c-273">Gibt an, ob die Verwendung des Sprach-Assistenten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-273">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="30d2c-274">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="30d2c-274">voiceDialingBlocked</span></span>|<span data-ttu-id="30d2c-275">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-275">Boolean</span></span>|<span data-ttu-id="30d2c-276">Gibt an, ob das Sprachwahlverfahren blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-276">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="30d2c-277">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="30d2c-277">webBrowserBlockPopups</span></span>|<span data-ttu-id="30d2c-278">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-278">Boolean</span></span>|<span data-ttu-id="30d2c-279">Gibt an, ob Popups innerhalb des Webbrowsers blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="30d2c-279">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="30d2c-280">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="30d2c-280">webBrowserBlockAutofill</span></span>|<span data-ttu-id="30d2c-281">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-281">Boolean</span></span>|<span data-ttu-id="30d2c-282">Gibt an, ob das AutoAusfüllen-Feature des Webbrowsers blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-282">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="30d2c-283">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="30d2c-283">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="30d2c-284">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-284">Boolean</span></span>|<span data-ttu-id="30d2c-285">Gibt an, ob JavaScript im Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-285">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="30d2c-286">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="30d2c-286">webBrowserBlocked</span></span>|<span data-ttu-id="30d2c-287">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-287">Boolean</span></span>|<span data-ttu-id="30d2c-288">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-288">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="30d2c-289">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="30d2c-289">webBrowserCookieSettings</span></span>|[<span data-ttu-id="30d2c-290">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="30d2c-290">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="30d2c-291">Cookieeinstellungen des Webbrowsers.</span><span class="sxs-lookup"><span data-stu-id="30d2c-291">Cookie settings within the web browser.</span></span> <span data-ttu-id="30d2c-292">Mögliche Werte sind: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited` und `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="30d2c-292">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="30d2c-293">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="30d2c-293">wiFiBlocked</span></span>|<span data-ttu-id="30d2c-294">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-294">Boolean</span></span>|<span data-ttu-id="30d2c-295">Gibt an, ob die WLAN-Synchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="30d2c-295">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="30d2c-296">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="30d2c-296">appsInstallAllowList</span></span>|<span data-ttu-id="30d2c-297">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="30d2c-297">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="30d2c-298">Liste von Apps, die auf dem KNOX-Gerät installiert werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="30d2c-298">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="30d2c-299">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="30d2c-299">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="30d2c-300">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="30d2c-300">appsLaunchBlockList</span></span>|<span data-ttu-id="30d2c-301">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="30d2c-301">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="30d2c-302">Liste von Apps, die auf dem KNOX-Gerät nicht gestartet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="30d2c-302">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="30d2c-303">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="30d2c-303">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="30d2c-304">appsHideList</span><span class="sxs-lookup"><span data-stu-id="30d2c-304">appsHideList</span></span>|<span data-ttu-id="30d2c-305">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="30d2c-305">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="30d2c-306">Liste von Apps, die auf dem KNOX-Gerät ausgeblendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="30d2c-306">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="30d2c-307">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="30d2c-307">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="30d2c-308">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="30d2c-308">securityRequireVerifyApps</span></span>|<span data-ttu-id="30d2c-309">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="30d2c-309">Boolean</span></span>|<span data-ttu-id="30d2c-310">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="30d2c-310">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="30d2c-311">Antwort</span><span class="sxs-lookup"><span data-stu-id="30d2c-311">Response</span></span>
<span data-ttu-id="30d2c-312">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="30d2c-312">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30d2c-313">Beispiel</span><span class="sxs-lookup"><span data-stu-id="30d2c-313">Example</span></span>
### <a name="request"></a><span data-ttu-id="30d2c-314">Anforderung</span><span class="sxs-lookup"><span data-stu-id="30d2c-314">Request</span></span>
<span data-ttu-id="30d2c-315">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="30d2c-315">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3033

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="30d2c-316">Antwort</span><span class="sxs-lookup"><span data-stu-id="30d2c-316">Response</span></span>
<span data-ttu-id="30d2c-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="30d2c-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3205

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```



