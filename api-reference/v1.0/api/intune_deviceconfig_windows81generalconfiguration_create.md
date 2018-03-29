# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="91f12-101">Erstellen von „windows81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="91f12-101">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="91f12-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="91f12-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91f12-103">Diese Methode erstellt ein neues Objekt des Typs [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91f12-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="91f12-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="91f12-104">Prerequisites</span></span>
<span data-ttu-id="91f12-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="91f12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="91f12-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="91f12-107">Permission type</span></span>|<span data-ttu-id="91f12-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="91f12-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91f12-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="91f12-109">Delegated (work or school account)</span></span>|<span data-ttu-id="91f12-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f12-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="91f12-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="91f12-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91f12-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="91f12-112">Not supported.</span></span>|
|<span data-ttu-id="91f12-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="91f12-113">Application</span></span>|<span data-ttu-id="91f12-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="91f12-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91f12-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="91f12-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="91f12-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="91f12-116">Request headers</span></span>
|<span data-ttu-id="91f12-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="91f12-117">Header</span></span>|<span data-ttu-id="91f12-118">Wert</span><span class="sxs-lookup"><span data-stu-id="91f12-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91f12-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="91f12-119">Authorization</span></span>|<span data-ttu-id="91f12-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="91f12-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="91f12-121">Accept</span><span class="sxs-lookup"><span data-stu-id="91f12-121">Accept</span></span>|<span data-ttu-id="91f12-122">application/json</span><span class="sxs-lookup"><span data-stu-id="91f12-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91f12-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="91f12-123">Request body</span></span>
<span data-ttu-id="91f12-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows81GeneralConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="91f12-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="91f12-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows81GeneralConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="91f12-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="91f12-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91f12-126">Property</span></span>|<span data-ttu-id="91f12-127">Typ</span><span class="sxs-lookup"><span data-stu-id="91f12-127">Type</span></span>|<span data-ttu-id="91f12-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91f12-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91f12-129">id</span><span class="sxs-lookup"><span data-stu-id="91f12-129">id</span></span>|<span data-ttu-id="91f12-130">String</span><span class="sxs-lookup"><span data-stu-id="91f12-130">String</span></span>|<span data-ttu-id="91f12-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="91f12-131">Key of the setting.</span></span> <span data-ttu-id="91f12-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91f12-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f12-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91f12-133">lastModifiedDateTime</span></span>|<span data-ttu-id="91f12-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91f12-134">DateTimeOffset</span></span>|<span data-ttu-id="91f12-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="91f12-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="91f12-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91f12-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f12-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91f12-137">createdDateTime</span></span>|<span data-ttu-id="91f12-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91f12-138">DateTimeOffset</span></span>|<span data-ttu-id="91f12-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="91f12-139">DateTime the object was created.</span></span> <span data-ttu-id="91f12-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91f12-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f12-141">description</span><span class="sxs-lookup"><span data-stu-id="91f12-141">description</span></span>|<span data-ttu-id="91f12-142">String</span><span class="sxs-lookup"><span data-stu-id="91f12-142">String</span></span>|<span data-ttu-id="91f12-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="91f12-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="91f12-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91f12-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f12-145">displayName</span><span class="sxs-lookup"><span data-stu-id="91f12-145">displayName</span></span>|<span data-ttu-id="91f12-146">String</span><span class="sxs-lookup"><span data-stu-id="91f12-146">String</span></span>|<span data-ttu-id="91f12-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="91f12-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="91f12-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91f12-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f12-149">version</span><span class="sxs-lookup"><span data-stu-id="91f12-149">version</span></span>|<span data-ttu-id="91f12-150">Int32</span><span class="sxs-lookup"><span data-stu-id="91f12-150">Int32</span></span>|<span data-ttu-id="91f12-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="91f12-151">Version of the device configuration.</span></span> <span data-ttu-id="91f12-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91f12-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f12-153">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="91f12-153">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="91f12-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-154">Boolean</span></span>|<span data-ttu-id="91f12-155">Gibt an, ob verhindert werden soll, dass der Benutzer E-Mail-Konten zu Geräten hinzufügt, die keinem Microsoft-Konto zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="91f12-155">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="91f12-156">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="91f12-156">applyOnlyToWindows81</span></span>|<span data-ttu-id="91f12-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-157">Boolean</span></span>|<span data-ttu-id="91f12-158">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="91f12-158">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="91f12-159">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="91f12-159">This property is read-only.</span></span>|
|<span data-ttu-id="91f12-160">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="91f12-160">browserBlockAutofill</span></span>|<span data-ttu-id="91f12-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-161">Boolean</span></span>|<span data-ttu-id="91f12-162">Gibt an, ob AutoAusfüllen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="91f12-162">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="91f12-163">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="91f12-163">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="91f12-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-164">Boolean</span></span>|<span data-ttu-id="91f12-165">Gibt an, ob die automatische Erkennung von Intranetwebsites blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="91f12-165">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="91f12-166">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="91f12-166">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="91f12-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-167">Boolean</span></span>|<span data-ttu-id="91f12-168">Gibt an, ob der Zugriff im Unternehmensmodus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="91f12-168">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="91f12-169">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="91f12-169">browserBlockJavaScript</span></span>|<span data-ttu-id="91f12-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-170">Boolean</span></span>|<span data-ttu-id="91f12-171">Gibt an, ob verhindert werden soll, dass der Benutzer JavaScript verwendet.</span><span class="sxs-lookup"><span data-stu-id="91f12-171">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="91f12-172">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="91f12-172">browserBlockPlugins</span></span>|<span data-ttu-id="91f12-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-173">Boolean</span></span>|<span data-ttu-id="91f12-174">Gibt an, ob Plug-Ins blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="91f12-174">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="91f12-175">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="91f12-175">browserBlockPopups</span></span>|<span data-ttu-id="91f12-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-176">Boolean</span></span>|<span data-ttu-id="91f12-177">Gibt an, ob Popups blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="91f12-177">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="91f12-178">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="91f12-178">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="91f12-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-179">Boolean</span></span>|<span data-ttu-id="91f12-180">Gibt an, ob verhindert werden soll, dass der Benutzer den „Do not track“-Header sendet.</span><span class="sxs-lookup"><span data-stu-id="91f12-180">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="91f12-181">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="91f12-181">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="91f12-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-182">Boolean</span></span>|<span data-ttu-id="91f12-183">Gibt an, ob Einträge mit nur einem einzigen Wort auf Intranetwebsites blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="91f12-183">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="91f12-184">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="91f12-184">browserRequireSmartScreen</span></span>|<span data-ttu-id="91f12-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-185">Boolean</span></span>|<span data-ttu-id="91f12-186">Gibt an, ob der Benutzer den Smartscreenfilter verwenden muss.</span><span class="sxs-lookup"><span data-stu-id="91f12-186">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="91f12-187">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="91f12-187">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="91f12-188">String</span><span class="sxs-lookup"><span data-stu-id="91f12-188">String</span></span>|<span data-ttu-id="91f12-189">Speicherort der Websiteliste für den Unternehmensmodus.</span><span class="sxs-lookup"><span data-stu-id="91f12-189">The enterprise mode site list location.</span></span> <span data-ttu-id="91f12-190">Dies kann eine lokale Datei, ein lokales Netzwerk oder ein HTTP-Speicherort sein.</span><span class="sxs-lookup"><span data-stu-id="91f12-190">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="91f12-191">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="91f12-191">browserInternetSecurityLevel</span></span>|<span data-ttu-id="91f12-192">String</span><span class="sxs-lookup"><span data-stu-id="91f12-192">String</span></span>|<span data-ttu-id="91f12-193">Internetsicherheitsstufe.</span><span class="sxs-lookup"><span data-stu-id="91f12-193">The internet security level.</span></span> <span data-ttu-id="91f12-194">Mögliche Werte sind: `userDefined`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="91f12-194">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="91f12-195">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="91f12-195">browserIntranetSecurityLevel</span></span>|<span data-ttu-id="91f12-196">String</span><span class="sxs-lookup"><span data-stu-id="91f12-196">String</span></span>|<span data-ttu-id="91f12-197">Intranetsicherheitsstufe.</span><span class="sxs-lookup"><span data-stu-id="91f12-197">The Intranet security level.</span></span> <span data-ttu-id="91f12-198">Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="91f12-198">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="91f12-199">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="91f12-199">browserLoggingReportLocation</span></span>|<span data-ttu-id="91f12-200">String</span><span class="sxs-lookup"><span data-stu-id="91f12-200">String</span></span>|<span data-ttu-id="91f12-201">Speicherort des Protokollierungsberichts</span><span class="sxs-lookup"><span data-stu-id="91f12-201">The logging report location.</span></span>|
|<span data-ttu-id="91f12-202">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="91f12-202">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="91f12-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-203">Boolean</span></span>|<span data-ttu-id="91f12-204">Gibt an, ob für eingeschränkte Websites die Sicherheitsstufe „Hoch“ zwingend ist.</span><span class="sxs-lookup"><span data-stu-id="91f12-204">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="91f12-205">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="91f12-205">browserRequireFirewall</span></span>|<span data-ttu-id="91f12-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-206">Boolean</span></span>|<span data-ttu-id="91f12-207">Gibt an, ob eine Firewall erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="91f12-207">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="91f12-208">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="91f12-208">browserRequireFraudWarning</span></span>|<span data-ttu-id="91f12-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-209">Boolean</span></span>|<span data-ttu-id="91f12-210">Gibt an, ob die Funktion zur Betrugswarnung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="91f12-210">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="91f12-211">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="91f12-211">browserTrustedSitesSecurityLevel</span></span>|<span data-ttu-id="91f12-212">String</span><span class="sxs-lookup"><span data-stu-id="91f12-212">String</span></span>|<span data-ttu-id="91f12-213">Sicherheitsstufe für vertrauenswürdige Websites.</span><span class="sxs-lookup"><span data-stu-id="91f12-213">The trusted sites security level.</span></span> <span data-ttu-id="91f12-214">Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh` und `high`.</span><span class="sxs-lookup"><span data-stu-id="91f12-214">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="91f12-215">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="91f12-215">cellularBlockDataRoaming</span></span>|<span data-ttu-id="91f12-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-216">Boolean</span></span>|<span data-ttu-id="91f12-217">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="91f12-217">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="91f12-218">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="91f12-218">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="91f12-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-219">Boolean</span></span>|<span data-ttu-id="91f12-220">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="91f12-220">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="91f12-221">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="91f12-221">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="91f12-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-222">Boolean</span></span>|<span data-ttu-id="91f12-223">Gibt an, ob verhindert werden soll, dass der Benutzer einen Bildcode und eine PIN verwendet.</span><span class="sxs-lookup"><span data-stu-id="91f12-223">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="91f12-224">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="91f12-224">passwordExpirationDays</span></span>|<span data-ttu-id="91f12-225">Int32</span><span class="sxs-lookup"><span data-stu-id="91f12-225">Int32</span></span>|<span data-ttu-id="91f12-226">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="91f12-226">Password expiration in days.</span></span>|
|<span data-ttu-id="91f12-227">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="91f12-227">passwordMinimumLength</span></span>|<span data-ttu-id="91f12-228">Int32</span><span class="sxs-lookup"><span data-stu-id="91f12-228">Int32</span></span>|<span data-ttu-id="91f12-229">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="91f12-229">The minimum password length.</span></span>|
|<span data-ttu-id="91f12-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="91f12-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="91f12-231">Int32</span><span class="sxs-lookup"><span data-stu-id="91f12-231">Int32</span></span>|<span data-ttu-id="91f12-232">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="91f12-232">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="91f12-233">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="91f12-233">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="91f12-234">Int32</span><span class="sxs-lookup"><span data-stu-id="91f12-234">Int32</span></span>|<span data-ttu-id="91f12-235">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="91f12-235">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="91f12-236">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="91f12-236">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="91f12-237">Int32</span><span class="sxs-lookup"><span data-stu-id="91f12-237">Int32</span></span>|<span data-ttu-id="91f12-238">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="91f12-238">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="91f12-239">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="91f12-239">Valid values 0 to 24</span></span>|
|<span data-ttu-id="91f12-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="91f12-240">passwordRequiredType</span></span>|<span data-ttu-id="91f12-241">String</span><span class="sxs-lookup"><span data-stu-id="91f12-241">String</span></span>|<span data-ttu-id="91f12-242">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="91f12-242">The required password type.</span></span> <span data-ttu-id="91f12-243">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="91f12-243">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="91f12-244">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="91f12-244">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="91f12-245">Int32</span><span class="sxs-lookup"><span data-stu-id="91f12-245">Int32</span></span>|<span data-ttu-id="91f12-246">Die Anzahl von fehlgeschlagenen Anmeldeversuchen, bevor eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="91f12-246">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="91f12-247">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="91f12-247">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="91f12-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-248">Boolean</span></span>|<span data-ttu-id="91f12-249">Gibt an, ob für ein Mobilgerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="91f12-249">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="91f12-250">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="91f12-250">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="91f12-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f12-251">Boolean</span></span>|<span data-ttu-id="91f12-252">Gibt an, ob automatische Updates erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="91f12-252">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="91f12-253">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="91f12-253">userAccountControlSettings</span></span>|<span data-ttu-id="91f12-254">String</span><span class="sxs-lookup"><span data-stu-id="91f12-254">String</span></span>|<span data-ttu-id="91f12-255">Einstellungen der Benutzerkontensteuerung.</span><span class="sxs-lookup"><span data-stu-id="91f12-255">The user account control settings.</span></span> <span data-ttu-id="91f12-256">Mögliche Werte sind: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming` und `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="91f12-256">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="91f12-257">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="91f12-257">workFoldersUrl</span></span>|<span data-ttu-id="91f12-258">String</span><span class="sxs-lookup"><span data-stu-id="91f12-258">String</span></span>|<span data-ttu-id="91f12-259">URL des Arbeitsordners.</span><span class="sxs-lookup"><span data-stu-id="91f12-259">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="91f12-260">Antwort</span><span class="sxs-lookup"><span data-stu-id="91f12-260">Response</span></span>
<span data-ttu-id="91f12-261">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="91f12-261">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91f12-262">Beispiel</span><span class="sxs-lookup"><span data-stu-id="91f12-262">Example</span></span>
### <a name="request"></a><span data-ttu-id="91f12-263">Anforderung</span><span class="sxs-lookup"><span data-stu-id="91f12-263">Request</span></span>
<span data-ttu-id="91f12-264">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="91f12-264">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1757

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="91f12-265">Antwort</span><span class="sxs-lookup"><span data-stu-id="91f12-265">Response</span></span>
<span data-ttu-id="91f12-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="91f12-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1865

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```



