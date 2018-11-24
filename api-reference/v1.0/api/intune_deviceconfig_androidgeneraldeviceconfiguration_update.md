# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="c1841-101">Aktualisieren von „androidGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="c1841-101">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="c1841-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c1841-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1841-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1841-103">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1841-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1841-104">Prerequisites</span></span>
<span data-ttu-id="c1841-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1841-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c1841-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1841-107">Permission type</span></span>|<span data-ttu-id="c1841-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1841-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1841-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1841-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c1841-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1841-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1841-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1841-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1841-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1841-112">Not supported.</span></span>|
|<span data-ttu-id="c1841-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1841-113">Application</span></span>|<span data-ttu-id="c1841-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1841-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1841-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1841-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c1841-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1841-116">Request headers</span></span>
|<span data-ttu-id="c1841-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c1841-117">Header</span></span>|<span data-ttu-id="c1841-118">Wert</span><span class="sxs-lookup"><span data-stu-id="c1841-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1841-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1841-119">Authorization</span></span>|<span data-ttu-id="c1841-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1841-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1841-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c1841-121">Accept</span></span>|<span data-ttu-id="c1841-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c1841-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1841-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1841-123">Request body</span></span>
<span data-ttu-id="c1841-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="c1841-124">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="c1841-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="c1841-125">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="c1841-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c1841-126">Property</span></span>|<span data-ttu-id="c1841-127">Typ</span><span class="sxs-lookup"><span data-stu-id="c1841-127">Type</span></span>|<span data-ttu-id="c1841-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1841-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1841-129">id</span><span class="sxs-lookup"><span data-stu-id="c1841-129">id</span></span>|<span data-ttu-id="c1841-130">String</span><span class="sxs-lookup"><span data-stu-id="c1841-130">String</span></span>|<span data-ttu-id="c1841-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="c1841-131">Key of the entity.</span></span> <span data-ttu-id="c1841-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1841-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1841-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1841-133">lastModifiedDateTime</span></span>|<span data-ttu-id="c1841-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1841-134">DateTimeOffset</span></span>|<span data-ttu-id="c1841-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1841-135">DateTime the object was last modified.</span></span> <span data-ttu-id="c1841-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1841-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1841-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1841-137">createdDateTime</span></span>|<span data-ttu-id="c1841-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1841-138">DateTimeOffset</span></span>|<span data-ttu-id="c1841-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1841-139">DateTime the object was created.</span></span> <span data-ttu-id="c1841-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1841-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1841-141">description</span><span class="sxs-lookup"><span data-stu-id="c1841-141">description</span></span>|<span data-ttu-id="c1841-142">String</span><span class="sxs-lookup"><span data-stu-id="c1841-142">String</span></span>|<span data-ttu-id="c1841-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c1841-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c1841-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1841-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1841-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c1841-145">displayName</span></span>|<span data-ttu-id="c1841-146">String</span><span class="sxs-lookup"><span data-stu-id="c1841-146">String</span></span>|<span data-ttu-id="c1841-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="c1841-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c1841-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1841-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1841-149">version</span><span class="sxs-lookup"><span data-stu-id="c1841-149">version</span></span>|<span data-ttu-id="c1841-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c1841-150">Int32</span></span>|<span data-ttu-id="c1841-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="c1841-151">Version of the device configuration.</span></span> <span data-ttu-id="c1841-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1841-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1841-153">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="c1841-153">appsBlockClipboardSharing</span></span>|<span data-ttu-id="c1841-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-154">Boolean</span></span>|<span data-ttu-id="c1841-155">Gibt an, ob die gemeinsame Nutzung der Zwischenablage zum Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-155">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="c1841-156">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="c1841-156">appsBlockCopyPaste</span></span>|<span data-ttu-id="c1841-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-157">Boolean</span></span>|<span data-ttu-id="c1841-158">Gibt an, ob Kopieren und Einfügen zwischen Anwendungen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-158">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="c1841-159">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="c1841-159">appsBlockYouTube</span></span>|<span data-ttu-id="c1841-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-160">Boolean</span></span>|<span data-ttu-id="c1841-161">Gibt an, ob die YouTube-App blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-161">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="c1841-162">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="c1841-162">bluetoothBlocked</span></span>|<span data-ttu-id="c1841-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-163">Boolean</span></span>|<span data-ttu-id="c1841-164">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-164">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="c1841-165">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c1841-165">cameraBlocked</span></span>|<span data-ttu-id="c1841-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-166">Boolean</span></span>|<span data-ttu-id="c1841-167">Gibt an, ob die Verwendung der Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-167">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="c1841-168">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="c1841-168">cellularBlockDataRoaming</span></span>|<span data-ttu-id="c1841-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-169">Boolean</span></span>|<span data-ttu-id="c1841-170">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-170">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="c1841-171">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="c1841-171">cellularBlockMessaging</span></span>|<span data-ttu-id="c1841-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-172">Boolean</span></span>|<span data-ttu-id="c1841-173">Gibt an, ob SMS-/MMS-Nachrichten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c1841-173">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="c1841-174">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="c1841-174">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="c1841-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-175">Boolean</span></span>|<span data-ttu-id="c1841-176">Gibt an, ob Sprachroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-176">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="c1841-177">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="c1841-177">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="c1841-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-178">Boolean</span></span>|<span data-ttu-id="c1841-179">Gibt an, ob die Synchronisierung von WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-179">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="c1841-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="c1841-180">compliantAppsList</span></span>|<span data-ttu-id="c1841-181">Collection von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c1841-181">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="c1841-182">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="c1841-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="c1841-183">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1841-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c1841-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="c1841-184">compliantAppListType</span></span>|[<span data-ttu-id="c1841-185">appListType</span><span class="sxs-lookup"><span data-stu-id="c1841-185">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="c1841-186">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="c1841-186">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="c1841-187">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="c1841-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c1841-188">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="c1841-188">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="c1841-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-189">Boolean</span></span>|<span data-ttu-id="c1841-190">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-190">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="c1841-191">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="c1841-191">locationServicesBlocked</span></span>|<span data-ttu-id="c1841-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-192">Boolean</span></span>|<span data-ttu-id="c1841-193">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c1841-193">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="c1841-194">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="c1841-194">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="c1841-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-195">Boolean</span></span>|<span data-ttu-id="c1841-196">Gibt an, ob die automatische Synchronisierung von Google-Konten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-196">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="c1841-197">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="c1841-197">googlePlayStoreBlocked</span></span>|<span data-ttu-id="c1841-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-198">Boolean</span></span>|<span data-ttu-id="c1841-199">Gibt an, ob der Google Play-Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-199">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="c1841-200">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="c1841-200">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="c1841-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-201">Boolean</span></span>|<span data-ttu-id="c1841-202">Gibt an, ob die Standbytaste im Kioskmodus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-202">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="c1841-203">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="c1841-203">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="c1841-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-204">Boolean</span></span>|<span data-ttu-id="c1841-205">Gibt an, ob die Lautstärkeregler im Kioskmodus blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c1841-205">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="c1841-206">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="c1841-206">kioskModeApps</span></span>|<span data-ttu-id="c1841-207">Collection von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c1841-207">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="c1841-208">Eine Liste der Apps, die ausgeführt werden können, wenn sich das Gerät im Kioskmodus befindet.</span><span class="sxs-lookup"><span data-stu-id="c1841-208">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="c1841-209">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1841-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c1841-210">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="c1841-210">nfcBlocked</span></span>|<span data-ttu-id="c1841-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-211">Boolean</span></span>|<span data-ttu-id="c1841-212">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-212">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="c1841-213">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="c1841-213">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="c1841-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-214">Boolean</span></span>|<span data-ttu-id="c1841-215">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-215">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="c1841-216">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="c1841-216">passwordBlockTrustAgents</span></span>|<span data-ttu-id="c1841-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-217">Boolean</span></span>|<span data-ttu-id="c1841-218">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c1841-218">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="c1841-219">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c1841-219">passwordExpirationDays</span></span>|<span data-ttu-id="c1841-220">Int32</span><span class="sxs-lookup"><span data-stu-id="c1841-220">Int32</span></span>|<span data-ttu-id="c1841-221">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="c1841-221">Number of days before the password expires.</span></span> <span data-ttu-id="c1841-222">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="c1841-222">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c1841-223">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c1841-223">passwordMinimumLength</span></span>|<span data-ttu-id="c1841-224">Int32</span><span class="sxs-lookup"><span data-stu-id="c1841-224">Int32</span></span>|<span data-ttu-id="c1841-225">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="c1841-225">Minimum length of passwords.</span></span> <span data-ttu-id="c1841-226">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="c1841-226">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c1841-227">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c1841-227">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c1841-228">Int32</span><span class="sxs-lookup"><span data-stu-id="c1841-228">Int32</span></span>|<span data-ttu-id="c1841-229">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="c1841-229">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c1841-230">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c1841-230">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c1841-231">Int32</span><span class="sxs-lookup"><span data-stu-id="c1841-231">Int32</span></span>|<span data-ttu-id="c1841-232">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="c1841-232">Number of previous passwords to block.</span></span> <span data-ttu-id="c1841-233">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="c1841-233">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c1841-234">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c1841-234">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c1841-235">Int32</span><span class="sxs-lookup"><span data-stu-id="c1841-235">Int32</span></span>|<span data-ttu-id="c1841-236">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="c1841-236">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="c1841-237">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="c1841-237">Valid values 4 to 11</span></span>|
|<span data-ttu-id="c1841-238">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c1841-238">passwordRequiredType</span></span>|[<span data-ttu-id="c1841-239">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c1841-239">androidRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|<span data-ttu-id="c1841-240">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="c1841-240">Type of password that is required.</span></span> <span data-ttu-id="c1841-241">Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="c1841-241">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="c1841-242">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c1841-242">passwordRequired</span></span>|<span data-ttu-id="c1841-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-243">Boolean</span></span>|<span data-ttu-id="c1841-244">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c1841-244">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="c1841-245">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="c1841-245">powerOffBlocked</span></span>|<span data-ttu-id="c1841-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-246">Boolean</span></span>|<span data-ttu-id="c1841-247">Gibt an, ob das Ausschalten des Geräts blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-247">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="c1841-248">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="c1841-248">factoryResetBlocked</span></span>|<span data-ttu-id="c1841-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-249">Boolean</span></span>|<span data-ttu-id="c1841-250">Gibt an, ob verhindert werden soll, dass der Benutzer eine Zurücksetzung auf die Werkseinstellungen durchführt.</span><span class="sxs-lookup"><span data-stu-id="c1841-250">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="c1841-251">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="c1841-251">screenCaptureBlocked</span></span>|<span data-ttu-id="c1841-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-252">Boolean</span></span>|<span data-ttu-id="c1841-253">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c1841-253">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="c1841-254">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="c1841-254">deviceSharingAllowed</span></span>|<span data-ttu-id="c1841-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-255">Boolean</span></span>|<span data-ttu-id="c1841-256">Gibt an, ob der Gerätefreigabemodus zugelassen wird.</span><span class="sxs-lookup"><span data-stu-id="c1841-256">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="c1841-257">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="c1841-257">storageBlockGoogleBackup</span></span>|<span data-ttu-id="c1841-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-258">Boolean</span></span>|<span data-ttu-id="c1841-259">Gibt an, ob die Google-Sicherung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-259">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="c1841-260">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="c1841-260">storageBlockRemovableStorage</span></span>|<span data-ttu-id="c1841-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-261">Boolean</span></span>|<span data-ttu-id="c1841-262">Gibt an, ob die Verwendung von Wechselmedien blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-262">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="c1841-263">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="c1841-263">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="c1841-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-264">Boolean</span></span>|<span data-ttu-id="c1841-265">Gibt an, ob eine Geräteverschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c1841-265">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="c1841-266">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="c1841-266">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="c1841-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-267">Boolean</span></span>|<span data-ttu-id="c1841-268">Gibt an, ob die Verschlüsselung von Wechselmedien erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="c1841-268">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="c1841-269">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="c1841-269">voiceAssistantBlocked</span></span>|<span data-ttu-id="c1841-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-270">Boolean</span></span>|<span data-ttu-id="c1841-271">Gibt an, ob die Verwendung des Sprach-Assistenten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-271">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="c1841-272">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="c1841-272">voiceDialingBlocked</span></span>|<span data-ttu-id="c1841-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-273">Boolean</span></span>|<span data-ttu-id="c1841-274">Gibt an, ob das Sprachwahlverfahren blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-274">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="c1841-275">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="c1841-275">webBrowserBlockPopups</span></span>|<span data-ttu-id="c1841-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-276">Boolean</span></span>|<span data-ttu-id="c1841-277">Gibt an, ob Popups innerhalb des Webbrowsers blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c1841-277">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="c1841-278">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="c1841-278">webBrowserBlockAutofill</span></span>|<span data-ttu-id="c1841-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-279">Boolean</span></span>|<span data-ttu-id="c1841-280">Gibt an, ob das AutoAusfüllen-Feature des Webbrowsers blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-280">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="c1841-281">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="c1841-281">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="c1841-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-282">Boolean</span></span>|<span data-ttu-id="c1841-283">Gibt an, ob JavaScript im Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-283">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="c1841-284">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="c1841-284">webBrowserBlocked</span></span>|<span data-ttu-id="c1841-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-285">Boolean</span></span>|<span data-ttu-id="c1841-286">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-286">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="c1841-287">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="c1841-287">webBrowserCookieSettings</span></span>|[<span data-ttu-id="c1841-288">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="c1841-288">webBrowserCookieSettings</span></span>](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|<span data-ttu-id="c1841-289">Cookieeinstellungen des Webbrowsers.</span><span class="sxs-lookup"><span data-stu-id="c1841-289">Cookie settings within the web browser.</span></span> <span data-ttu-id="c1841-290">Mögliche Werte sind: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited` und `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="c1841-290">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="c1841-291">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="c1841-291">wiFiBlocked</span></span>|<span data-ttu-id="c1841-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-292">Boolean</span></span>|<span data-ttu-id="c1841-293">Gibt an, ob die WLAN-Synchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1841-293">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="c1841-294">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="c1841-294">appsInstallAllowList</span></span>|<span data-ttu-id="c1841-295">Collection von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c1841-295">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="c1841-296">Liste von Apps, die auf dem KNOX-Gerät installiert werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="c1841-296">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="c1841-297">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1841-297">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c1841-298">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="c1841-298">appsLaunchBlockList</span></span>|<span data-ttu-id="c1841-299">Collection von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c1841-299">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="c1841-300">Liste von Apps, die auf dem KNOX-Gerät nicht gestartet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="c1841-300">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="c1841-301">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1841-301">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c1841-302">appsHideList</span><span class="sxs-lookup"><span data-stu-id="c1841-302">appsHideList</span></span>|<span data-ttu-id="c1841-303">Collection von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c1841-303">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="c1841-304">Liste von Apps, die auf dem KNOX-Gerät ausgeblendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="c1841-304">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="c1841-305">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="c1841-305">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c1841-306">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c1841-306">securityRequireVerifyApps</span></span>|<span data-ttu-id="c1841-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1841-307">Boolean</span></span>|<span data-ttu-id="c1841-308">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="c1841-308">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="c1841-309">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1841-309">Response</span></span>
<span data-ttu-id="c1841-310">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c1841-310">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1841-311">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1841-311">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1841-312">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1841-312">Request</span></span>
<span data-ttu-id="c1841-313">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1841-313">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1841-314">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1841-314">Response</span></span>
<span data-ttu-id="c1841-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1841-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



