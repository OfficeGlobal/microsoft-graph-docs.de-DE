# <a name="update-androidworkprofilecompliancepolicy"></a><span data-ttu-id="57bd5-101">AndroidWorkProfileCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="57bd5-101">Update androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="57bd5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="57bd5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57bd5-103">Aktualisieren Sie die Eigenschaften eines [AndroidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="57bd5-103">Update the properties of a [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57bd5-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="57bd5-104">Prerequisites</span></span>
<span data-ttu-id="57bd5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="57bd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="57bd5-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="57bd5-107">Permission type</span></span>|<span data-ttu-id="57bd5-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="57bd5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57bd5-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="57bd5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="57bd5-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57bd5-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57bd5-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="57bd5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57bd5-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57bd5-112">Not supported.</span></span>|
|<span data-ttu-id="57bd5-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="57bd5-113">Application</span></span>|<span data-ttu-id="57bd5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57bd5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57bd5-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="57bd5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="57bd5-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="57bd5-116">Request headers</span></span>
|<span data-ttu-id="57bd5-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="57bd5-117">Header</span></span>|<span data-ttu-id="57bd5-118">Wert</span><span class="sxs-lookup"><span data-stu-id="57bd5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57bd5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="57bd5-119">Authorization</span></span>|<span data-ttu-id="57bd5-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="57bd5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57bd5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="57bd5-121">Accept</span></span>|<span data-ttu-id="57bd5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="57bd5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57bd5-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="57bd5-123">Request body</span></span>
<span data-ttu-id="57bd5-124">Geben Sie im Textkörper Anforderung für das Objekt [AndroidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="57bd5-124">In the request body, supply a JSON representation for the [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="57bd5-125">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="57bd5-125">The following table shows the properties that are required when you create the [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md).</span></span>

|<span data-ttu-id="57bd5-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="57bd5-126">Property</span></span>|<span data-ttu-id="57bd5-127">Typ</span><span class="sxs-lookup"><span data-stu-id="57bd5-127">Type</span></span>|<span data-ttu-id="57bd5-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57bd5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57bd5-129">id</span><span class="sxs-lookup"><span data-stu-id="57bd5-129">id</span></span>|<span data-ttu-id="57bd5-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="57bd5-130">String</span></span>|<span data-ttu-id="57bd5-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="57bd5-131">Key of the entity.</span></span> <span data-ttu-id="57bd5-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57bd5-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57bd5-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57bd5-133">createdDateTime</span></span>|<span data-ttu-id="57bd5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57bd5-134">DateTimeOffset</span></span>|<span data-ttu-id="57bd5-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="57bd5-135">DateTime the object was created.</span></span> <span data-ttu-id="57bd5-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57bd5-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57bd5-137">description</span><span class="sxs-lookup"><span data-stu-id="57bd5-137">description</span></span>|<span data-ttu-id="57bd5-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="57bd5-138">String</span></span>|<span data-ttu-id="57bd5-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="57bd5-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="57bd5-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57bd5-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57bd5-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57bd5-141">lastModifiedDateTime</span></span>|<span data-ttu-id="57bd5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57bd5-142">DateTimeOffset</span></span>|<span data-ttu-id="57bd5-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="57bd5-143">DateTime the object was last modified.</span></span> <span data-ttu-id="57bd5-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57bd5-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57bd5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="57bd5-145">displayName</span></span>|<span data-ttu-id="57bd5-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="57bd5-146">String</span></span>|<span data-ttu-id="57bd5-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="57bd5-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="57bd5-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57bd5-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57bd5-149">Version</span><span class="sxs-lookup"><span data-stu-id="57bd5-149">version</span></span>|<span data-ttu-id="57bd5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="57bd5-150">Int32</span></span>|<span data-ttu-id="57bd5-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="57bd5-151">Version of the device configuration.</span></span> <span data-ttu-id="57bd5-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57bd5-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57bd5-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="57bd5-153">passwordRequired</span></span>|<span data-ttu-id="57bd5-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57bd5-154">Boolean</span></span>|<span data-ttu-id="57bd5-155">Legt fest, dass zum Entsperren des Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="57bd5-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="57bd5-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="57bd5-156">passwordMinimumLength</span></span>|<span data-ttu-id="57bd5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="57bd5-157">Int32</span></span>|<span data-ttu-id="57bd5-158">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="57bd5-158">Minimum password length.</span></span> <span data-ttu-id="57bd5-159">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="57bd5-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="57bd5-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="57bd5-160">passwordRequiredType</span></span>|[<span data-ttu-id="57bd5-161">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="57bd5-161">androidRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|<span data-ttu-id="57bd5-162">Typ der Zeichen in Kennwort.</span><span class="sxs-lookup"><span data-stu-id="57bd5-162">Type of characters in password.</span></span> <span data-ttu-id="57bd5-163">Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="57bd5-163">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="57bd5-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="57bd5-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="57bd5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="57bd5-165">Int32</span></span>|<span data-ttu-id="57bd5-166">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="57bd5-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="57bd5-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="57bd5-167">passwordExpirationDays</span></span>|<span data-ttu-id="57bd5-168">Int32</span><span class="sxs-lookup"><span data-stu-id="57bd5-168">Int32</span></span>|<span data-ttu-id="57bd5-169">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="57bd5-169">Number of days before the password expires.</span></span> <span data-ttu-id="57bd5-170">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="57bd5-170">Valid values 1 to 365</span></span>|
|<span data-ttu-id="57bd5-171">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="57bd5-171">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="57bd5-172">Int32</span><span class="sxs-lookup"><span data-stu-id="57bd5-172">Int32</span></span>|<span data-ttu-id="57bd5-173">Legt fest, wie viele der zuletzt verwendeten Kennwörter nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="57bd5-173">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="57bd5-174">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="57bd5-174">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="57bd5-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57bd5-175">Boolean</span></span>|<span data-ttu-id="57bd5-176">Legt fest, dass Geräte die Installation von Apps aus unbekannten Quellen nicht zulassen dürfen.</span><span class="sxs-lookup"><span data-stu-id="57bd5-176">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="57bd5-177">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="57bd5-177">securityDisableUsbDebugging</span></span>|<span data-ttu-id="57bd5-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57bd5-178">Boolean</span></span>|<span data-ttu-id="57bd5-179">Deaktiviert das USB-Debuggen auf Android-Geräten.</span><span class="sxs-lookup"><span data-stu-id="57bd5-179">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="57bd5-180">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="57bd5-180">securityRequireVerifyApps</span></span>|<span data-ttu-id="57bd5-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57bd5-181">Boolean</span></span>|<span data-ttu-id="57bd5-182">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="57bd5-182">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="57bd5-183">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="57bd5-183">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="57bd5-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57bd5-184">Boolean</span></span>|<span data-ttu-id="57bd5-185">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="57bd5-185">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="57bd5-186">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="57bd5-186">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="57bd5-187">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="57bd5-187">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="57bd5-188">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="57bd5-188">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="57bd5-189">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="57bd5-189">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="57bd5-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="57bd5-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="57bd5-191">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57bd5-191">Boolean</span></span>|<span data-ttu-id="57bd5-192">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="57bd5-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="57bd5-193">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="57bd5-193">osMinimumVersion</span></span>|<span data-ttu-id="57bd5-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="57bd5-194">String</span></span>|<span data-ttu-id="57bd5-195">Mindestversion von Android</span><span class="sxs-lookup"><span data-stu-id="57bd5-195">Minimum Android version.</span></span>|
|<span data-ttu-id="57bd5-196">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="57bd5-196">osMaximumVersion</span></span>|<span data-ttu-id="57bd5-197">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="57bd5-197">String</span></span>|<span data-ttu-id="57bd5-198">Maximalversion von Android</span><span class="sxs-lookup"><span data-stu-id="57bd5-198">Maximum Android version.</span></span>|
|<span data-ttu-id="57bd5-199">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="57bd5-199">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="57bd5-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="57bd5-200">String</span></span>|<span data-ttu-id="57bd5-201">Mindestens geforderter Sicherheitspatchlevel von Android</span><span class="sxs-lookup"><span data-stu-id="57bd5-201">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="57bd5-202">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="57bd5-202">storageRequireEncryption</span></span>|<span data-ttu-id="57bd5-203">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57bd5-203">Boolean</span></span>|<span data-ttu-id="57bd5-204">Legt fest, dass auf Android-Geräten Verschlüsselung aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="57bd5-204">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="57bd5-205">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="57bd5-205">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="57bd5-206">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57bd5-206">Boolean</span></span>|<span data-ttu-id="57bd5-207">Legt fest, dass das Gerät die SafetyNet-Basisintegritätsprüfung bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="57bd5-207">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="57bd5-208">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="57bd5-208">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="57bd5-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57bd5-209">Boolean</span></span>|<span data-ttu-id="57bd5-210">Legt fest, dass das Gerät die Prüfung zum SafetyNet-zertifizierten Gerät bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="57bd5-210">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="57bd5-211">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="57bd5-211">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="57bd5-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57bd5-212">Boolean</span></span>|<span data-ttu-id="57bd5-213">Legt fest, dass Google Play Services auf dem Gerät installiert und aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="57bd5-213">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="57bd5-214">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="57bd5-214">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="57bd5-215">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57bd5-215">Boolean</span></span>|<span data-ttu-id="57bd5-216">Legt fest, dass die Sicherheitsanbieter des Geräts aktuell sein müssen.</span><span class="sxs-lookup"><span data-stu-id="57bd5-216">Require the device to have up to date security providers.</span></span> <span data-ttu-id="57bd5-217">Die aktuelle Version von Google Play Services muss auf dem Gerät installiert und aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="57bd5-217">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="57bd5-218">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="57bd5-218">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="57bd5-219">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="57bd5-219">Boolean</span></span>|<span data-ttu-id="57bd5-220">Legt fest, dass das Gerät die Laufzeitintegritätsprüfung für Unternehmensportal-Client-Apps bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="57bd5-220">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="57bd5-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="57bd5-221">Response</span></span>
<span data-ttu-id="57bd5-222">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="57bd5-222">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57bd5-223">Beispiel</span><span class="sxs-lookup"><span data-stu-id="57bd5-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="57bd5-224">Anforderung</span><span class="sxs-lookup"><span data-stu-id="57bd5-224">Request</span></span>
<span data-ttu-id="57bd5-225">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="57bd5-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1170

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="57bd5-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="57bd5-226">Response</span></span>
<span data-ttu-id="57bd5-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="57bd5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1342

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "id": "4e385271-5271-4e38-7152-384e7152384e",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```



