# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="d6093-101">Aktualisieren von „windowsPhone81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="d6093-101">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="d6093-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d6093-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6093-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6093-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6093-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d6093-104">Prerequisites</span></span>
<span data-ttu-id="d6093-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d6093-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d6093-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d6093-107">Permission type</span></span>|<span data-ttu-id="d6093-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d6093-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6093-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d6093-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d6093-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6093-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6093-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d6093-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6093-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6093-112">Not supported.</span></span>|
|<span data-ttu-id="d6093-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d6093-113">Application</span></span>|<span data-ttu-id="d6093-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6093-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6093-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6093-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d6093-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d6093-116">Request headers</span></span>
|<span data-ttu-id="d6093-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d6093-117">Header</span></span>|<span data-ttu-id="d6093-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d6093-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6093-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6093-119">Authorization</span></span>|<span data-ttu-id="d6093-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d6093-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d6093-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d6093-121">Accept</span></span>|<span data-ttu-id="d6093-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d6093-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6093-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d6093-123">Request body</span></span>
<span data-ttu-id="d6093-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="d6093-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="d6093-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="d6093-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="d6093-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d6093-126">Property</span></span>|<span data-ttu-id="d6093-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d6093-127">Type</span></span>|<span data-ttu-id="d6093-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6093-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6093-129">id</span><span class="sxs-lookup"><span data-stu-id="d6093-129">id</span></span>|<span data-ttu-id="d6093-130">String</span><span class="sxs-lookup"><span data-stu-id="d6093-130">String</span></span>|<span data-ttu-id="d6093-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="d6093-131">Key of the setting.</span></span> <span data-ttu-id="d6093-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6093-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6093-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6093-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d6093-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6093-134">DateTimeOffset</span></span>|<span data-ttu-id="d6093-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d6093-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="d6093-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6093-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6093-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6093-137">createdDateTime</span></span>|<span data-ttu-id="d6093-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6093-138">DateTimeOffset</span></span>|<span data-ttu-id="d6093-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d6093-139">DateTime the object was created.</span></span> <span data-ttu-id="d6093-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6093-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6093-141">description</span><span class="sxs-lookup"><span data-stu-id="d6093-141">description</span></span>|<span data-ttu-id="d6093-142">String</span><span class="sxs-lookup"><span data-stu-id="d6093-142">String</span></span>|<span data-ttu-id="d6093-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d6093-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d6093-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6093-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6093-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d6093-145">displayName</span></span>|<span data-ttu-id="d6093-146">String</span><span class="sxs-lookup"><span data-stu-id="d6093-146">String</span></span>|<span data-ttu-id="d6093-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d6093-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d6093-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6093-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6093-149">version</span><span class="sxs-lookup"><span data-stu-id="d6093-149">version</span></span>|<span data-ttu-id="d6093-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d6093-150">Int32</span></span>|<span data-ttu-id="d6093-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d6093-151">Version of the device configuration.</span></span> <span data-ttu-id="d6093-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6093-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6093-153">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="d6093-153">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="d6093-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-154">Boolean</span></span>|<span data-ttu-id="d6093-155">Wert, der angibt, ob die Richtlinie nur für Windows Phone 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="d6093-155">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="d6093-156">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d6093-156">This property is read-only.</span></span>|
|<span data-ttu-id="d6093-157">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="d6093-157">appsBlockCopyPaste</span></span>|<span data-ttu-id="d6093-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-158">Boolean</span></span>|<span data-ttu-id="d6093-159">Gibt an, ob Kopieren/Einfügen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6093-159">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="d6093-160">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="d6093-160">bluetoothBlocked</span></span>|<span data-ttu-id="d6093-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-161">Boolean</span></span>|<span data-ttu-id="d6093-162">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6093-162">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="d6093-163">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="d6093-163">cameraBlocked</span></span>|<span data-ttu-id="d6093-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-164">Boolean</span></span>|<span data-ttu-id="d6093-165">Gibt an, ob die Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6093-165">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="d6093-166">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="d6093-166">cellularBlockWifiTethering</span></span>|<span data-ttu-id="d6093-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-167">Boolean</span></span>|<span data-ttu-id="d6093-168">Gibt an, ob WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6093-168">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="d6093-169">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="d6093-169">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="d6093-170">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="d6093-170">compliantAppsList</span></span>|<span data-ttu-id="d6093-171">Collection von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d6093-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="d6093-172">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="d6093-172">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="d6093-173">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d6093-173">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d6093-174">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="d6093-174">compliantAppListType</span></span>|<span data-ttu-id="d6093-175">String</span><span class="sxs-lookup"><span data-stu-id="d6093-175">String</span></span>|<span data-ttu-id="d6093-176">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="d6093-176">List that is in the AppComplianceList.</span></span> <span data-ttu-id="d6093-177">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="d6093-177">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d6093-178">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="d6093-178">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="d6093-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-179">Boolean</span></span>|<span data-ttu-id="d6093-180">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6093-180">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="d6093-181">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="d6093-181">emailBlockAddingAccounts</span></span>|<span data-ttu-id="d6093-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-182">Boolean</span></span>|<span data-ttu-id="d6093-183">Gibt an, ob benutzerdefinierte E-Mail-Konten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d6093-183">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="d6093-184">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="d6093-184">locationServicesBlocked</span></span>|<span data-ttu-id="d6093-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-185">Boolean</span></span>|<span data-ttu-id="d6093-186">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d6093-186">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="d6093-187">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="d6093-187">microsoftAccountBlocked</span></span>|<span data-ttu-id="d6093-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-188">Boolean</span></span>|<span data-ttu-id="d6093-189">Gibt an, ob die Verwendung eines Microsoft-Kontos erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="d6093-189">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="d6093-190">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="d6093-190">nfcBlocked</span></span>|<span data-ttu-id="d6093-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-191">Boolean</span></span>|<span data-ttu-id="d6093-192">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6093-192">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="d6093-193">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d6093-193">passwordBlockSimple</span></span>|<span data-ttu-id="d6093-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-194">Boolean</span></span>|<span data-ttu-id="d6093-195">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6093-195">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="d6093-196">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d6093-196">passwordExpirationDays</span></span>|<span data-ttu-id="d6093-197">Int32</span><span class="sxs-lookup"><span data-stu-id="d6093-197">Int32</span></span>|<span data-ttu-id="d6093-198">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="d6093-198">Number of days before the password expires.</span></span>|
|<span data-ttu-id="d6093-199">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d6093-199">passwordMinimumLength</span></span>|<span data-ttu-id="d6093-200">Int32</span><span class="sxs-lookup"><span data-stu-id="d6093-200">Int32</span></span>|<span data-ttu-id="d6093-201">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="d6093-201">Minimum length of passwords.</span></span>|
|<span data-ttu-id="d6093-202">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d6093-202">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d6093-203">Int32</span><span class="sxs-lookup"><span data-stu-id="d6093-203">Int32</span></span>|<span data-ttu-id="d6093-204">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="d6093-204">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="d6093-205">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d6093-205">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="d6093-206">Int32</span><span class="sxs-lookup"><span data-stu-id="d6093-206">Int32</span></span>|<span data-ttu-id="d6093-207">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss</span><span class="sxs-lookup"><span data-stu-id="d6093-207">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="d6093-208">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d6093-208">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d6093-209">Int32</span><span class="sxs-lookup"><span data-stu-id="d6093-209">Int32</span></span>|<span data-ttu-id="d6093-210">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="d6093-210">Number of previous passwords to block.</span></span> <span data-ttu-id="d6093-211">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="d6093-211">Valid values 0 to 24</span></span>|
|<span data-ttu-id="d6093-212">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="d6093-212">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="d6093-213">Int32</span><span class="sxs-lookup"><span data-stu-id="d6093-213">Int32</span></span>|<span data-ttu-id="d6093-214">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="d6093-214">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="d6093-215">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d6093-215">passwordRequiredType</span></span>|<span data-ttu-id="d6093-216">String</span><span class="sxs-lookup"><span data-stu-id="d6093-216">String</span></span>|<span data-ttu-id="d6093-217">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="d6093-217">Password type that is required.</span></span> <span data-ttu-id="d6093-218">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="d6093-218">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d6093-219">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="d6093-219">passwordRequired</span></span>|<span data-ttu-id="d6093-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-220">Boolean</span></span>|<span data-ttu-id="d6093-221">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d6093-221">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="d6093-222">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="d6093-222">screenCaptureBlocked</span></span>|<span data-ttu-id="d6093-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-223">Boolean</span></span>|<span data-ttu-id="d6093-224">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d6093-224">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="d6093-225">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="d6093-225">storageBlockRemovableStorage</span></span>|<span data-ttu-id="d6093-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-226">Boolean</span></span>|<span data-ttu-id="d6093-227">Gibt an, ob Wechselmedien blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d6093-227">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="d6093-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="d6093-228">storageRequireEncryption</span></span>|<span data-ttu-id="d6093-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-229">Boolean</span></span>|<span data-ttu-id="d6093-230">Gibt an, ob Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d6093-230">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="d6093-231">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="d6093-231">webBrowserBlocked</span></span>|<span data-ttu-id="d6093-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-232">Boolean</span></span>|<span data-ttu-id="d6093-233">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6093-233">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="d6093-234">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="d6093-234">wifiBlocked</span></span>|<span data-ttu-id="d6093-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-235">Boolean</span></span>|<span data-ttu-id="d6093-236">Gibt an, ob die WLAN-Funktion blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6093-236">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="d6093-237">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="d6093-237">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="d6093-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-238">Boolean</span></span>|<span data-ttu-id="d6093-239">Gibt an, ob die automatische Herstellung einer Verbindung zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6093-239">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="d6093-240">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="d6093-240">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="d6093-241">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="d6093-241">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="d6093-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-242">Boolean</span></span>|<span data-ttu-id="d6093-243">Gibt an, ob die Erstellung von Berichten zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6093-243">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="d6093-244">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="d6093-244">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="d6093-245">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d6093-245">windowsStoreBlocked</span></span>|<span data-ttu-id="d6093-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6093-246">Boolean</span></span>|<span data-ttu-id="d6093-247">Gibt an, ob der Windows Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6093-247">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="d6093-248">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6093-248">Response</span></span>
<span data-ttu-id="d6093-249">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d6093-249">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6093-250">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d6093-250">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6093-251">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6093-251">Request</span></span>
<span data-ttu-id="d6093-252">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d6093-252">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1452

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="d6093-253">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6093-253">Response</span></span>
<span data-ttu-id="d6093-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d6093-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```



