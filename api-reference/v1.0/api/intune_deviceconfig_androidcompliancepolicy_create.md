# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="57f02-101">androidCompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="57f02-101">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="57f02-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="57f02-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57f02-103">Erstellt neue Objekte des Typs [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57f02-103">Create a new [plannerBucket](../resources/intune_deviceconfig_androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57f02-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="57f02-104">Prerequisites</span></span>
<span data-ttu-id="57f02-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="57f02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="57f02-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="57f02-107">Permission type</span></span>|<span data-ttu-id="57f02-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="57f02-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57f02-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="57f02-109">Delegated (work or school account)</span></span>|<span data-ttu-id="57f02-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57f02-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57f02-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="57f02-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57f02-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57f02-112">Not supported.</span></span>|
|<span data-ttu-id="57f02-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="57f02-113">Application</span></span>|<span data-ttu-id="57f02-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57f02-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57f02-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="57f02-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="57f02-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="57f02-116">Request headers</span></span>
|<span data-ttu-id="57f02-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="57f02-117">Header</span></span>|<span data-ttu-id="57f02-118">Wert</span><span class="sxs-lookup"><span data-stu-id="57f02-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57f02-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="57f02-119">Authorization</span></span>|<span data-ttu-id="57f02-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="57f02-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="57f02-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="57f02-121">Accept</span></span>|<span data-ttu-id="57f02-122">application/json</span><span class="sxs-lookup"><span data-stu-id="57f02-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57f02-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="57f02-123">Request body</span></span>
<span data-ttu-id="57f02-124">Geben Sie im Anforderungstext eine JSON Darstellung für das androidCompliancePolicy-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="57f02-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="57f02-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidCompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="57f02-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="57f02-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="57f02-126">Property</span></span>|<span data-ttu-id="57f02-127">Typ</span><span class="sxs-lookup"><span data-stu-id="57f02-127">Type</span></span>|<span data-ttu-id="57f02-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57f02-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57f02-129">id</span><span class="sxs-lookup"><span data-stu-id="57f02-129">id</span></span>|<span data-ttu-id="57f02-130">String</span><span class="sxs-lookup"><span data-stu-id="57f02-130">String</span></span>|<span data-ttu-id="57f02-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="57f02-131">Key of the setting.</span></span> <span data-ttu-id="57f02-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57f02-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57f02-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57f02-133">createdDateTime</span></span>|<span data-ttu-id="57f02-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57f02-134">DateTimeOffset</span></span>|<span data-ttu-id="57f02-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="57f02-135">DateTime the object was created.</span></span> <span data-ttu-id="57f02-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57f02-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57f02-137">description</span><span class="sxs-lookup"><span data-stu-id="57f02-137">description</span></span>|<span data-ttu-id="57f02-138">String</span><span class="sxs-lookup"><span data-stu-id="57f02-138">String</span></span>|<span data-ttu-id="57f02-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="57f02-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="57f02-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57f02-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57f02-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57f02-141">lastModifiedDateTime</span></span>|<span data-ttu-id="57f02-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57f02-142">DateTimeOffset</span></span>|<span data-ttu-id="57f02-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="57f02-143">Indicates the date the object was last modified.</span></span> <span data-ttu-id="57f02-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57f02-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57f02-145">displayName</span><span class="sxs-lookup"><span data-stu-id="57f02-145">displayName</span></span>|<span data-ttu-id="57f02-146">String</span><span class="sxs-lookup"><span data-stu-id="57f02-146">String</span></span>|<span data-ttu-id="57f02-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="57f02-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="57f02-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57f02-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57f02-149">Version</span><span class="sxs-lookup"><span data-stu-id="57f02-149">version</span></span>|<span data-ttu-id="57f02-150">Int32</span><span class="sxs-lookup"><span data-stu-id="57f02-150">Int32</span></span>|<span data-ttu-id="57f02-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="57f02-151">Version of the device configuration.</span></span> <span data-ttu-id="57f02-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="57f02-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="57f02-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="57f02-153">passwordRequired</span></span>|<span data-ttu-id="57f02-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="57f02-154">Boolean</span></span>|<span data-ttu-id="57f02-155">Legt fest, dass zum Entsperren des Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="57f02-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="57f02-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="57f02-156">passwordMinimumLength</span></span>|<span data-ttu-id="57f02-157">Int32</span><span class="sxs-lookup"><span data-stu-id="57f02-157">Int32</span></span>|<span data-ttu-id="57f02-158">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="57f02-158">Minimum password length.</span></span> <span data-ttu-id="57f02-159">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="57f02-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="57f02-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="57f02-160">passwordRequiredType</span></span>|<span data-ttu-id="57f02-161">String</span><span class="sxs-lookup"><span data-stu-id="57f02-161">String</span></span>|<span data-ttu-id="57f02-162">Zulässige Zeichentypen für das Kennwort. Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="57f02-162">Type of characters in password Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="57f02-163">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="57f02-163">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="57f02-164">Int32</span><span class="sxs-lookup"><span data-stu-id="57f02-164">Int32</span></span>|<span data-ttu-id="57f02-165">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="57f02-165">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="57f02-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="57f02-166">passwordExpirationDays</span></span>|<span data-ttu-id="57f02-167">Int32</span><span class="sxs-lookup"><span data-stu-id="57f02-167">Int32</span></span>|<span data-ttu-id="57f02-168">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="57f02-168">Number of days before the password expires.</span></span> <span data-ttu-id="57f02-169">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="57f02-169">Valid values 1 to 365</span></span>|
|<span data-ttu-id="57f02-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="57f02-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="57f02-171">Int32</span><span class="sxs-lookup"><span data-stu-id="57f02-171">Int32</span></span>|<span data-ttu-id="57f02-172">Legt fest, wie viele der zuletzt verwendeten Kennwörter nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="57f02-172">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="57f02-173">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="57f02-173">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="57f02-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="57f02-174">Boolean</span></span>|<span data-ttu-id="57f02-175">Legt fest, dass Geräte die Installation von Apps aus unbekannten Quellen nicht zulassen dürfen.</span><span class="sxs-lookup"><span data-stu-id="57f02-175">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="57f02-176">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="57f02-176">securityDisableUsbDebugging</span></span>|<span data-ttu-id="57f02-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="57f02-177">Boolean</span></span>|<span data-ttu-id="57f02-178">Deaktiviert das USB-Debuggen auf Android-Geräten.</span><span class="sxs-lookup"><span data-stu-id="57f02-178">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="57f02-179">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="57f02-179">securityRequireVerifyApps</span></span>|<span data-ttu-id="57f02-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="57f02-180">Boolean</span></span>|<span data-ttu-id="57f02-181">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="57f02-181">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="57f02-182">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="57f02-182">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="57f02-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="57f02-183">Boolean</span></span>|<span data-ttu-id="57f02-184">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="57f02-184">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="57f02-185">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="57f02-185">deviceThreatProtectionRequiredSecurityLevel</span></span>|<span data-ttu-id="57f02-186">String</span><span class="sxs-lookup"><span data-stu-id="57f02-186">String</span></span>|<span data-ttu-id="57f02-187">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="57f02-187">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="57f02-188">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="57f02-188">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="57f02-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="57f02-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="57f02-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="57f02-190">Boolean</span></span>|<span data-ttu-id="57f02-191">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="57f02-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="57f02-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="57f02-192">osMinimumVersion</span></span>|<span data-ttu-id="57f02-193">String</span><span class="sxs-lookup"><span data-stu-id="57f02-193">String</span></span>|<span data-ttu-id="57f02-194">Mindestversion von Android</span><span class="sxs-lookup"><span data-stu-id="57f02-194">Minimum Android version.</span></span>|
|<span data-ttu-id="57f02-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="57f02-195">osMaximumVersion</span></span>|<span data-ttu-id="57f02-196">String</span><span class="sxs-lookup"><span data-stu-id="57f02-196">String</span></span>|<span data-ttu-id="57f02-197">Maximalversion von Android</span><span class="sxs-lookup"><span data-stu-id="57f02-197">Maximum Android version.</span></span>|
|<span data-ttu-id="57f02-198">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="57f02-198">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="57f02-199">String</span><span class="sxs-lookup"><span data-stu-id="57f02-199">String</span></span>|<span data-ttu-id="57f02-200">Mindestens geforderter Sicherheitspatchlevel von Android</span><span class="sxs-lookup"><span data-stu-id="57f02-200">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="57f02-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="57f02-201">storageRequireEncryption</span></span>|<span data-ttu-id="57f02-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="57f02-202">Boolean</span></span>|<span data-ttu-id="57f02-203">Legt fest, dass auf Android-Geräten Verschlüsselung aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="57f02-203">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="57f02-204">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="57f02-204">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="57f02-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="57f02-205">Boolean</span></span>|<span data-ttu-id="57f02-206">Legt fest, dass das Gerät die SafetyNet-Basisintegritätsprüfung bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="57f02-206">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="57f02-207">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="57f02-207">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="57f02-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="57f02-208">Boolean</span></span>|<span data-ttu-id="57f02-209">Legt fest, dass das Gerät die Prüfung zum SafetyNet-zertifizierten Gerät bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="57f02-209">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="57f02-210">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="57f02-210">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="57f02-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="57f02-211">Boolean</span></span>|<span data-ttu-id="57f02-212">Legt fest, dass Google Play Services auf dem Gerät installiert und aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="57f02-212">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="57f02-213">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="57f02-213">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="57f02-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="57f02-214">Boolean</span></span>|<span data-ttu-id="57f02-215">Legt fest, dass die Sicherheitsanbieter des Geräts aktuell sein müssen.</span><span class="sxs-lookup"><span data-stu-id="57f02-215">Require the device to have up to date security providers.</span></span> <span data-ttu-id="57f02-216">Die aktuelle Version von Google Play Services muss auf dem Gerät installiert und aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="57f02-216">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="57f02-217">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="57f02-217">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="57f02-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="57f02-218">Boolean</span></span>|<span data-ttu-id="57f02-219">Legt fest, dass das Gerät die Laufzeitintegritätsprüfung für Unternehmensportal-Client-Apps bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="57f02-219">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="57f02-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="57f02-220">Response</span></span>
<span data-ttu-id="57f02-221">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="57f02-221">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_deviceconfig_androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57f02-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="57f02-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="57f02-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="57f02-223">Request</span></span>
<span data-ttu-id="57f02-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="57f02-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1223

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="57f02-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="57f02-225">Response</span></span>
<span data-ttu-id="57f02-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="57f02-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



