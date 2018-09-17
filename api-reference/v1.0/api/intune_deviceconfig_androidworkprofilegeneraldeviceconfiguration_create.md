# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="39ad4-101">androidWorkProfileGeneralDeviceConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="39ad4-101">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="39ad4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="39ad4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39ad4-103">Erstellt ein neues [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="39ad4-103">Create a new [androidStoreApp](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39ad4-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="39ad4-104">Prerequisites</span></span>
<span data-ttu-id="39ad4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="39ad4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="39ad4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39ad4-107">Permission type</span></span>|<span data-ttu-id="39ad4-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39ad4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39ad4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39ad4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="39ad4-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39ad4-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39ad4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39ad4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39ad4-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39ad4-112">Not supported.</span></span>|
|<span data-ttu-id="39ad4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39ad4-113">Application</span></span>|<span data-ttu-id="39ad4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39ad4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39ad4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39ad4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="39ad4-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39ad4-116">Request headers</span></span>
|<span data-ttu-id="39ad4-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="39ad4-117">Header</span></span>|<span data-ttu-id="39ad4-118">Wert</span><span class="sxs-lookup"><span data-stu-id="39ad4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39ad4-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="39ad4-119">Authorization</span></span>|<span data-ttu-id="39ad4-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="39ad4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39ad4-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="39ad4-121">Accept</span></span>|<span data-ttu-id="39ad4-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="39ad4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39ad4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39ad4-123">Request body</span></span>
<span data-ttu-id="39ad4-124">Geben Sie im Anforderungstext eine JSON-Darstellung des androidWorkProfileGeneralDeviceConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="39ad4-124">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="39ad4-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen von androidWorkProfileGeneralDeviceConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="39ad4-125">The following table shows the properties that are required when you create the deviceAppManagement.</span></span>

|<span data-ttu-id="39ad4-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="39ad4-126">Property</span></span>|<span data-ttu-id="39ad4-127">Typ</span><span class="sxs-lookup"><span data-stu-id="39ad4-127">Type</span></span>|<span data-ttu-id="39ad4-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39ad4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39ad4-129">ID</span><span class="sxs-lookup"><span data-stu-id="39ad4-129">id</span></span>|<span data-ttu-id="39ad4-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="39ad4-130">String</span></span>|<span data-ttu-id="39ad4-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="39ad4-131">Key of the entity.</span></span> <span data-ttu-id="39ad4-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ad4-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ad4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39ad4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="39ad4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ad4-134">DateTimeOffset</span></span>|<span data-ttu-id="39ad4-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="39ad4-135">DateTime the object was last modified.</span></span> <span data-ttu-id="39ad4-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ad4-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ad4-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39ad4-137">createdDateTime</span></span>|<span data-ttu-id="39ad4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ad4-138">DateTimeOffset</span></span>|<span data-ttu-id="39ad4-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="39ad4-139">DateTime the object was created.</span></span> <span data-ttu-id="39ad4-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ad4-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ad4-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39ad4-141">description</span></span>|<span data-ttu-id="39ad4-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="39ad4-142">String</span></span>|<span data-ttu-id="39ad4-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="39ad4-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="39ad4-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ad4-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ad4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="39ad4-145">displayName</span></span>|<span data-ttu-id="39ad4-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="39ad4-146">String</span></span>|<span data-ttu-id="39ad4-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="39ad4-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="39ad4-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ad4-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ad4-149">Version</span><span class="sxs-lookup"><span data-stu-id="39ad4-149">version</span></span>|<span data-ttu-id="39ad4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-150">Int32</span></span>|<span data-ttu-id="39ad4-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="39ad4-151">Version of the device configuration.</span></span> <span data-ttu-id="39ad4-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ad4-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ad4-153">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="39ad4-153">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="39ad4-154">boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-154">Boolean</span></span>|<span data-ttu-id="39ad4-155">Gibt an, ob die Entsperrung durch Fingerabdruck blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="39ad4-155">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="39ad4-156">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="39ad4-156">passwordBlockTrustAgents</span></span>|<span data-ttu-id="39ad4-157">boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-157">Boolean</span></span>|<span data-ttu-id="39ad4-158">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agents blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="39ad4-158">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="39ad4-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="39ad4-159">passwordExpirationDays</span></span>|<span data-ttu-id="39ad4-160">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-160">Int32</span></span>|<span data-ttu-id="39ad4-161">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="39ad4-161">Number of days before the password expires.</span></span> <span data-ttu-id="39ad4-162">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="39ad4-162">Valid values 1 to 365</span></span>|
|<span data-ttu-id="39ad4-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="39ad4-163">passwordMinimumLength</span></span>|<span data-ttu-id="39ad4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-164">Int32</span></span>|<span data-ttu-id="39ad4-165">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="39ad4-165">Minimum length of passwords.</span></span> <span data-ttu-id="39ad4-166">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="39ad4-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="39ad4-167">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="39ad4-167">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="39ad4-168">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-168">Int32</span></span>|<span data-ttu-id="39ad4-169">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="39ad4-169">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="39ad4-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="39ad4-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="39ad4-171">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-171">Int32</span></span>|<span data-ttu-id="39ad4-172">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="39ad4-172">Number of previous passwords to block.</span></span> <span data-ttu-id="39ad4-173">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="39ad4-173">Valid values 0 to 24</span></span>|
|<span data-ttu-id="39ad4-174">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="39ad4-174">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="39ad4-175">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-175">Int32</span></span>|<span data-ttu-id="39ad4-176">Legt fest, nach wie vielen fehlgeschlagenen Anmeldeversuchen eine Zurücksetzung auf die Werkseinstellungen durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="39ad4-176">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="39ad4-177">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="39ad4-177">Valid values 4 to 11</span></span>|
|<span data-ttu-id="39ad4-178">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="39ad4-178">passwordRequiredType</span></span>|[<span data-ttu-id="39ad4-179">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="39ad4-179">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="39ad4-180">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="39ad4-180">Type of password that is required.</span></span> <span data-ttu-id="39ad4-181">Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="39ad4-181">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="39ad4-182">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="39ad4-182">workProfileDataSharingType</span></span>|[<span data-ttu-id="39ad4-183">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="39ad4-183">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune_deviceconfig_androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="39ad4-184">Typ der zulässigen Datenfreigabe.</span><span class="sxs-lookup"><span data-stu-id="39ad4-184">Type of data sharing that is allowed.</span></span> <span data-ttu-id="39ad4-185">Mögliche Werte: sind `deviceDefault`, `preventAny`, `allowPersonalToWork` und `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="39ad4-185">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="39ad4-186">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="39ad4-186">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="39ad4-187">Boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-187">Boolean</span></span>|<span data-ttu-id="39ad4-188">Gibt an, ob Benachrichtigungen blockiert werden, während ein Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="39ad4-188">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="39ad4-189">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="39ad4-189">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="39ad4-190">Boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-190">Boolean</span></span>|<span data-ttu-id="39ad4-191">Blockiert Benutzer vom Hinzufügen/Entfernen von Konten im Arbeitsprofil.</span><span class="sxs-lookup"><span data-stu-id="39ad4-191">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="39ad4-192">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="39ad4-192">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="39ad4-193">Boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-193">Boolean</span></span>|<span data-ttu-id="39ad4-194">Lässt zu, dass Bluetooth-Geräte auf Unternehmenskontakte zugreifen.</span><span class="sxs-lookup"><span data-stu-id="39ad4-194">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="39ad4-195">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="39ad4-195">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="39ad4-196">Boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-196">Boolean</span></span>|<span data-ttu-id="39ad4-197">Blockiert die Bildschirmaufnahme im Arbeitsprofil.</span><span class="sxs-lookup"><span data-stu-id="39ad4-197">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="39ad4-198">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="39ad4-198">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="39ad4-199">Boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-199">Boolean</span></span>|<span data-ttu-id="39ad4-200">Blockiert die Anzeige der Arbeitsprofil-Rufnummernanzeige im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="39ad4-200">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="39ad4-201">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="39ad4-201">workProfileBlockCamera</span></span>|<span data-ttu-id="39ad4-202">Boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-202">Boolean</span></span>|<span data-ttu-id="39ad4-203">Blockiert die Kamera des Arbeitsprofils.</span><span class="sxs-lookup"><span data-stu-id="39ad4-203">Block work profile camera.</span></span>|
|<span data-ttu-id="39ad4-204">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="39ad4-204">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="39ad4-205">Boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-205">Boolean</span></span>|<span data-ttu-id="39ad4-206">Blockiert die Verfügbarkeit der Kontakte des Arbeitsprofils im persönlichen Profil.</span><span class="sxs-lookup"><span data-stu-id="39ad4-206">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="39ad4-207">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="39ad4-207">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="39ad4-208">Boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-208">Boolean</span></span>|<span data-ttu-id="39ad4-209">Boolescher Wert, der angibt, ob die Einstellung für ein Verbot von übergreifendem Kopieren und Einfügen des Profils aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="39ad4-209">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="39ad4-210">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="39ad4-210">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="39ad4-211">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="39ad4-211">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune_deviceconfig_androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="39ad4-212">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="39ad4-212">Type of password that is required.</span></span> <span data-ttu-id="39ad4-213">Mögliche Werte: sind `deviceDefault`, `prompt`, `autoGrant` und `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="39ad4-213">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="39ad4-214">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="39ad4-214">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="39ad4-215">Boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-215">Boolean</span></span>|<span data-ttu-id="39ad4-216">Gibt an, ob die Entsperrung durch Fingerabdruck für das Arbeitsprofil blockiert werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="39ad4-216">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="39ad4-217">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="39ad4-217">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="39ad4-218">Boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-218">Boolean</span></span>|<span data-ttu-id="39ad4-219">Gibt an, ob Smart Lock oder andere Vertrauensstellungs-Agenten für das Arbeitsprofil blockiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="39ad4-219">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="39ad4-220">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="39ad4-220">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="39ad4-221">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-221">Int32</span></span>|<span data-ttu-id="39ad4-222">Anzahl der Tage bis zum Ablaufen des Kennworts des Arbeitsprofils.</span><span class="sxs-lookup"><span data-stu-id="39ad4-222">Number of days before the password expires.</span></span> <span data-ttu-id="39ad4-223">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="39ad4-223">Valid values 1 to 365</span></span>|
|<span data-ttu-id="39ad4-224">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="39ad4-224">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="39ad4-225">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-225">Int32</span></span>|<span data-ttu-id="39ad4-226">Mindestlänge des Kennworts des Arbeitsprofils.</span><span class="sxs-lookup"><span data-stu-id="39ad4-226">Minimum length of work profile password.</span></span> <span data-ttu-id="39ad4-227">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="39ad4-227">Valid values 4 to 16</span></span>|
|<span data-ttu-id="39ad4-228">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="39ad4-228">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="39ad4-229">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-229">Int32</span></span>|<span data-ttu-id="39ad4-230">Mindestanzahl der numerischen Zeichen im Kennwort des Arbeitsprofils.</span><span class="sxs-lookup"><span data-stu-id="39ad4-230">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="39ad4-231">Gültige Werte: 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="39ad4-231">Valid values 1 to 24</span></span>|
|<span data-ttu-id="39ad4-232">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="39ad4-232">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="39ad4-233">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-233">Int32</span></span>|<span data-ttu-id="39ad4-234">Mindestanzahl der Nicht-Buchstaben-Zeichen im Kennwort des Arbeitsprofils.</span><span class="sxs-lookup"><span data-stu-id="39ad4-234">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="39ad4-235">Gültige Werte: 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="39ad4-235">Valid values 1 to 24</span></span>|
|<span data-ttu-id="39ad4-236">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="39ad4-236">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="39ad4-237">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-237">Int32</span></span>|<span data-ttu-id="39ad4-238">Mindestanzahl der Buchstaben im Kennwort des Arbeitsprofils.</span><span class="sxs-lookup"><span data-stu-id="39ad4-238">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="39ad4-239">Gültige Werte: 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="39ad4-239">Valid values 1 to 24</span></span>|
|<span data-ttu-id="39ad4-240">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="39ad4-240">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="39ad4-241">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-241">Int32</span></span>|<span data-ttu-id="39ad4-242">Mindestanzahl der Kleinbuchstaben im Kennwort des Arbeitsprofils.</span><span class="sxs-lookup"><span data-stu-id="39ad4-242">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="39ad4-243">Gültige Werte: 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="39ad4-243">Valid values 1 to 24</span></span>|
|<span data-ttu-id="39ad4-244">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="39ad4-244">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="39ad4-245">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-245">Int32</span></span>|<span data-ttu-id="39ad4-246">Mindestanzahl der Großbuchstaben im Kennwort des Arbeitsprofils.</span><span class="sxs-lookup"><span data-stu-id="39ad4-246">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="39ad4-247">Gültige Werte: 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="39ad4-247">Valid values 1 to 24</span></span>|
|<span data-ttu-id="39ad4-248">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="39ad4-248">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="39ad4-249">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-249">Int32</span></span>|<span data-ttu-id="39ad4-250">Mindestanzahl der Symbole im Kennwort des Arbeitsprofils.</span><span class="sxs-lookup"><span data-stu-id="39ad4-250">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="39ad4-251">Gültige Werte: 1 bis 10</span><span class="sxs-lookup"><span data-stu-id="39ad4-251">Valid values 1 to 24</span></span>|
|<span data-ttu-id="39ad4-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="39ad4-252">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="39ad4-253">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-253">Int32</span></span>|<span data-ttu-id="39ad4-254">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="39ad4-254">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="39ad4-255">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="39ad4-255">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="39ad4-256">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-256">Int32</span></span>|<span data-ttu-id="39ad4-257">Anzahl der zuletzt verwendeten Kennwörter des Arbeitsprofils, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="39ad4-257">Number of previous passwords to block.</span></span> <span data-ttu-id="39ad4-258">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="39ad4-258">Valid values 0 to 24</span></span>|
|<span data-ttu-id="39ad4-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="39ad4-259">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="39ad4-260">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad4-260">Int32</span></span>|<span data-ttu-id="39ad4-261">Anzahl der fehlgeschlagenen Anmeldeversuche, bevor ein Arbeitsprofil entfernt und alle Firmendaten gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="39ad4-261">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="39ad4-262">Gültige Werte: 4 bis 11.</span><span class="sxs-lookup"><span data-stu-id="39ad4-262">Valid values 4 to 11</span></span>|
|<span data-ttu-id="39ad4-263">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="39ad4-263">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="39ad4-264">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="39ad4-264">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="39ad4-265">Geforderter Kennworttyp des Arbeitsprofils.</span><span class="sxs-lookup"><span data-stu-id="39ad4-265">Type of password that is required.</span></span> <span data-ttu-id="39ad4-266">Mögliche Werte sind: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric` und `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="39ad4-266">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="39ad4-267">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="39ad4-267">workProfileRequirePassword</span></span>|<span data-ttu-id="39ad4-268">Boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-268">Boolean</span></span>|<span data-ttu-id="39ad4-269">Entscheidet, ob ein Kennwort für ein Arbeitsprofil erforderlich ist oder nicht</span><span class="sxs-lookup"><span data-stu-id="39ad4-269">Password is required or not for work profile</span></span>|
|<span data-ttu-id="39ad4-270">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="39ad4-270">securityRequireVerifyApps</span></span>|<span data-ttu-id="39ad4-271">Boolesch</span><span class="sxs-lookup"><span data-stu-id="39ad4-271">Boolean</span></span>|<span data-ttu-id="39ad4-272">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="39ad4-272">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="39ad4-273">Antwort</span><span class="sxs-lookup"><span data-stu-id="39ad4-273">Response</span></span>
<span data-ttu-id="39ad4-274">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und ein [AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="39ad4-274">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39ad4-275">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39ad4-275">Example</span></span>
### <a name="request"></a><span data-ttu-id="39ad4-276">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39ad4-276">Request</span></span>
<span data-ttu-id="39ad4-277">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39ad4-277">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1895

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="39ad4-278">Antwort</span><span class="sxs-lookup"><span data-stu-id="39ad4-278">Response</span></span>
<span data-ttu-id="39ad4-p126">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39ad4-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```








