# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="4c655-101">Erstellen von „windows81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="4c655-101">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="4c655-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4c655-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c655-103">Diese Methode erstellt ein neues Objekt des Typs [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c655-103">Create a new [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c655-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4c655-104">Prerequisites</span></span>
<span data-ttu-id="4c655-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c655-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4c655-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4c655-107">Permission type</span></span>|<span data-ttu-id="4c655-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4c655-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c655-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4c655-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4c655-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c655-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c655-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4c655-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c655-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c655-112">Not supported.</span></span>|
|<span data-ttu-id="4c655-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4c655-113">Application</span></span>|<span data-ttu-id="4c655-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c655-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c655-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c655-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4c655-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4c655-116">Request headers</span></span>
|<span data-ttu-id="4c655-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4c655-117">Header</span></span>|<span data-ttu-id="4c655-118">Wert</span><span class="sxs-lookup"><span data-stu-id="4c655-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c655-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4c655-119">Authorization</span></span>|<span data-ttu-id="4c655-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4c655-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c655-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="4c655-121">Accept</span></span>|<span data-ttu-id="4c655-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="4c655-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c655-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4c655-123">Request body</span></span>
<span data-ttu-id="4c655-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows81GeneralConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="4c655-124">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="4c655-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows81GeneralConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="4c655-125">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="4c655-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4c655-126">Property</span></span>|<span data-ttu-id="4c655-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4c655-127">Type</span></span>|<span data-ttu-id="4c655-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c655-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c655-129">id</span><span class="sxs-lookup"><span data-stu-id="4c655-129">id</span></span>|<span data-ttu-id="4c655-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c655-130">String</span></span>|<span data-ttu-id="4c655-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4c655-131">Key of the entity.</span></span> <span data-ttu-id="4c655-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c655-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c655-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c655-133">lastModifiedDateTime</span></span>|<span data-ttu-id="4c655-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c655-134">DateTimeOffset</span></span>|<span data-ttu-id="4c655-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4c655-135">DateTime the object was last modified.</span></span> <span data-ttu-id="4c655-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c655-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c655-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c655-137">createdDateTime</span></span>|<span data-ttu-id="4c655-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c655-138">DateTimeOffset</span></span>|<span data-ttu-id="4c655-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4c655-139">DateTime the object was created.</span></span> <span data-ttu-id="4c655-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c655-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c655-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c655-141">description</span></span>|<span data-ttu-id="4c655-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c655-142">String</span></span>|<span data-ttu-id="4c655-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4c655-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4c655-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c655-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c655-145">displayName</span><span class="sxs-lookup"><span data-stu-id="4c655-145">displayName</span></span>|<span data-ttu-id="4c655-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c655-146">String</span></span>|<span data-ttu-id="4c655-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4c655-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4c655-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c655-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c655-149">Version</span><span class="sxs-lookup"><span data-stu-id="4c655-149">version</span></span>|<span data-ttu-id="4c655-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4c655-150">Int32</span></span>|<span data-ttu-id="4c655-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="4c655-151">Version of the device configuration.</span></span> <span data-ttu-id="4c655-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c655-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c655-153">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="4c655-153">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="4c655-154">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-154">Boolean</span></span>|<span data-ttu-id="4c655-155">Gibt an, ob verhindert werden soll, dass der Benutzer E-Mail-Konten zu Geräten hinzufügt, die keinem Microsoft-Konto zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="4c655-155">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="4c655-156">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="4c655-156">applyOnlyToWindows81</span></span>|<span data-ttu-id="4c655-157">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-157">Boolean</span></span>|<span data-ttu-id="4c655-158">Wert, der angibt, ob die Richtlinie nur für Windows 8.1 gilt.</span><span class="sxs-lookup"><span data-stu-id="4c655-158">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="4c655-159">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4c655-159">This property is read-only.</span></span>|
|<span data-ttu-id="4c655-160">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="4c655-160">browserBlockAutofill</span></span>|<span data-ttu-id="4c655-161">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-161">Boolean</span></span>|<span data-ttu-id="4c655-162">Gibt an, ob AutoAusfüllen blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4c655-162">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="4c655-163">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="4c655-163">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="4c655-164">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-164">Boolean</span></span>|<span data-ttu-id="4c655-165">Gibt an, ob die automatische Erkennung von Intranetwebsites blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4c655-165">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="4c655-166">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="4c655-166">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="4c655-167">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-167">Boolean</span></span>|<span data-ttu-id="4c655-168">Gibt an, ob der Zugriff im Unternehmensmodus blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4c655-168">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="4c655-169">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="4c655-169">browserBlockJavaScript</span></span>|<span data-ttu-id="4c655-170">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-170">Boolean</span></span>|<span data-ttu-id="4c655-171">Gibt an, ob verhindert werden soll, dass der Benutzer JavaScript verwendet.</span><span class="sxs-lookup"><span data-stu-id="4c655-171">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="4c655-172">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="4c655-172">browserBlockPlugins</span></span>|<span data-ttu-id="4c655-173">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-173">Boolean</span></span>|<span data-ttu-id="4c655-174">Gibt an, ob Plug-Ins blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4c655-174">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="4c655-175">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="4c655-175">browserBlockPopups</span></span>|<span data-ttu-id="4c655-176">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-176">Boolean</span></span>|<span data-ttu-id="4c655-177">Gibt an, ob Popups blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4c655-177">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="4c655-178">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="4c655-178">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="4c655-179">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-179">Boolean</span></span>|<span data-ttu-id="4c655-180">Gibt an, ob verhindert werden soll, dass der Benutzer den „Do not track“-Header sendet.</span><span class="sxs-lookup"><span data-stu-id="4c655-180">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="4c655-181">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="4c655-181">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="4c655-182">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-182">Boolean</span></span>|<span data-ttu-id="4c655-183">Gibt an, ob Einträge mit nur einem einzigen Wort auf Intranetwebsites blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4c655-183">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="4c655-184">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="4c655-184">browserRequireSmartScreen</span></span>|<span data-ttu-id="4c655-185">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-185">Boolean</span></span>|<span data-ttu-id="4c655-186">Gibt an, ob der Benutzer den Smartscreenfilter verwenden muss.</span><span class="sxs-lookup"><span data-stu-id="4c655-186">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="4c655-187">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="4c655-187">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="4c655-188">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c655-188">String</span></span>|<span data-ttu-id="4c655-189">Speicherort der Websiteliste für den Unternehmensmodus.</span><span class="sxs-lookup"><span data-stu-id="4c655-189">The enterprise mode site list location.</span></span> <span data-ttu-id="4c655-190">Dies kann eine lokale Datei, ein lokales Netzwerk oder ein HTTP-Speicherort sein.</span><span class="sxs-lookup"><span data-stu-id="4c655-190">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="4c655-191">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4c655-191">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="4c655-192">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4c655-192">internetSiteSecurityLevel</span></span>](../resources/intune_deviceconfig_internetsitesecuritylevel.md)|<span data-ttu-id="4c655-p110">Die Sicherheitsstufe für das Internet. Mögliche Werte sind: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="4c655-p110">The internet security level. The possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="4c655-195">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4c655-195">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="4c655-196">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4c655-196">siteSecurityLevel</span></span>](../resources/intune_deviceconfig_sitesecuritylevel.md)|<span data-ttu-id="4c655-p111">Die Sicherheitsstufe des Intranets. Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="4c655-p111">The Intranet security level. The possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="4c655-199">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="4c655-199">browserLoggingReportLocation</span></span>|<span data-ttu-id="4c655-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c655-200">String</span></span>|<span data-ttu-id="4c655-201">Speicherort des Protokollierungsberichts</span><span class="sxs-lookup"><span data-stu-id="4c655-201">The logging report location.</span></span>|
|<span data-ttu-id="4c655-202">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="4c655-202">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="4c655-203">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-203">Boolean</span></span>|<span data-ttu-id="4c655-204">Gibt an, ob für eingeschränkte Websites die Sicherheitsstufe „Hoch“ zwingend ist.</span><span class="sxs-lookup"><span data-stu-id="4c655-204">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="4c655-205">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="4c655-205">browserRequireFirewall</span></span>|<span data-ttu-id="4c655-206">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-206">Boolean</span></span>|<span data-ttu-id="4c655-207">Gibt an, ob eine Firewall erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="4c655-207">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="4c655-208">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="4c655-208">browserRequireFraudWarning</span></span>|<span data-ttu-id="4c655-209">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-209">Boolean</span></span>|<span data-ttu-id="4c655-210">Gibt an, ob die Funktion zur Betrugswarnung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="4c655-210">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="4c655-211">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4c655-211">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="4c655-212">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4c655-212">siteSecurityLevel</span></span>](../resources/intune_deviceconfig_sitesecuritylevel.md)|<span data-ttu-id="4c655-p112">Die Sicherheitsstufe für vertrauenswürdige Sites. Mögliche Werte sind: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="4c655-p112">The trusted sites security level. The possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="4c655-215">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="4c655-215">cellularBlockDataRoaming</span></span>|<span data-ttu-id="4c655-216">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-216">Boolean</span></span>|<span data-ttu-id="4c655-217">Gibt an, ob Datenroaming blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4c655-217">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="4c655-218">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="4c655-218">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="4c655-219">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-219">Boolean</span></span>|<span data-ttu-id="4c655-220">Gibt an, ob die Übermittlung von Diagnosedaten blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4c655-220">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="4c655-221">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="4c655-221">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="4c655-222">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-222">Boolean</span></span>|<span data-ttu-id="4c655-223">Gibt an, ob verhindert werden soll, dass der Benutzer einen Bildcode und eine PIN verwendet.</span><span class="sxs-lookup"><span data-stu-id="4c655-223">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="4c655-224">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4c655-224">passwordExpirationDays</span></span>|<span data-ttu-id="4c655-225">Int32</span><span class="sxs-lookup"><span data-stu-id="4c655-225">Int32</span></span>|<span data-ttu-id="4c655-226">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="4c655-226">Password expiration in days.</span></span>|
|<span data-ttu-id="4c655-227">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4c655-227">passwordMinimumLength</span></span>|<span data-ttu-id="4c655-228">Int32</span><span class="sxs-lookup"><span data-stu-id="4c655-228">Int32</span></span>|<span data-ttu-id="4c655-229">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="4c655-229">The minimum password length.</span></span>|
|<span data-ttu-id="4c655-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4c655-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4c655-231">Int32</span><span class="sxs-lookup"><span data-stu-id="4c655-231">Int32</span></span>|<span data-ttu-id="4c655-232">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="4c655-232">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4c655-233">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4c655-233">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4c655-234">Int32</span><span class="sxs-lookup"><span data-stu-id="4c655-234">Int32</span></span>|<span data-ttu-id="4c655-235">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="4c655-235">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4c655-236">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4c655-236">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4c655-237">Int32</span><span class="sxs-lookup"><span data-stu-id="4c655-237">Int32</span></span>|<span data-ttu-id="4c655-238">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="4c655-238">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="4c655-239">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="4c655-239">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4c655-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4c655-240">passwordRequiredType</span></span>|[<span data-ttu-id="4c655-241">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4c655-241">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="4c655-p114">Der erforderliche Kennworttyp. Mögliche Werte: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4c655-p114">The required password type. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4c655-244">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4c655-244">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4c655-245">Int32</span><span class="sxs-lookup"><span data-stu-id="4c655-245">Int32</span></span>|<span data-ttu-id="4c655-246">Die Anzahl von fehlgeschlagenen Anmeldeversuchen, bevor eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="4c655-246">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="4c655-247">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="4c655-247">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="4c655-248">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-248">Boolean</span></span>|<span data-ttu-id="4c655-249">Gibt an, ob für ein Mobilgerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="4c655-249">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="4c655-250">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="4c655-250">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="4c655-251">boolesch</span><span class="sxs-lookup"><span data-stu-id="4c655-251">Boolean</span></span>|<span data-ttu-id="4c655-252">Gibt an, ob automatische Updates erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4c655-252">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="4c655-253">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="4c655-253">userAccountControlSettings</span></span>|[<span data-ttu-id="4c655-254">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="4c655-254">windowsUserAccountControlSettings</span></span>](../resources/intune_deviceconfig_windowsuseraccountcontrolsettings.md)|<span data-ttu-id="4c655-p115">Die Steuerung der Benutzerkontensteuerung. Mögliche Werte sind: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="4c655-p115">The user account control settings. The possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="4c655-257">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="4c655-257">workFoldersUrl</span></span>|<span data-ttu-id="4c655-258">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c655-258">String</span></span>|<span data-ttu-id="4c655-259">URL des Arbeitsordners.</span><span class="sxs-lookup"><span data-stu-id="4c655-259">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="4c655-260">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c655-260">Response</span></span>
<span data-ttu-id="4c655-261">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4c655-261">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c655-262">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4c655-262">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c655-263">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c655-263">Request</span></span>
<span data-ttu-id="4c655-264">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4c655-264">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4c655-265">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c655-265">Response</span></span>
<span data-ttu-id="4c655-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4c655-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








