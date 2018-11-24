# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="1b16b-101">Erstellen von „windowsPhone81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="1b16b-101">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="1b16b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1b16b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b16b-103">Diese Methode erstellt ein neues Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b16b-103">Create a new [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b16b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1b16b-104">Prerequisites</span></span>
<span data-ttu-id="1b16b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1b16b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1b16b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1b16b-107">Permission type</span></span>|<span data-ttu-id="1b16b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1b16b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b16b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1b16b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1b16b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b16b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b16b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1b16b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b16b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b16b-112">Not supported.</span></span>|
|<span data-ttu-id="1b16b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1b16b-113">Application</span></span>|<span data-ttu-id="1b16b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b16b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b16b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b16b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1b16b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1b16b-116">Request headers</span></span>
|<span data-ttu-id="1b16b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1b16b-117">Header</span></span>|<span data-ttu-id="1b16b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="1b16b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b16b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b16b-119">Authorization</span></span>|<span data-ttu-id="1b16b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1b16b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b16b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1b16b-121">Accept</span></span>|<span data-ttu-id="1b16b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1b16b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b16b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1b16b-123">Request body</span></span>
<span data-ttu-id="1b16b-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsPhone81GeneralConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="1b16b-124">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="1b16b-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsPhone81GeneralConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="1b16b-125">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="1b16b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1b16b-126">Property</span></span>|<span data-ttu-id="1b16b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="1b16b-127">Type</span></span>|<span data-ttu-id="1b16b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b16b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b16b-129">id</span><span class="sxs-lookup"><span data-stu-id="1b16b-129">id</span></span>|<span data-ttu-id="1b16b-130">String</span><span class="sxs-lookup"><span data-stu-id="1b16b-130">String</span></span>|<span data-ttu-id="1b16b-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="1b16b-131">Key of the entity.</span></span> <span data-ttu-id="1b16b-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b16b-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b16b-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b16b-133">lastModifiedDateTime</span></span>|<span data-ttu-id="1b16b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b16b-134">DateTimeOffset</span></span>|<span data-ttu-id="1b16b-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1b16b-135">DateTime the object was last modified.</span></span> <span data-ttu-id="1b16b-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b16b-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b16b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b16b-137">createdDateTime</span></span>|<span data-ttu-id="1b16b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b16b-138">DateTimeOffset</span></span>|<span data-ttu-id="1b16b-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1b16b-139">DateTime the object was created.</span></span> <span data-ttu-id="1b16b-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b16b-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b16b-141">description</span><span class="sxs-lookup"><span data-stu-id="1b16b-141">description</span></span>|<span data-ttu-id="1b16b-142">String</span><span class="sxs-lookup"><span data-stu-id="1b16b-142">String</span></span>|<span data-ttu-id="1b16b-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1b16b-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1b16b-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b16b-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b16b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="1b16b-145">displayName</span></span>|<span data-ttu-id="1b16b-146">String</span><span class="sxs-lookup"><span data-stu-id="1b16b-146">String</span></span>|<span data-ttu-id="1b16b-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1b16b-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1b16b-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b16b-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b16b-149">version</span><span class="sxs-lookup"><span data-stu-id="1b16b-149">version</span></span>|<span data-ttu-id="1b16b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1b16b-150">Int32</span></span>|<span data-ttu-id="1b16b-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="1b16b-151">Version of the device configuration.</span></span> <span data-ttu-id="1b16b-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b16b-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b16b-153">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="1b16b-153">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="1b16b-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-154">Boolean</span></span>|<span data-ttu-id="1b16b-155">Wert, der angibt, ob die Richtlinie nur für Windows Phone 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="1b16b-155">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="1b16b-156">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1b16b-156">This property is read-only.</span></span>|
|<span data-ttu-id="1b16b-157">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="1b16b-157">appsBlockCopyPaste</span></span>|<span data-ttu-id="1b16b-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-158">Boolean</span></span>|<span data-ttu-id="1b16b-159">Gibt an, ob Kopieren/Einfügen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b16b-159">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="1b16b-160">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="1b16b-160">bluetoothBlocked</span></span>|<span data-ttu-id="1b16b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-161">Boolean</span></span>|<span data-ttu-id="1b16b-162">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b16b-162">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="1b16b-163">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="1b16b-163">cameraBlocked</span></span>|<span data-ttu-id="1b16b-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-164">Boolean</span></span>|<span data-ttu-id="1b16b-165">Gibt an, ob die Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b16b-165">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="1b16b-166">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="1b16b-166">cellularBlockWifiTethering</span></span>|<span data-ttu-id="1b16b-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-167">Boolean</span></span>|<span data-ttu-id="1b16b-168">Gibt an, ob WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b16b-168">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="1b16b-169">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="1b16b-169">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="1b16b-170">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="1b16b-170">compliantAppsList</span></span>|<span data-ttu-id="1b16b-171">Collection von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1b16b-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="1b16b-172">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="1b16b-172">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="1b16b-173">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="1b16b-173">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="1b16b-174">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="1b16b-174">compliantAppListType</span></span>|[<span data-ttu-id="1b16b-175">appListType</span><span class="sxs-lookup"><span data-stu-id="1b16b-175">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="1b16b-176">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="1b16b-176">List that is in the AppComplianceList.</span></span> <span data-ttu-id="1b16b-177">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="1b16b-177">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="1b16b-178">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="1b16b-178">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="1b16b-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-179">Boolean</span></span>|<span data-ttu-id="1b16b-180">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b16b-180">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="1b16b-181">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="1b16b-181">emailBlockAddingAccounts</span></span>|<span data-ttu-id="1b16b-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-182">Boolean</span></span>|<span data-ttu-id="1b16b-183">Gibt an, ob benutzerdefinierte E-Mail-Konten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="1b16b-183">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="1b16b-184">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="1b16b-184">locationServicesBlocked</span></span>|<span data-ttu-id="1b16b-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-185">Boolean</span></span>|<span data-ttu-id="1b16b-186">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="1b16b-186">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="1b16b-187">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="1b16b-187">microsoftAccountBlocked</span></span>|<span data-ttu-id="1b16b-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-188">Boolean</span></span>|<span data-ttu-id="1b16b-189">Gibt an, ob die Verwendung eines Microsoft-Kontos erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="1b16b-189">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="1b16b-190">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="1b16b-190">nfcBlocked</span></span>|<span data-ttu-id="1b16b-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-191">Boolean</span></span>|<span data-ttu-id="1b16b-192">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b16b-192">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="1b16b-193">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="1b16b-193">passwordBlockSimple</span></span>|<span data-ttu-id="1b16b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-194">Boolean</span></span>|<span data-ttu-id="1b16b-195">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b16b-195">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="1b16b-196">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1b16b-196">passwordExpirationDays</span></span>|<span data-ttu-id="1b16b-197">Int32</span><span class="sxs-lookup"><span data-stu-id="1b16b-197">Int32</span></span>|<span data-ttu-id="1b16b-198">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="1b16b-198">Number of days before the password expires.</span></span>|
|<span data-ttu-id="1b16b-199">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1b16b-199">passwordMinimumLength</span></span>|<span data-ttu-id="1b16b-200">Int32</span><span class="sxs-lookup"><span data-stu-id="1b16b-200">Int32</span></span>|<span data-ttu-id="1b16b-201">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="1b16b-201">Minimum length of passwords.</span></span>|
|<span data-ttu-id="1b16b-202">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1b16b-202">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1b16b-203">Int32</span><span class="sxs-lookup"><span data-stu-id="1b16b-203">Int32</span></span>|<span data-ttu-id="1b16b-204">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="1b16b-204">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="1b16b-205">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="1b16b-205">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="1b16b-206">Int32</span><span class="sxs-lookup"><span data-stu-id="1b16b-206">Int32</span></span>|<span data-ttu-id="1b16b-207">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss</span><span class="sxs-lookup"><span data-stu-id="1b16b-207">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="1b16b-208">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1b16b-208">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1b16b-209">Int32</span><span class="sxs-lookup"><span data-stu-id="1b16b-209">Int32</span></span>|<span data-ttu-id="1b16b-210">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="1b16b-210">Number of previous passwords to block.</span></span> <span data-ttu-id="1b16b-211">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="1b16b-211">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1b16b-212">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1b16b-212">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1b16b-213">Int32</span><span class="sxs-lookup"><span data-stu-id="1b16b-213">Int32</span></span>|<span data-ttu-id="1b16b-214">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="1b16b-214">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="1b16b-215">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1b16b-215">passwordRequiredType</span></span>|[<span data-ttu-id="1b16b-216">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1b16b-216">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="1b16b-217">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="1b16b-217">Password type that is required.</span></span> <span data-ttu-id="1b16b-218">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="1b16b-218">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="1b16b-219">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="1b16b-219">passwordRequired</span></span>|<span data-ttu-id="1b16b-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-220">Boolean</span></span>|<span data-ttu-id="1b16b-221">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="1b16b-221">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="1b16b-222">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="1b16b-222">screenCaptureBlocked</span></span>|<span data-ttu-id="1b16b-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-223">Boolean</span></span>|<span data-ttu-id="1b16b-224">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="1b16b-224">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="1b16b-225">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="1b16b-225">storageBlockRemovableStorage</span></span>|<span data-ttu-id="1b16b-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-226">Boolean</span></span>|<span data-ttu-id="1b16b-227">Gibt an, ob Wechselmedien blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="1b16b-227">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="1b16b-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="1b16b-228">storageRequireEncryption</span></span>|<span data-ttu-id="1b16b-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-229">Boolean</span></span>|<span data-ttu-id="1b16b-230">Gibt an, ob Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="1b16b-230">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="1b16b-231">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="1b16b-231">webBrowserBlocked</span></span>|<span data-ttu-id="1b16b-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-232">Boolean</span></span>|<span data-ttu-id="1b16b-233">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b16b-233">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="1b16b-234">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="1b16b-234">wifiBlocked</span></span>|<span data-ttu-id="1b16b-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-235">Boolean</span></span>|<span data-ttu-id="1b16b-236">Gibt an, ob die WLAN-Funktion blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b16b-236">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="1b16b-237">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="1b16b-237">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="1b16b-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-238">Boolean</span></span>|<span data-ttu-id="1b16b-239">Gibt an, ob die automatische Herstellung einer Verbindung zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b16b-239">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="1b16b-240">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="1b16b-240">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="1b16b-241">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="1b16b-241">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="1b16b-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-242">Boolean</span></span>|<span data-ttu-id="1b16b-243">Gibt an, ob die Erstellung von Berichten zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b16b-243">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="1b16b-244">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="1b16b-244">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="1b16b-245">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="1b16b-245">windowsStoreBlocked</span></span>|<span data-ttu-id="1b16b-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b16b-246">Boolean</span></span>|<span data-ttu-id="1b16b-247">Gibt an, ob der Windows Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b16b-247">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="1b16b-248">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b16b-248">Response</span></span>
<span data-ttu-id="1b16b-249">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1b16b-249">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b16b-250">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1b16b-250">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b16b-251">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b16b-251">Request</span></span>
<span data-ttu-id="1b16b-252">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1b16b-252">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="1b16b-253">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b16b-253">Response</span></span>
<span data-ttu-id="1b16b-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b16b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



