---
title: Erstellen von androidWorkProfileCompliancePolicy
description: Erstellen eines neuen AndroidWorkProfileCompliancePolicy-Objekts.
author: tfitzmac
ms.openlocfilehash: ef3b9b7d15eea1911a17747b845ca80341ae02a5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339305"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="71908-103">Erstellen von androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="71908-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="71908-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="71908-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71908-105">Erstellen eines neuen [AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="71908-105">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71908-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="71908-106">Prerequisites</span></span>
<span data-ttu-id="71908-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71908-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71908-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71908-109">Permission type</span></span>|<span data-ttu-id="71908-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71908-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71908-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71908-111">Delegated (work or school account)</span></span>|<span data-ttu-id="71908-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71908-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71908-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71908-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71908-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71908-114">Not supported.</span></span>|
|<span data-ttu-id="71908-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71908-115">Application</span></span>|<span data-ttu-id="71908-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71908-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71908-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71908-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="71908-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71908-118">Request headers</span></span>
|<span data-ttu-id="71908-119">Header</span><span class="sxs-lookup"><span data-stu-id="71908-119">Header</span></span>|<span data-ttu-id="71908-120">Wert</span><span class="sxs-lookup"><span data-stu-id="71908-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71908-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="71908-121">Authorization</span></span>|<span data-ttu-id="71908-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="71908-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71908-123">Accept</span><span class="sxs-lookup"><span data-stu-id="71908-123">Accept</span></span>|<span data-ttu-id="71908-124">application/json</span><span class="sxs-lookup"><span data-stu-id="71908-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71908-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71908-125">Request body</span></span>
<span data-ttu-id="71908-126">Geben Sie im Textkörper Anforderung für das Objekt AndroidWorkProfileCompliancePolicy eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="71908-126">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="71908-127">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidWorkProfileCompliancePolicy erstellen.</span><span class="sxs-lookup"><span data-stu-id="71908-127">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="71908-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71908-128">Property</span></span>|<span data-ttu-id="71908-129">Typ</span><span class="sxs-lookup"><span data-stu-id="71908-129">Type</span></span>|<span data-ttu-id="71908-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71908-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71908-131">id</span><span class="sxs-lookup"><span data-stu-id="71908-131">id</span></span>|<span data-ttu-id="71908-132">String</span><span class="sxs-lookup"><span data-stu-id="71908-132">String</span></span>|<span data-ttu-id="71908-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="71908-133">Key of the entity.</span></span> <span data-ttu-id="71908-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71908-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="71908-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71908-135">createdDateTime</span></span>|<span data-ttu-id="71908-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71908-136">DateTimeOffset</span></span>|<span data-ttu-id="71908-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="71908-137">DateTime the object was created.</span></span> <span data-ttu-id="71908-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71908-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="71908-139">description</span><span class="sxs-lookup"><span data-stu-id="71908-139">description</span></span>|<span data-ttu-id="71908-140">String</span><span class="sxs-lookup"><span data-stu-id="71908-140">String</span></span>|<span data-ttu-id="71908-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="71908-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71908-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71908-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="71908-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71908-143">lastModifiedDateTime</span></span>|<span data-ttu-id="71908-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71908-144">DateTimeOffset</span></span>|<span data-ttu-id="71908-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="71908-145">DateTime the object was last modified.</span></span> <span data-ttu-id="71908-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71908-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="71908-147">displayName</span><span class="sxs-lookup"><span data-stu-id="71908-147">displayName</span></span>|<span data-ttu-id="71908-148">String</span><span class="sxs-lookup"><span data-stu-id="71908-148">String</span></span>|<span data-ttu-id="71908-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="71908-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71908-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71908-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="71908-151">Version</span><span class="sxs-lookup"><span data-stu-id="71908-151">version</span></span>|<span data-ttu-id="71908-152">Int32</span><span class="sxs-lookup"><span data-stu-id="71908-152">Int32</span></span>|<span data-ttu-id="71908-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="71908-153">Version of the device configuration.</span></span> <span data-ttu-id="71908-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71908-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="71908-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="71908-155">passwordRequired</span></span>|<span data-ttu-id="71908-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71908-156">Boolean</span></span>|<span data-ttu-id="71908-157">Legt fest, dass zum Entsperren des Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="71908-157">Require a password to unlock device.</span></span>|
|<span data-ttu-id="71908-158">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="71908-158">passwordMinimumLength</span></span>|<span data-ttu-id="71908-159">Int32</span><span class="sxs-lookup"><span data-stu-id="71908-159">Int32</span></span>|<span data-ttu-id="71908-160">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="71908-160">Minimum password length.</span></span> <span data-ttu-id="71908-161">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="71908-161">Valid values 4 to 16</span></span>|
|<span data-ttu-id="71908-162">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="71908-162">passwordRequiredType</span></span>|[<span data-ttu-id="71908-163">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="71908-163">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="71908-164">Typ der Zeichen in Kennwort.</span><span class="sxs-lookup"><span data-stu-id="71908-164">Type of characters in password.</span></span> <span data-ttu-id="71908-165">Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="71908-165">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="71908-166">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="71908-166">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="71908-167">Int32</span><span class="sxs-lookup"><span data-stu-id="71908-167">Int32</span></span>|<span data-ttu-id="71908-168">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="71908-168">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="71908-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="71908-169">passwordExpirationDays</span></span>|<span data-ttu-id="71908-170">Int32</span><span class="sxs-lookup"><span data-stu-id="71908-170">Int32</span></span>|<span data-ttu-id="71908-171">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="71908-171">Number of days before the password expires.</span></span> <span data-ttu-id="71908-172">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="71908-172">Valid values 1 to 365</span></span>|
|<span data-ttu-id="71908-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="71908-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="71908-174">Int32</span><span class="sxs-lookup"><span data-stu-id="71908-174">Int32</span></span>|<span data-ttu-id="71908-175">Legt fest, wie viele der zuletzt verwendeten Kennwörter nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="71908-175">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="71908-176">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="71908-176">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="71908-177">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71908-177">Boolean</span></span>|<span data-ttu-id="71908-178">Legt fest, dass Geräte die Installation von Apps aus unbekannten Quellen nicht zulassen dürfen.</span><span class="sxs-lookup"><span data-stu-id="71908-178">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="71908-179">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="71908-179">securityDisableUsbDebugging</span></span>|<span data-ttu-id="71908-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71908-180">Boolean</span></span>|<span data-ttu-id="71908-181">Deaktiviert das USB-Debuggen auf Android-Geräten.</span><span class="sxs-lookup"><span data-stu-id="71908-181">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="71908-182">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="71908-182">securityRequireVerifyApps</span></span>|<span data-ttu-id="71908-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71908-183">Boolean</span></span>|<span data-ttu-id="71908-184">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="71908-184">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="71908-185">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="71908-185">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="71908-186">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71908-186">Boolean</span></span>|<span data-ttu-id="71908-187">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="71908-187">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="71908-188">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="71908-188">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="71908-189">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="71908-189">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="71908-190">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="71908-190">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="71908-191">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="71908-191">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="71908-192">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="71908-192">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="71908-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71908-193">Boolean</span></span>|<span data-ttu-id="71908-194">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="71908-194">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="71908-195">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="71908-195">osMinimumVersion</span></span>|<span data-ttu-id="71908-196">String</span><span class="sxs-lookup"><span data-stu-id="71908-196">String</span></span>|<span data-ttu-id="71908-197">Mindestversion von Android</span><span class="sxs-lookup"><span data-stu-id="71908-197">Minimum Android version.</span></span>|
|<span data-ttu-id="71908-198">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="71908-198">osMaximumVersion</span></span>|<span data-ttu-id="71908-199">String</span><span class="sxs-lookup"><span data-stu-id="71908-199">String</span></span>|<span data-ttu-id="71908-200">Maximalversion von Android</span><span class="sxs-lookup"><span data-stu-id="71908-200">Maximum Android version.</span></span>|
|<span data-ttu-id="71908-201">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="71908-201">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="71908-202">String</span><span class="sxs-lookup"><span data-stu-id="71908-202">String</span></span>|<span data-ttu-id="71908-203">Mindestens geforderter Sicherheitspatchlevel von Android</span><span class="sxs-lookup"><span data-stu-id="71908-203">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="71908-204">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="71908-204">storageRequireEncryption</span></span>|<span data-ttu-id="71908-205">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71908-205">Boolean</span></span>|<span data-ttu-id="71908-206">Legt fest, dass auf Android-Geräten Verschlüsselung aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="71908-206">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="71908-207">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="71908-207">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="71908-208">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71908-208">Boolean</span></span>|<span data-ttu-id="71908-209">Legt fest, dass das Gerät die SafetyNet-Basisintegritätsprüfung bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="71908-209">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="71908-210">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="71908-210">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="71908-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71908-211">Boolean</span></span>|<span data-ttu-id="71908-212">Legt fest, dass das Gerät die Prüfung zum SafetyNet-zertifizierten Gerät bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="71908-212">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="71908-213">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="71908-213">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="71908-214">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71908-214">Boolean</span></span>|<span data-ttu-id="71908-215">Legt fest, dass Google Play Services auf dem Gerät installiert und aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="71908-215">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="71908-216">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="71908-216">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="71908-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71908-217">Boolean</span></span>|<span data-ttu-id="71908-218">Legt fest, dass die Sicherheitsanbieter des Geräts aktuell sein müssen.</span><span class="sxs-lookup"><span data-stu-id="71908-218">Require the device to have up to date security providers.</span></span> <span data-ttu-id="71908-219">Die aktuelle Version von Google Play Services muss auf dem Gerät installiert und aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="71908-219">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="71908-220">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="71908-220">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="71908-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="71908-221">Boolean</span></span>|<span data-ttu-id="71908-222">Legt fest, dass das Gerät die Laufzeitintegritätsprüfung für Unternehmensportal-Client-Apps bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="71908-222">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="71908-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="71908-223">Response</span></span>
<span data-ttu-id="71908-224">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="71908-224">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71908-225">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71908-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="71908-226">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71908-226">Request</span></span>
<span data-ttu-id="71908-227">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71908-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="71908-228">Antwort</span><span class="sxs-lookup"><span data-stu-id="71908-228">Response</span></span>
<span data-ttu-id="71908-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71908-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



