---
title: androidCompliancePolicy erstellen
description: Erstellt neue Objekte des Typs androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c82e218a442aa9f866fdbea4ae5b46bb768de57a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250698"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="59555-103">androidCompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="59555-103">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="59555-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="59555-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59555-105">Erstellt neue Objekte des Typs [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59555-105">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59555-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="59555-106">Prerequisites</span></span>
<span data-ttu-id="59555-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="59555-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="59555-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="59555-109">Permission type</span></span>|<span data-ttu-id="59555-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="59555-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59555-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="59555-111">Delegated (work or school account)</span></span>|<span data-ttu-id="59555-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59555-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="59555-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="59555-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59555-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59555-114">Not supported.</span></span>|
|<span data-ttu-id="59555-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="59555-115">Application</span></span>|<span data-ttu-id="59555-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59555-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59555-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="59555-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="59555-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="59555-118">Request headers</span></span>
|<span data-ttu-id="59555-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="59555-119">Header</span></span>|<span data-ttu-id="59555-120">Wert</span><span class="sxs-lookup"><span data-stu-id="59555-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59555-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="59555-121">Authorization</span></span>|<span data-ttu-id="59555-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="59555-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59555-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="59555-123">Accept</span></span>|<span data-ttu-id="59555-124">application/json</span><span class="sxs-lookup"><span data-stu-id="59555-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59555-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="59555-125">Request body</span></span>
<span data-ttu-id="59555-126">Geben Sie im Anforderungstext eine JSON Darstellung für das androidCompliancePolicy-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="59555-126">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="59555-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidCompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="59555-127">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="59555-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="59555-128">Property</span></span>|<span data-ttu-id="59555-129">Typ</span><span class="sxs-lookup"><span data-stu-id="59555-129">Type</span></span>|<span data-ttu-id="59555-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59555-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59555-131">id</span><span class="sxs-lookup"><span data-stu-id="59555-131">id</span></span>|<span data-ttu-id="59555-132">string</span><span class="sxs-lookup"><span data-stu-id="59555-132">String</span></span>|<span data-ttu-id="59555-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="59555-133">Key of the entity.</span></span> <span data-ttu-id="59555-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59555-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59555-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59555-135">createdDateTime</span></span>|<span data-ttu-id="59555-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59555-136">DateTimeOffset</span></span>|<span data-ttu-id="59555-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="59555-137">DateTime the object was created.</span></span> <span data-ttu-id="59555-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59555-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59555-139">description</span><span class="sxs-lookup"><span data-stu-id="59555-139">description</span></span>|<span data-ttu-id="59555-140">String</span><span class="sxs-lookup"><span data-stu-id="59555-140">String</span></span>|<span data-ttu-id="59555-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="59555-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="59555-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59555-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59555-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59555-143">lastModifiedDateTime</span></span>|<span data-ttu-id="59555-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59555-144">DateTimeOffset</span></span>|<span data-ttu-id="59555-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="59555-145">DateTime the object was last modified.</span></span> <span data-ttu-id="59555-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59555-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59555-147">displayName</span><span class="sxs-lookup"><span data-stu-id="59555-147">displayName</span></span>|<span data-ttu-id="59555-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="59555-148">String</span></span>|<span data-ttu-id="59555-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="59555-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="59555-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59555-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59555-151">Version</span><span class="sxs-lookup"><span data-stu-id="59555-151">version</span></span>|<span data-ttu-id="59555-152">Int32</span><span class="sxs-lookup"><span data-stu-id="59555-152">Int32</span></span>|<span data-ttu-id="59555-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="59555-153">Version of the device configuration.</span></span> <span data-ttu-id="59555-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="59555-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59555-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="59555-155">passwordRequired</span></span>|<span data-ttu-id="59555-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="59555-156">Boolean</span></span>|<span data-ttu-id="59555-157">Legt fest, dass zum Entsperren des Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="59555-157">Require a password to unlock device.</span></span>|
|<span data-ttu-id="59555-158">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="59555-158">passwordMinimumLength</span></span>|<span data-ttu-id="59555-159">Int32</span><span class="sxs-lookup"><span data-stu-id="59555-159">Int32</span></span>|<span data-ttu-id="59555-160">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="59555-160">Minimum password length.</span></span> <span data-ttu-id="59555-161">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="59555-161">Valid values 4 to 16</span></span>|
|<span data-ttu-id="59555-162">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="59555-162">passwordRequiredType</span></span>|[<span data-ttu-id="59555-163">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="59555-163">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="59555-164">Typ der Zeichen im Kennwort.</span><span class="sxs-lookup"><span data-stu-id="59555-164">Type of characters in password.</span></span> <span data-ttu-id="59555-165">Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="59555-165">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="59555-166">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="59555-166">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="59555-167">Int32</span><span class="sxs-lookup"><span data-stu-id="59555-167">Int32</span></span>|<span data-ttu-id="59555-168">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="59555-168">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="59555-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="59555-169">passwordExpirationDays</span></span>|<span data-ttu-id="59555-170">Int32</span><span class="sxs-lookup"><span data-stu-id="59555-170">Int32</span></span>|<span data-ttu-id="59555-171">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="59555-171">Number of days before the password expires.</span></span> <span data-ttu-id="59555-172">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="59555-172">Valid values 1 to 365</span></span>|
|<span data-ttu-id="59555-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="59555-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="59555-174">Int32</span><span class="sxs-lookup"><span data-stu-id="59555-174">Int32</span></span>|<span data-ttu-id="59555-175">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="59555-175">Number of previous passwords to block.</span></span> <span data-ttu-id="59555-176">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="59555-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="59555-177">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="59555-177">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="59555-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="59555-178">Boolean</span></span>|<span data-ttu-id="59555-179">Legt fest, dass Geräte die Installation von Apps aus unbekannten Quellen nicht zulassen dürfen.</span><span class="sxs-lookup"><span data-stu-id="59555-179">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="59555-180">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="59555-180">securityDisableUsbDebugging</span></span>|<span data-ttu-id="59555-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="59555-181">Boolean</span></span>|<span data-ttu-id="59555-182">Deaktiviert das USB-Debuggen auf Android-Geräten.</span><span class="sxs-lookup"><span data-stu-id="59555-182">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="59555-183">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="59555-183">securityRequireVerifyApps</span></span>|<span data-ttu-id="59555-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="59555-184">Boolean</span></span>|<span data-ttu-id="59555-185">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="59555-185">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="59555-186">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="59555-186">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="59555-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="59555-187">Boolean</span></span>|<span data-ttu-id="59555-188">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="59555-188">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="59555-189">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="59555-189">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="59555-190">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="59555-190">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="59555-191">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="59555-191">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="59555-192">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="59555-192">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="59555-193">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="59555-193">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="59555-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="59555-194">Boolean</span></span>|<span data-ttu-id="59555-195">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="59555-195">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="59555-196">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="59555-196">osMinimumVersion</span></span>|<span data-ttu-id="59555-197">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="59555-197">String</span></span>|<span data-ttu-id="59555-198">Mindestversion von Android</span><span class="sxs-lookup"><span data-stu-id="59555-198">Minimum Android version.</span></span>|
|<span data-ttu-id="59555-199">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="59555-199">osMaximumVersion</span></span>|<span data-ttu-id="59555-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="59555-200">String</span></span>|<span data-ttu-id="59555-201">Maximalversion von Android</span><span class="sxs-lookup"><span data-stu-id="59555-201">Maximum Android version.</span></span>|
|<span data-ttu-id="59555-202">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="59555-202">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="59555-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="59555-203">String</span></span>|<span data-ttu-id="59555-204">Mindestens geforderter Sicherheitspatchlevel von Android</span><span class="sxs-lookup"><span data-stu-id="59555-204">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="59555-205">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="59555-205">storageRequireEncryption</span></span>|<span data-ttu-id="59555-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="59555-206">Boolean</span></span>|<span data-ttu-id="59555-207">Legt fest, dass auf Android-Geräten Verschlüsselung aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="59555-207">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="59555-208">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="59555-208">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="59555-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="59555-209">Boolean</span></span>|<span data-ttu-id="59555-210">Legt fest, dass das Gerät die SafetyNet-Basisintegritätsprüfung bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="59555-210">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="59555-211">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="59555-211">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="59555-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="59555-212">Boolean</span></span>|<span data-ttu-id="59555-213">Legt fest, dass das Gerät die Prüfung zum SafetyNet-zertifizierten Gerät bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="59555-213">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="59555-214">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="59555-214">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="59555-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="59555-215">Boolean</span></span>|<span data-ttu-id="59555-216">Legt fest, dass Google Play Services auf dem Gerät installiert und aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="59555-216">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="59555-217">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="59555-217">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="59555-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="59555-218">Boolean</span></span>|<span data-ttu-id="59555-219">Legt fest, dass die Sicherheitsanbieter des Geräts aktuell sein müssen.</span><span class="sxs-lookup"><span data-stu-id="59555-219">Require the device to have up to date security providers.</span></span> <span data-ttu-id="59555-220">Die aktuelle Version von Google Play Services muss auf dem Gerät installiert und aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="59555-220">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="59555-221">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="59555-221">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="59555-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="59555-222">Boolean</span></span>|<span data-ttu-id="59555-223">Legt fest, dass das Gerät die Laufzeitintegritätsprüfung für Unternehmensportal-Client-Apps bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="59555-223">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="59555-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="59555-224">Response</span></span>
<span data-ttu-id="59555-225">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="59555-225">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59555-226">Beispiel</span><span class="sxs-lookup"><span data-stu-id="59555-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="59555-227">Anforderung</span><span class="sxs-lookup"><span data-stu-id="59555-227">Request</span></span>
<span data-ttu-id="59555-228">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="59555-228">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="59555-229">Antwort</span><span class="sxs-lookup"><span data-stu-id="59555-229">Response</span></span>
<span data-ttu-id="59555-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="59555-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



