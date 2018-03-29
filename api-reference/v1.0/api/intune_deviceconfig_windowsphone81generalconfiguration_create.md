# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="84b83-101">Erstellen von „windowsPhone81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="84b83-101">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="84b83-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="84b83-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84b83-103">Diese Methode erstellt ein neues Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84b83-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84b83-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="84b83-104">Prerequisites</span></span>
<span data-ttu-id="84b83-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="84b83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="84b83-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="84b83-107">Permission type</span></span>|<span data-ttu-id="84b83-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="84b83-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84b83-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="84b83-109">Delegated (work or school account)</span></span>|<span data-ttu-id="84b83-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84b83-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84b83-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="84b83-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84b83-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84b83-112">Not supported.</span></span>|
|<span data-ttu-id="84b83-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="84b83-113">Application</span></span>|<span data-ttu-id="84b83-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84b83-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84b83-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="84b83-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="84b83-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="84b83-116">Request headers</span></span>
|<span data-ttu-id="84b83-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="84b83-117">Header</span></span>|<span data-ttu-id="84b83-118">Wert</span><span class="sxs-lookup"><span data-stu-id="84b83-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84b83-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="84b83-119">Authorization</span></span>|<span data-ttu-id="84b83-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="84b83-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="84b83-121">Accept</span><span class="sxs-lookup"><span data-stu-id="84b83-121">Accept</span></span>|<span data-ttu-id="84b83-122">application/json</span><span class="sxs-lookup"><span data-stu-id="84b83-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84b83-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="84b83-123">Request body</span></span>
<span data-ttu-id="84b83-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsPhone81GeneralConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="84b83-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="84b83-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsPhone81GeneralConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="84b83-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="84b83-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="84b83-126">Property</span></span>|<span data-ttu-id="84b83-127">Typ</span><span class="sxs-lookup"><span data-stu-id="84b83-127">Type</span></span>|<span data-ttu-id="84b83-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84b83-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84b83-129">id</span><span class="sxs-lookup"><span data-stu-id="84b83-129">id</span></span>|<span data-ttu-id="84b83-130">String</span><span class="sxs-lookup"><span data-stu-id="84b83-130">String</span></span>|<span data-ttu-id="84b83-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="84b83-131">Key of the setting.</span></span> <span data-ttu-id="84b83-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84b83-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84b83-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84b83-133">lastModifiedDateTime</span></span>|<span data-ttu-id="84b83-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84b83-134">DateTimeOffset</span></span>|<span data-ttu-id="84b83-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="84b83-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="84b83-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84b83-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84b83-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84b83-137">createdDateTime</span></span>|<span data-ttu-id="84b83-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84b83-138">DateTimeOffset</span></span>|<span data-ttu-id="84b83-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="84b83-139">DateTime the object was created.</span></span> <span data-ttu-id="84b83-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84b83-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84b83-141">description</span><span class="sxs-lookup"><span data-stu-id="84b83-141">description</span></span>|<span data-ttu-id="84b83-142">String</span><span class="sxs-lookup"><span data-stu-id="84b83-142">String</span></span>|<span data-ttu-id="84b83-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="84b83-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="84b83-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84b83-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84b83-145">displayName</span><span class="sxs-lookup"><span data-stu-id="84b83-145">displayName</span></span>|<span data-ttu-id="84b83-146">String</span><span class="sxs-lookup"><span data-stu-id="84b83-146">String</span></span>|<span data-ttu-id="84b83-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="84b83-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="84b83-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84b83-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84b83-149">version</span><span class="sxs-lookup"><span data-stu-id="84b83-149">version</span></span>|<span data-ttu-id="84b83-150">Int32</span><span class="sxs-lookup"><span data-stu-id="84b83-150">Int32</span></span>|<span data-ttu-id="84b83-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="84b83-151">Version of the device configuration.</span></span> <span data-ttu-id="84b83-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="84b83-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84b83-153">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="84b83-153">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="84b83-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-154">Boolean</span></span>|<span data-ttu-id="84b83-155">Wert, der angibt, ob die Richtlinie nur für Windows Phone 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="84b83-155">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="84b83-156">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="84b83-156">This property is read-only.</span></span>|
|<span data-ttu-id="84b83-157">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="84b83-157">appsBlockCopyPaste</span></span>|<span data-ttu-id="84b83-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-158">Boolean</span></span>|<span data-ttu-id="84b83-159">Gibt an, ob Kopieren/Einfügen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="84b83-159">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="84b83-160">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="84b83-160">bluetoothBlocked</span></span>|<span data-ttu-id="84b83-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-161">Boolean</span></span>|<span data-ttu-id="84b83-162">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="84b83-162">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="84b83-163">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="84b83-163">cameraBlocked</span></span>|<span data-ttu-id="84b83-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-164">Boolean</span></span>|<span data-ttu-id="84b83-165">Gibt an, ob die Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="84b83-165">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="84b83-166">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="84b83-166">cellularBlockWifiTethering</span></span>|<span data-ttu-id="84b83-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-167">Boolean</span></span>|<span data-ttu-id="84b83-168">Gibt an, ob WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="84b83-168">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="84b83-169">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="84b83-169">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="84b83-170">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="84b83-170">compliantAppsList</span></span>|<span data-ttu-id="84b83-171">Collection von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="84b83-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="84b83-172">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="84b83-172">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="84b83-173">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="84b83-173">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="84b83-174">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="84b83-174">compliantAppListType</span></span>|<span data-ttu-id="84b83-175">String</span><span class="sxs-lookup"><span data-stu-id="84b83-175">String</span></span>|<span data-ttu-id="84b83-176">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="84b83-176">List that is in the AppComplianceList.</span></span> <span data-ttu-id="84b83-177">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="84b83-177">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="84b83-178">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="84b83-178">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="84b83-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-179">Boolean</span></span>|<span data-ttu-id="84b83-180">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="84b83-180">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="84b83-181">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="84b83-181">emailBlockAddingAccounts</span></span>|<span data-ttu-id="84b83-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-182">Boolean</span></span>|<span data-ttu-id="84b83-183">Gibt an, ob benutzerdefinierte E-Mail-Konten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="84b83-183">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="84b83-184">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="84b83-184">locationServicesBlocked</span></span>|<span data-ttu-id="84b83-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-185">Boolean</span></span>|<span data-ttu-id="84b83-186">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="84b83-186">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="84b83-187">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="84b83-187">microsoftAccountBlocked</span></span>|<span data-ttu-id="84b83-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-188">Boolean</span></span>|<span data-ttu-id="84b83-189">Gibt an, ob die Verwendung eines Microsoft-Kontos erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="84b83-189">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="84b83-190">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="84b83-190">nfcBlocked</span></span>|<span data-ttu-id="84b83-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-191">Boolean</span></span>|<span data-ttu-id="84b83-192">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="84b83-192">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="84b83-193">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="84b83-193">passwordBlockSimple</span></span>|<span data-ttu-id="84b83-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-194">Boolean</span></span>|<span data-ttu-id="84b83-195">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="84b83-195">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="84b83-196">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="84b83-196">passwordExpirationDays</span></span>|<span data-ttu-id="84b83-197">Int32</span><span class="sxs-lookup"><span data-stu-id="84b83-197">Int32</span></span>|<span data-ttu-id="84b83-198">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="84b83-198">Number of days before the password expires.</span></span>|
|<span data-ttu-id="84b83-199">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="84b83-199">passwordMinimumLength</span></span>|<span data-ttu-id="84b83-200">Int32</span><span class="sxs-lookup"><span data-stu-id="84b83-200">Int32</span></span>|<span data-ttu-id="84b83-201">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="84b83-201">Minimum length of passwords.</span></span>|
|<span data-ttu-id="84b83-202">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="84b83-202">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="84b83-203">Int32</span><span class="sxs-lookup"><span data-stu-id="84b83-203">Int32</span></span>|<span data-ttu-id="84b83-204">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="84b83-204">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="84b83-205">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="84b83-205">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="84b83-206">Int32</span><span class="sxs-lookup"><span data-stu-id="84b83-206">Int32</span></span>|<span data-ttu-id="84b83-207">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss</span><span class="sxs-lookup"><span data-stu-id="84b83-207">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="84b83-208">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="84b83-208">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="84b83-209">Int32</span><span class="sxs-lookup"><span data-stu-id="84b83-209">Int32</span></span>|<span data-ttu-id="84b83-210">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="84b83-210">Number of previous passwords to block.</span></span> <span data-ttu-id="84b83-211">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="84b83-211">Valid values 0 to 24</span></span>|
|<span data-ttu-id="84b83-212">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="84b83-212">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="84b83-213">Int32</span><span class="sxs-lookup"><span data-stu-id="84b83-213">Int32</span></span>|<span data-ttu-id="84b83-214">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="84b83-214">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="84b83-215">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="84b83-215">passwordRequiredType</span></span>|<span data-ttu-id="84b83-216">String</span><span class="sxs-lookup"><span data-stu-id="84b83-216">String</span></span>|<span data-ttu-id="84b83-217">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="84b83-217">Password type that is required.</span></span> <span data-ttu-id="84b83-218">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="84b83-218">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="84b83-219">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="84b83-219">passwordRequired</span></span>|<span data-ttu-id="84b83-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-220">Boolean</span></span>|<span data-ttu-id="84b83-221">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="84b83-221">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="84b83-222">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="84b83-222">screenCaptureBlocked</span></span>|<span data-ttu-id="84b83-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-223">Boolean</span></span>|<span data-ttu-id="84b83-224">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="84b83-224">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="84b83-225">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="84b83-225">storageBlockRemovableStorage</span></span>|<span data-ttu-id="84b83-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-226">Boolean</span></span>|<span data-ttu-id="84b83-227">Gibt an, ob Wechselmedien blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="84b83-227">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="84b83-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="84b83-228">storageRequireEncryption</span></span>|<span data-ttu-id="84b83-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-229">Boolean</span></span>|<span data-ttu-id="84b83-230">Gibt an, ob Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="84b83-230">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="84b83-231">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="84b83-231">webBrowserBlocked</span></span>|<span data-ttu-id="84b83-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-232">Boolean</span></span>|<span data-ttu-id="84b83-233">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="84b83-233">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="84b83-234">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="84b83-234">wifiBlocked</span></span>|<span data-ttu-id="84b83-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-235">Boolean</span></span>|<span data-ttu-id="84b83-236">Gibt an, ob die WLAN-Funktion blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="84b83-236">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="84b83-237">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="84b83-237">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="84b83-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-238">Boolean</span></span>|<span data-ttu-id="84b83-239">Gibt an, ob die automatische Herstellung einer Verbindung zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="84b83-239">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="84b83-240">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="84b83-240">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="84b83-241">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="84b83-241">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="84b83-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-242">Boolean</span></span>|<span data-ttu-id="84b83-243">Gibt an, ob die Erstellung von Berichten zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="84b83-243">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="84b83-244">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="84b83-244">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="84b83-245">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="84b83-245">windowsStoreBlocked</span></span>|<span data-ttu-id="84b83-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b83-246">Boolean</span></span>|<span data-ttu-id="84b83-247">Gibt an, ob der Windows Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="84b83-247">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="84b83-248">Antwort</span><span class="sxs-lookup"><span data-stu-id="84b83-248">Response</span></span>
<span data-ttu-id="84b83-249">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="84b83-249">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84b83-250">Beispiel</span><span class="sxs-lookup"><span data-stu-id="84b83-250">Example</span></span>
### <a name="request"></a><span data-ttu-id="84b83-251">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84b83-251">Request</span></span>
<span data-ttu-id="84b83-252">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="84b83-252">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1525

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="84b83-253">Antwort</span><span class="sxs-lookup"><span data-stu-id="84b83-253">Response</span></span>
<span data-ttu-id="84b83-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="84b83-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



