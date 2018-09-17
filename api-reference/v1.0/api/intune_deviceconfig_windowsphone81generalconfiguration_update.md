# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="f578e-101">Aktualisieren von „windowsPhone81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="f578e-101">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="f578e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f578e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f578e-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f578e-103">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f578e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f578e-104">Prerequisites</span></span>
<span data-ttu-id="f578e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f578e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f578e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f578e-107">Permission type</span></span>|<span data-ttu-id="f578e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f578e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f578e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f578e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f578e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f578e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f578e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f578e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f578e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f578e-112">Not supported.</span></span>|
|<span data-ttu-id="f578e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f578e-113">Application</span></span>|<span data-ttu-id="f578e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f578e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f578e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f578e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f578e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f578e-116">Request headers</span></span>
|<span data-ttu-id="f578e-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f578e-117">Header</span></span>|<span data-ttu-id="f578e-118">Wert</span><span class="sxs-lookup"><span data-stu-id="f578e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f578e-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f578e-119">Authorization</span></span>|<span data-ttu-id="f578e-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f578e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f578e-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="f578e-121">Accept</span></span>|<span data-ttu-id="f578e-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="f578e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f578e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f578e-123">Request body</span></span>
<span data-ttu-id="f578e-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="f578e-124">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="f578e-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f578e-125">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="f578e-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f578e-126">Property</span></span>|<span data-ttu-id="f578e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="f578e-127">Type</span></span>|<span data-ttu-id="f578e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f578e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f578e-129">ID</span><span class="sxs-lookup"><span data-stu-id="f578e-129">id</span></span>|<span data-ttu-id="f578e-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f578e-130">String</span></span>|<span data-ttu-id="f578e-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f578e-131">Key of the entity.</span></span> <span data-ttu-id="f578e-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f578e-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f578e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f578e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="f578e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f578e-134">DateTimeOffset</span></span>|<span data-ttu-id="f578e-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f578e-135">DateTime the object was last modified.</span></span> <span data-ttu-id="f578e-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f578e-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f578e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f578e-137">createdDateTime</span></span>|<span data-ttu-id="f578e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f578e-138">DateTimeOffset</span></span>|<span data-ttu-id="f578e-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="f578e-139">DateTime the object was created.</span></span> <span data-ttu-id="f578e-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f578e-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f578e-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f578e-141">description</span></span>|<span data-ttu-id="f578e-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f578e-142">String</span></span>|<span data-ttu-id="f578e-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f578e-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f578e-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f578e-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f578e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f578e-145">displayName</span></span>|<span data-ttu-id="f578e-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f578e-146">String</span></span>|<span data-ttu-id="f578e-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="f578e-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f578e-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f578e-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f578e-149">Version</span><span class="sxs-lookup"><span data-stu-id="f578e-149">version</span></span>|<span data-ttu-id="f578e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f578e-150">Int32</span></span>|<span data-ttu-id="f578e-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f578e-151">Version of the device configuration.</span></span> <span data-ttu-id="f578e-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f578e-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f578e-153">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="f578e-153">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="f578e-154">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-154">Boolean</span></span>|<span data-ttu-id="f578e-155">Wert, der angibt, ob die Richtlinie nur für Windows Phone 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="f578e-155">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="f578e-156">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f578e-156">This property is read-only.</span></span>|
|<span data-ttu-id="f578e-157">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="f578e-157">appsBlockCopyPaste</span></span>|<span data-ttu-id="f578e-158">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-158">Boolean</span></span>|<span data-ttu-id="f578e-159">Gibt an, ob Kopieren/Einfügen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f578e-159">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="f578e-160">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="f578e-160">bluetoothBlocked</span></span>|<span data-ttu-id="f578e-161">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-161">Boolean</span></span>|<span data-ttu-id="f578e-162">Gibt an, ob Bluetooth blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f578e-162">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="f578e-163">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="f578e-163">cameraBlocked</span></span>|<span data-ttu-id="f578e-164">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-164">Boolean</span></span>|<span data-ttu-id="f578e-165">Gibt an, ob die Kamera blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f578e-165">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="f578e-166">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="f578e-166">cellularBlockWifiTethering</span></span>|<span data-ttu-id="f578e-167">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-167">Boolean</span></span>|<span data-ttu-id="f578e-168">Gibt an, ob WLAN-Tethering blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f578e-168">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="f578e-169">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="f578e-169">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="f578e-170">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="f578e-170">compliantAppsList</span></span>|<span data-ttu-id="f578e-171">Collection von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f578e-171">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="f578e-172">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="f578e-172">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="f578e-173">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="f578e-173">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f578e-174">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="f578e-174">compliantAppListType</span></span>|[<span data-ttu-id="f578e-175">appListType</span><span class="sxs-lookup"><span data-stu-id="f578e-175">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="f578e-p111">Eine Liste in der AppComplianceList. Mögliche Werte: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="f578e-p111">List that is in the AppComplianceList. The possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="f578e-178">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="f578e-178">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="f578e-179">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-179">Boolean</span></span>|<span data-ttu-id="f578e-180">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f578e-180">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="f578e-181">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="f578e-181">emailBlockAddingAccounts</span></span>|<span data-ttu-id="f578e-182">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-182">Boolean</span></span>|<span data-ttu-id="f578e-183">Gibt an, ob benutzerdefinierte E-Mail-Konten blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f578e-183">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="f578e-184">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="f578e-184">locationServicesBlocked</span></span>|<span data-ttu-id="f578e-185">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-185">Boolean</span></span>|<span data-ttu-id="f578e-186">Gibt an, ob die Ortungsdienste blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f578e-186">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="f578e-187">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="f578e-187">microsoftAccountBlocked</span></span>|<span data-ttu-id="f578e-188">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-188">Boolean</span></span>|<span data-ttu-id="f578e-189">Gibt an, ob die Verwendung eines Microsoft-Kontos erlaubt ist.</span><span class="sxs-lookup"><span data-stu-id="f578e-189">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="f578e-190">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="f578e-190">nfcBlocked</span></span>|<span data-ttu-id="f578e-191">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-191">Boolean</span></span>|<span data-ttu-id="f578e-192">Gibt an, ob NFC (Near Field Communication) blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f578e-192">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="f578e-193">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f578e-193">passwordBlockSimple</span></span>|<span data-ttu-id="f578e-194">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-194">Boolean</span></span>|<span data-ttu-id="f578e-195">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f578e-195">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="f578e-196">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f578e-196">passwordExpirationDays</span></span>|<span data-ttu-id="f578e-197">Int32</span><span class="sxs-lookup"><span data-stu-id="f578e-197">Int32</span></span>|<span data-ttu-id="f578e-198">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="f578e-198">Number of days before the password expires.</span></span>|
|<span data-ttu-id="f578e-199">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f578e-199">passwordMinimumLength</span></span>|<span data-ttu-id="f578e-200">Int32</span><span class="sxs-lookup"><span data-stu-id="f578e-200">Int32</span></span>|<span data-ttu-id="f578e-201">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="f578e-201">Minimum length of passwords.</span></span>|
|<span data-ttu-id="f578e-202">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f578e-202">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f578e-203">Int32</span><span class="sxs-lookup"><span data-stu-id="f578e-203">Int32</span></span>|<span data-ttu-id="f578e-204">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="f578e-204">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="f578e-205">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f578e-205">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f578e-206">Int32</span><span class="sxs-lookup"><span data-stu-id="f578e-206">Int32</span></span>|<span data-ttu-id="f578e-207">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss</span><span class="sxs-lookup"><span data-stu-id="f578e-207">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="f578e-208">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f578e-208">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f578e-209">Int32</span><span class="sxs-lookup"><span data-stu-id="f578e-209">Int32</span></span>|<span data-ttu-id="f578e-210">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="f578e-210">Number of previous passwords to block.</span></span> <span data-ttu-id="f578e-211">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="f578e-211">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f578e-212">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f578e-212">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f578e-213">Int32</span><span class="sxs-lookup"><span data-stu-id="f578e-213">Int32</span></span>|<span data-ttu-id="f578e-214">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="f578e-214">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="f578e-215">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f578e-215">passwordRequiredType</span></span>|[<span data-ttu-id="f578e-216">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f578e-216">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="f578e-p113">Der benötigte Kennworttyp. Mögliche Werte: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f578e-p113">Password type that is required. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f578e-219">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f578e-219">passwordRequired</span></span>|<span data-ttu-id="f578e-220">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-220">Boolean</span></span>|<span data-ttu-id="f578e-221">Gibt an, ob ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="f578e-221">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="f578e-222">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="f578e-222">screenCaptureBlocked</span></span>|<span data-ttu-id="f578e-223">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-223">Boolean</span></span>|<span data-ttu-id="f578e-224">Gibt an, ob Screenshots blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f578e-224">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="f578e-225">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="f578e-225">storageBlockRemovableStorage</span></span>|<span data-ttu-id="f578e-226">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-226">Boolean</span></span>|<span data-ttu-id="f578e-227">Gibt an, ob Wechselmedien blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f578e-227">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="f578e-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f578e-228">storageRequireEncryption</span></span>|<span data-ttu-id="f578e-229">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-229">Boolean</span></span>|<span data-ttu-id="f578e-230">Gibt an, ob Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="f578e-230">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="f578e-231">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="f578e-231">webBrowserBlocked</span></span>|<span data-ttu-id="f578e-232">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-232">Boolean</span></span>|<span data-ttu-id="f578e-233">Gibt an, ob der Webbrowser blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f578e-233">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="f578e-234">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="f578e-234">wifiBlocked</span></span>|<span data-ttu-id="f578e-235">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-235">Boolean</span></span>|<span data-ttu-id="f578e-236">Gibt an, ob die WLAN-Funktion blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f578e-236">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="f578e-237">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="f578e-237">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="f578e-238">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-238">Boolean</span></span>|<span data-ttu-id="f578e-239">Gibt an, ob die automatische Herstellung einer Verbindung zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f578e-239">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="f578e-240">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="f578e-240">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="f578e-241">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="f578e-241">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="f578e-242">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-242">Boolean</span></span>|<span data-ttu-id="f578e-243">Gibt an, ob die Erstellung von Berichten zu WLAN-Hotspots blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f578e-243">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="f578e-244">Hat keine Auswirkungen, wenn die WLAN-Funktion blockiert ist.</span><span class="sxs-lookup"><span data-stu-id="f578e-244">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="f578e-245">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f578e-245">windowsStoreBlocked</span></span>|<span data-ttu-id="f578e-246">boolesch</span><span class="sxs-lookup"><span data-stu-id="f578e-246">Boolean</span></span>|<span data-ttu-id="f578e-247">Gibt an, ob der Windows Store blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f578e-247">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="f578e-248">Antwort</span><span class="sxs-lookup"><span data-stu-id="f578e-248">Response</span></span>
<span data-ttu-id="f578e-249">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f578e-249">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f578e-250">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f578e-250">Example</span></span>
### <a name="request"></a><span data-ttu-id="f578e-251">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f578e-251">Request</span></span>
<span data-ttu-id="f578e-252">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f578e-252">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f578e-253">Antwort</span><span class="sxs-lookup"><span data-stu-id="f578e-253">Response</span></span>
<span data-ttu-id="f578e-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f578e-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








