# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="8e19a-101">androidCompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="8e19a-101">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="8e19a-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e19a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e19a-103">Erstellt neue Objekte des Typs [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8e19a-103">Create a new [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e19a-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8e19a-104">Prerequisites</span></span>
<span data-ttu-id="8e19a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e19a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8e19a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8e19a-107">Permission type</span></span>|<span data-ttu-id="8e19a-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8e19a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e19a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8e19a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8e19a-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e19a-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e19a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8e19a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e19a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e19a-112">Not supported.</span></span>|
|<span data-ttu-id="8e19a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8e19a-113">Application</span></span>|<span data-ttu-id="8e19a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e19a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e19a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e19a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="8e19a-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8e19a-116">Request headers</span></span>
|<span data-ttu-id="8e19a-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8e19a-117">Header</span></span>|<span data-ttu-id="8e19a-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8e19a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e19a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e19a-119">Authorization</span></span>|<span data-ttu-id="8e19a-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8e19a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e19a-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8e19a-121">Accept</span></span>|<span data-ttu-id="8e19a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8e19a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e19a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8e19a-123">Request body</span></span>
<span data-ttu-id="8e19a-124">Geben Sie im Anforderungstext eine JSON Darstellung für das androidCompliancePolicy-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="8e19a-124">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="8e19a-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidCompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8e19a-125">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="8e19a-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e19a-126">Property</span></span>|<span data-ttu-id="8e19a-127">Typ</span><span class="sxs-lookup"><span data-stu-id="8e19a-127">Type</span></span>|<span data-ttu-id="8e19a-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e19a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e19a-129">id</span><span class="sxs-lookup"><span data-stu-id="8e19a-129">id</span></span>|<span data-ttu-id="8e19a-130">String</span><span class="sxs-lookup"><span data-stu-id="8e19a-130">String</span></span>|<span data-ttu-id="8e19a-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="8e19a-131">Key of the entity.</span></span> <span data-ttu-id="8e19a-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8e19a-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e19a-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e19a-133">createdDateTime</span></span>|<span data-ttu-id="8e19a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e19a-134">DateTimeOffset</span></span>|<span data-ttu-id="8e19a-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8e19a-135">DateTime the object was created.</span></span> <span data-ttu-id="8e19a-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8e19a-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e19a-137">description</span><span class="sxs-lookup"><span data-stu-id="8e19a-137">description</span></span>|<span data-ttu-id="8e19a-138">String</span><span class="sxs-lookup"><span data-stu-id="8e19a-138">String</span></span>|<span data-ttu-id="8e19a-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8e19a-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8e19a-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8e19a-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e19a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e19a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="8e19a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e19a-142">DateTimeOffset</span></span>|<span data-ttu-id="8e19a-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8e19a-143">DateTime the object was last modified.</span></span> <span data-ttu-id="8e19a-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8e19a-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e19a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8e19a-145">displayName</span></span>|<span data-ttu-id="8e19a-146">String</span><span class="sxs-lookup"><span data-stu-id="8e19a-146">String</span></span>|<span data-ttu-id="8e19a-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8e19a-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8e19a-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8e19a-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e19a-149">Version</span><span class="sxs-lookup"><span data-stu-id="8e19a-149">version</span></span>|<span data-ttu-id="8e19a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8e19a-150">Int32</span></span>|<span data-ttu-id="8e19a-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8e19a-151">Version of the device configuration.</span></span> <span data-ttu-id="8e19a-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8e19a-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8e19a-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8e19a-153">passwordRequired</span></span>|<span data-ttu-id="8e19a-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e19a-154">Boolean</span></span>|<span data-ttu-id="8e19a-155">Legt fest, dass zum Entsperren des Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="8e19a-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="8e19a-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8e19a-156">passwordMinimumLength</span></span>|<span data-ttu-id="8e19a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="8e19a-157">Int32</span></span>|<span data-ttu-id="8e19a-158">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="8e19a-158">Minimum password length.</span></span> <span data-ttu-id="8e19a-159">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="8e19a-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="8e19a-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8e19a-160">passwordRequiredType</span></span>|[<span data-ttu-id="8e19a-161">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8e19a-161">androidRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|<span data-ttu-id="8e19a-162">Typ der Zeichen in Kennwort.</span><span class="sxs-lookup"><span data-stu-id="8e19a-162">Type of characters in password.</span></span> <span data-ttu-id="8e19a-163">Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="8e19a-163">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="8e19a-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8e19a-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8e19a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8e19a-165">Int32</span></span>|<span data-ttu-id="8e19a-166">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="8e19a-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="8e19a-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8e19a-167">passwordExpirationDays</span></span>|<span data-ttu-id="8e19a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="8e19a-168">Int32</span></span>|<span data-ttu-id="8e19a-169">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="8e19a-169">Number of days before the password expires.</span></span> <span data-ttu-id="8e19a-170">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="8e19a-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="8e19a-171">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8e19a-171">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8e19a-172">Int32</span><span class="sxs-lookup"><span data-stu-id="8e19a-172">Int32</span></span>|<span data-ttu-id="8e19a-173">Legt fest, wie viele der zuletzt verwendeten Kennwörter nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="8e19a-173">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="8e19a-174">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="8e19a-174">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="8e19a-175">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e19a-175">Boolean</span></span>|<span data-ttu-id="8e19a-176">Legt fest, dass Geräte die Installation von Apps aus unbekannten Quellen nicht zulassen dürfen.</span><span class="sxs-lookup"><span data-stu-id="8e19a-176">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="8e19a-177">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="8e19a-177">securityDisableUsbDebugging</span></span>|<span data-ttu-id="8e19a-178">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e19a-178">Boolean</span></span>|<span data-ttu-id="8e19a-179">Deaktiviert das USB-Debuggen auf Android-Geräten.</span><span class="sxs-lookup"><span data-stu-id="8e19a-179">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="8e19a-180">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="8e19a-180">securityRequireVerifyApps</span></span>|<span data-ttu-id="8e19a-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e19a-181">Boolean</span></span>|<span data-ttu-id="8e19a-182">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="8e19a-182">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="8e19a-183">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="8e19a-183">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="8e19a-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e19a-184">Boolean</span></span>|<span data-ttu-id="8e19a-185">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="8e19a-185">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="8e19a-186">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8e19a-186">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="8e19a-187">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="8e19a-187">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="8e19a-188">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="8e19a-188">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="8e19a-189">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="8e19a-189">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="8e19a-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="8e19a-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="8e19a-191">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e19a-191">Boolean</span></span>|<span data-ttu-id="8e19a-192">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="8e19a-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="8e19a-193">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8e19a-193">osMinimumVersion</span></span>|<span data-ttu-id="8e19a-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e19a-194">String</span></span>|<span data-ttu-id="8e19a-195">Mindestversion von Android</span><span class="sxs-lookup"><span data-stu-id="8e19a-195">Minimum Android version.</span></span>|
|<span data-ttu-id="8e19a-196">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8e19a-196">osMaximumVersion</span></span>|<span data-ttu-id="8e19a-197">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e19a-197">String</span></span>|<span data-ttu-id="8e19a-198">Maximalversion von Android</span><span class="sxs-lookup"><span data-stu-id="8e19a-198">Maximum Android version.</span></span>|
|<span data-ttu-id="8e19a-199">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="8e19a-199">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="8e19a-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e19a-200">String</span></span>|<span data-ttu-id="8e19a-201">Mindestens geforderter Sicherheitspatchlevel von Android</span><span class="sxs-lookup"><span data-stu-id="8e19a-201">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="8e19a-202">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="8e19a-202">storageRequireEncryption</span></span>|<span data-ttu-id="8e19a-203">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e19a-203">Boolean</span></span>|<span data-ttu-id="8e19a-204">Legt fest, dass auf Android-Geräten Verschlüsselung aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="8e19a-204">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="8e19a-205">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="8e19a-205">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="8e19a-206">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e19a-206">Boolean</span></span>|<span data-ttu-id="8e19a-207">Legt fest, dass das Gerät die SafetyNet-Basisintegritätsprüfung bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="8e19a-207">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="8e19a-208">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="8e19a-208">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="8e19a-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e19a-209">Boolean</span></span>|<span data-ttu-id="8e19a-210">Legt fest, dass das Gerät die Prüfung zum SafetyNet-zertifizierten Gerät bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="8e19a-210">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="8e19a-211">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="8e19a-211">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="8e19a-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e19a-212">Boolean</span></span>|<span data-ttu-id="8e19a-213">Legt fest, dass Google Play Services auf dem Gerät installiert und aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="8e19a-213">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="8e19a-214">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="8e19a-214">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="8e19a-215">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e19a-215">Boolean</span></span>|<span data-ttu-id="8e19a-216">Legt fest, dass die Sicherheitsanbieter des Geräts aktuell sein müssen.</span><span class="sxs-lookup"><span data-stu-id="8e19a-216">Require the device to have up to date security providers.</span></span> <span data-ttu-id="8e19a-217">Die aktuelle Version von Google Play Services muss auf dem Gerät installiert und aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="8e19a-217">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="8e19a-218">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="8e19a-218">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="8e19a-219">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8e19a-219">Boolean</span></span>|<span data-ttu-id="8e19a-220">Legt fest, dass das Gerät die Laufzeitintegritätsprüfung für Unternehmensportal-Client-Apps bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="8e19a-220">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="8e19a-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e19a-221">Response</span></span>
<span data-ttu-id="8e19a-222">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8e19a-222">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e19a-223">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8e19a-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e19a-224">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e19a-224">Request</span></span>
<span data-ttu-id="8e19a-225">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8e19a-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="8e19a-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e19a-226">Response</span></span>
<span data-ttu-id="8e19a-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8e19a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "id": "752c820f-820f-752c-0f82-2c750f822c75",
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



