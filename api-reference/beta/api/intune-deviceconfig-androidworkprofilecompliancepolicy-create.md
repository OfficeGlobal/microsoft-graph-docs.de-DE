---
title: Erstellen von androidWorkProfileCompliancePolicy
description: Erstellen eines neuen AndroidWorkProfileCompliancePolicy-Objekts.
ms.openlocfilehash: a937c1aab21264cda0920d662d2e13b379b42e8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060275"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="4ea63-103">Erstellen von androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4ea63-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="4ea63-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4ea63-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ea63-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4ea63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ea63-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4ea63-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ea63-107">Erstellen eines neuen [AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4ea63-107">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ea63-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4ea63-108">Prerequisites</span></span>
<span data-ttu-id="4ea63-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ea63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ea63-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4ea63-111">Permission type</span></span>|<span data-ttu-id="4ea63-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4ea63-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ea63-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4ea63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ea63-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ea63-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ea63-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4ea63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ea63-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ea63-116">Not supported.</span></span>|
|<span data-ttu-id="4ea63-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4ea63-117">Application</span></span>|<span data-ttu-id="4ea63-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ea63-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ea63-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ea63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="4ea63-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4ea63-120">Request headers</span></span>
|<span data-ttu-id="4ea63-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4ea63-121">Header</span></span>|<span data-ttu-id="4ea63-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4ea63-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ea63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ea63-123">Authorization</span></span>|<span data-ttu-id="4ea63-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4ea63-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ea63-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4ea63-125">Accept</span></span>|<span data-ttu-id="4ea63-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ea63-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ea63-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4ea63-127">Request body</span></span>
<span data-ttu-id="4ea63-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidWorkProfileCompliancePolicy eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="4ea63-128">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="4ea63-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidWorkProfileCompliancePolicy erstellen.</span><span class="sxs-lookup"><span data-stu-id="4ea63-129">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="4ea63-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4ea63-130">Property</span></span>|<span data-ttu-id="4ea63-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4ea63-131">Type</span></span>|<span data-ttu-id="4ea63-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ea63-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ea63-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4ea63-133">roleScopeTagIds</span></span>|<span data-ttu-id="4ea63-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="4ea63-134">String collection</span></span>|<span data-ttu-id="4ea63-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="4ea63-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4ea63-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ea63-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4ea63-137">id</span><span class="sxs-lookup"><span data-stu-id="4ea63-137">id</span></span>|<span data-ttu-id="4ea63-138">String</span><span class="sxs-lookup"><span data-stu-id="4ea63-138">String</span></span>|<span data-ttu-id="4ea63-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4ea63-139">Key of the entity.</span></span> <span data-ttu-id="4ea63-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ea63-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4ea63-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ea63-141">createdDateTime</span></span>|<span data-ttu-id="4ea63-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ea63-142">DateTimeOffset</span></span>|<span data-ttu-id="4ea63-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4ea63-143">DateTime the object was created.</span></span> <span data-ttu-id="4ea63-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ea63-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4ea63-145">description</span><span class="sxs-lookup"><span data-stu-id="4ea63-145">description</span></span>|<span data-ttu-id="4ea63-146">String</span><span class="sxs-lookup"><span data-stu-id="4ea63-146">String</span></span>|<span data-ttu-id="4ea63-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4ea63-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4ea63-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ea63-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4ea63-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ea63-149">lastModifiedDateTime</span></span>|<span data-ttu-id="4ea63-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ea63-150">DateTimeOffset</span></span>|<span data-ttu-id="4ea63-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4ea63-151">DateTime the object was last modified.</span></span> <span data-ttu-id="4ea63-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ea63-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4ea63-153">displayName</span><span class="sxs-lookup"><span data-stu-id="4ea63-153">displayName</span></span>|<span data-ttu-id="4ea63-154">String</span><span class="sxs-lookup"><span data-stu-id="4ea63-154">String</span></span>|<span data-ttu-id="4ea63-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4ea63-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4ea63-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ea63-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4ea63-157">Version</span><span class="sxs-lookup"><span data-stu-id="4ea63-157">version</span></span>|<span data-ttu-id="4ea63-158">Int32</span><span class="sxs-lookup"><span data-stu-id="4ea63-158">Int32</span></span>|<span data-ttu-id="4ea63-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="4ea63-159">Version of the device configuration.</span></span> <span data-ttu-id="4ea63-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4ea63-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4ea63-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4ea63-161">passwordRequired</span></span>|<span data-ttu-id="4ea63-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ea63-162">Boolean</span></span>|<span data-ttu-id="4ea63-163">Legt fest, dass zum Entsperren des Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="4ea63-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="4ea63-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4ea63-164">passwordMinimumLength</span></span>|<span data-ttu-id="4ea63-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4ea63-165">Int32</span></span>|<span data-ttu-id="4ea63-166">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="4ea63-166">Minimum password length.</span></span> <span data-ttu-id="4ea63-167">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="4ea63-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4ea63-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4ea63-168">passwordRequiredType</span></span>|[<span data-ttu-id="4ea63-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4ea63-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="4ea63-170">Typ der Zeichen in Kennwort.</span><span class="sxs-lookup"><span data-stu-id="4ea63-170">Type of characters in password.</span></span> <span data-ttu-id="4ea63-171">Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="4ea63-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="4ea63-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4ea63-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4ea63-173">Int32</span><span class="sxs-lookup"><span data-stu-id="4ea63-173">Int32</span></span>|<span data-ttu-id="4ea63-174">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="4ea63-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="4ea63-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4ea63-175">passwordExpirationDays</span></span>|<span data-ttu-id="4ea63-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4ea63-176">Int32</span></span>|<span data-ttu-id="4ea63-177">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="4ea63-177">Number of days before the password expires.</span></span> <span data-ttu-id="4ea63-178">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="4ea63-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="4ea63-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4ea63-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4ea63-180">Int32</span><span class="sxs-lookup"><span data-stu-id="4ea63-180">Int32</span></span>|<span data-ttu-id="4ea63-181">Legt fest, wie viele der zuletzt verwendeten Kennwörter nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="4ea63-181">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="4ea63-182">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="4ea63-182">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="4ea63-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ea63-183">Boolean</span></span>|<span data-ttu-id="4ea63-184">Legt fest, dass Geräte die Installation von Apps aus unbekannten Quellen nicht zulassen dürfen.</span><span class="sxs-lookup"><span data-stu-id="4ea63-184">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="4ea63-185">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="4ea63-185">securityDisableUsbDebugging</span></span>|<span data-ttu-id="4ea63-186">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ea63-186">Boolean</span></span>|<span data-ttu-id="4ea63-187">Deaktiviert das USB-Debuggen auf Android-Geräten.</span><span class="sxs-lookup"><span data-stu-id="4ea63-187">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="4ea63-188">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="4ea63-188">securityRequireVerifyApps</span></span>|<span data-ttu-id="4ea63-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ea63-189">Boolean</span></span>|<span data-ttu-id="4ea63-190">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="4ea63-190">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="4ea63-191">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4ea63-191">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="4ea63-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ea63-192">Boolean</span></span>|<span data-ttu-id="4ea63-193">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="4ea63-193">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="4ea63-194">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4ea63-194">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="4ea63-195">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="4ea63-195">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="4ea63-196">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="4ea63-196">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="4ea63-197">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="4ea63-197">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="4ea63-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="4ea63-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="4ea63-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ea63-199">Boolean</span></span>|<span data-ttu-id="4ea63-200">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="4ea63-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="4ea63-201">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4ea63-201">osMinimumVersion</span></span>|<span data-ttu-id="4ea63-202">String</span><span class="sxs-lookup"><span data-stu-id="4ea63-202">String</span></span>|<span data-ttu-id="4ea63-203">Mindestversion von Android</span><span class="sxs-lookup"><span data-stu-id="4ea63-203">Minimum Android version.</span></span>|
|<span data-ttu-id="4ea63-204">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4ea63-204">osMaximumVersion</span></span>|<span data-ttu-id="4ea63-205">String</span><span class="sxs-lookup"><span data-stu-id="4ea63-205">String</span></span>|<span data-ttu-id="4ea63-206">Maximalversion von Android</span><span class="sxs-lookup"><span data-stu-id="4ea63-206">Maximum Android version.</span></span>|
|<span data-ttu-id="4ea63-207">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="4ea63-207">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="4ea63-208">String</span><span class="sxs-lookup"><span data-stu-id="4ea63-208">String</span></span>|<span data-ttu-id="4ea63-209">Mindestens geforderter Sicherheitspatchlevel von Android</span><span class="sxs-lookup"><span data-stu-id="4ea63-209">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="4ea63-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4ea63-210">storageRequireEncryption</span></span>|<span data-ttu-id="4ea63-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ea63-211">Boolean</span></span>|<span data-ttu-id="4ea63-212">Legt fest, dass auf Android-Geräten Verschlüsselung aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="4ea63-212">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="4ea63-213">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="4ea63-213">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="4ea63-214">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ea63-214">Boolean</span></span>|<span data-ttu-id="4ea63-215">Legt fest, dass das Gerät die SafetyNet-Basisintegritätsprüfung bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="4ea63-215">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="4ea63-216">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="4ea63-216">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="4ea63-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ea63-217">Boolean</span></span>|<span data-ttu-id="4ea63-218">Legt fest, dass das Gerät die Prüfung zum SafetyNet-zertifizierten Gerät bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="4ea63-218">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="4ea63-219">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="4ea63-219">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="4ea63-220">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ea63-220">Boolean</span></span>|<span data-ttu-id="4ea63-221">Legt fest, dass Google Play Services auf dem Gerät installiert und aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="4ea63-221">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="4ea63-222">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="4ea63-222">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="4ea63-223">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ea63-223">Boolean</span></span>|<span data-ttu-id="4ea63-224">Legt fest, dass die Sicherheitsanbieter des Geräts aktuell sein müssen.</span><span class="sxs-lookup"><span data-stu-id="4ea63-224">Require the device to have up to date security providers.</span></span> <span data-ttu-id="4ea63-225">Die aktuelle Version von Google Play Services muss auf dem Gerät installiert und aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="4ea63-225">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="4ea63-226">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="4ea63-226">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="4ea63-227">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4ea63-227">Boolean</span></span>|<span data-ttu-id="4ea63-228">Legt fest, dass das Gerät die Laufzeitintegritätsprüfung für Unternehmensportal-Client-Apps bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="4ea63-228">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="4ea63-229">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ea63-229">Response</span></span>
<span data-ttu-id="4ea63-230">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4ea63-230">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ea63-231">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ea63-231">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ea63-232">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ea63-232">Request</span></span>
<span data-ttu-id="4ea63-233">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4ea63-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1296

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="4ea63-234">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ea63-234">Response</span></span>
<span data-ttu-id="4ea63-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ea63-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1404

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




