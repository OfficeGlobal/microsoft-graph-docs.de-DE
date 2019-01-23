---
title: Erstellen von androidWorkProfileCompliancePolicy
description: Erstellen eines neuen AndroidWorkProfileCompliancePolicy-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b650a56ab36f4fc8062eefe8cb6cbd7f23be826
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401306"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="43dcd-103">Erstellen von androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="43dcd-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="43dcd-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="43dcd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="43dcd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="43dcd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43dcd-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="43dcd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43dcd-107">Erstellen eines neuen [AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="43dcd-107">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43dcd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="43dcd-108">Prerequisites</span></span>
<span data-ttu-id="43dcd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="43dcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="43dcd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="43dcd-111">Permission type</span></span>|<span data-ttu-id="43dcd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="43dcd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43dcd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="43dcd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43dcd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43dcd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43dcd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="43dcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43dcd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43dcd-116">Not supported.</span></span>|
|<span data-ttu-id="43dcd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="43dcd-117">Application</span></span>|<span data-ttu-id="43dcd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43dcd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43dcd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43dcd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="43dcd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="43dcd-120">Request headers</span></span>
|<span data-ttu-id="43dcd-121">Header</span><span class="sxs-lookup"><span data-stu-id="43dcd-121">Header</span></span>|<span data-ttu-id="43dcd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="43dcd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43dcd-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="43dcd-123">Authorization</span></span>|<span data-ttu-id="43dcd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="43dcd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43dcd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="43dcd-125">Accept</span></span>|<span data-ttu-id="43dcd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43dcd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43dcd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="43dcd-127">Request body</span></span>
<span data-ttu-id="43dcd-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidWorkProfileCompliancePolicy eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="43dcd-128">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="43dcd-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidWorkProfileCompliancePolicy erstellen.</span><span class="sxs-lookup"><span data-stu-id="43dcd-129">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="43dcd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="43dcd-130">Property</span></span>|<span data-ttu-id="43dcd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="43dcd-131">Type</span></span>|<span data-ttu-id="43dcd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43dcd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43dcd-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="43dcd-133">roleScopeTagIds</span></span>|<span data-ttu-id="43dcd-134">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="43dcd-134">String collection</span></span>|<span data-ttu-id="43dcd-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="43dcd-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="43dcd-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="43dcd-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43dcd-137">id</span><span class="sxs-lookup"><span data-stu-id="43dcd-137">id</span></span>|<span data-ttu-id="43dcd-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="43dcd-138">String</span></span>|<span data-ttu-id="43dcd-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="43dcd-139">Key of the entity.</span></span> <span data-ttu-id="43dcd-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="43dcd-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43dcd-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43dcd-141">createdDateTime</span></span>|<span data-ttu-id="43dcd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43dcd-142">DateTimeOffset</span></span>|<span data-ttu-id="43dcd-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="43dcd-143">DateTime the object was created.</span></span> <span data-ttu-id="43dcd-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="43dcd-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43dcd-145">description</span><span class="sxs-lookup"><span data-stu-id="43dcd-145">description</span></span>|<span data-ttu-id="43dcd-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="43dcd-146">String</span></span>|<span data-ttu-id="43dcd-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="43dcd-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="43dcd-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="43dcd-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43dcd-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43dcd-149">lastModifiedDateTime</span></span>|<span data-ttu-id="43dcd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43dcd-150">DateTimeOffset</span></span>|<span data-ttu-id="43dcd-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="43dcd-151">DateTime the object was last modified.</span></span> <span data-ttu-id="43dcd-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="43dcd-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43dcd-153">displayName</span><span class="sxs-lookup"><span data-stu-id="43dcd-153">displayName</span></span>|<span data-ttu-id="43dcd-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="43dcd-154">String</span></span>|<span data-ttu-id="43dcd-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="43dcd-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="43dcd-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="43dcd-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43dcd-157">Version</span><span class="sxs-lookup"><span data-stu-id="43dcd-157">version</span></span>|<span data-ttu-id="43dcd-158">Int32</span><span class="sxs-lookup"><span data-stu-id="43dcd-158">Int32</span></span>|<span data-ttu-id="43dcd-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="43dcd-159">Version of the device configuration.</span></span> <span data-ttu-id="43dcd-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="43dcd-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="43dcd-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="43dcd-161">passwordRequired</span></span>|<span data-ttu-id="43dcd-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="43dcd-162">Boolean</span></span>|<span data-ttu-id="43dcd-163">Legt fest, dass zum Entsperren des Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="43dcd-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="43dcd-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="43dcd-164">passwordMinimumLength</span></span>|<span data-ttu-id="43dcd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="43dcd-165">Int32</span></span>|<span data-ttu-id="43dcd-166">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="43dcd-166">Minimum password length.</span></span> <span data-ttu-id="43dcd-167">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="43dcd-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="43dcd-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="43dcd-168">passwordRequiredType</span></span>|[<span data-ttu-id="43dcd-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="43dcd-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="43dcd-170">Typ der Zeichen in Kennwort.</span><span class="sxs-lookup"><span data-stu-id="43dcd-170">Type of characters in password.</span></span> <span data-ttu-id="43dcd-171">Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="43dcd-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="43dcd-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="43dcd-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="43dcd-173">Int32</span><span class="sxs-lookup"><span data-stu-id="43dcd-173">Int32</span></span>|<span data-ttu-id="43dcd-174">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="43dcd-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="43dcd-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="43dcd-175">passwordExpirationDays</span></span>|<span data-ttu-id="43dcd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="43dcd-176">Int32</span></span>|<span data-ttu-id="43dcd-177">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="43dcd-177">Number of days before the password expires.</span></span> <span data-ttu-id="43dcd-178">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="43dcd-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="43dcd-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="43dcd-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="43dcd-180">Int32</span><span class="sxs-lookup"><span data-stu-id="43dcd-180">Int32</span></span>|<span data-ttu-id="43dcd-181">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="43dcd-181">Number of previous passwords to block.</span></span> <span data-ttu-id="43dcd-182">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="43dcd-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="43dcd-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="43dcd-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="43dcd-184">Int32</span><span class="sxs-lookup"><span data-stu-id="43dcd-184">Int32</span></span>|<span data-ttu-id="43dcd-185">Anzahl der Anmeldung Fehler vor Herstellerstandard zulässig.</span><span class="sxs-lookup"><span data-stu-id="43dcd-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="43dcd-186">Gültige Werte 1 bis 16</span><span class="sxs-lookup"><span data-stu-id="43dcd-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="43dcd-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="43dcd-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="43dcd-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="43dcd-188">Boolean</span></span>|<span data-ttu-id="43dcd-189">Legt fest, dass Geräte die Installation von Apps aus unbekannten Quellen nicht zulassen dürfen.</span><span class="sxs-lookup"><span data-stu-id="43dcd-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="43dcd-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="43dcd-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="43dcd-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="43dcd-191">Boolean</span></span>|<span data-ttu-id="43dcd-192">Deaktiviert das USB-Debuggen auf Android-Geräten.</span><span class="sxs-lookup"><span data-stu-id="43dcd-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="43dcd-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="43dcd-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="43dcd-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="43dcd-194">Boolean</span></span>|<span data-ttu-id="43dcd-195">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="43dcd-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="43dcd-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="43dcd-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="43dcd-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="43dcd-197">Boolean</span></span>|<span data-ttu-id="43dcd-198">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="43dcd-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="43dcd-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="43dcd-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="43dcd-200">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="43dcd-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="43dcd-201">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="43dcd-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="43dcd-202">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="43dcd-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="43dcd-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="43dcd-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="43dcd-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="43dcd-204">Boolean</span></span>|<span data-ttu-id="43dcd-205">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="43dcd-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="43dcd-206">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="43dcd-206">osMinimumVersion</span></span>|<span data-ttu-id="43dcd-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="43dcd-207">String</span></span>|<span data-ttu-id="43dcd-208">Mindestversion von Android</span><span class="sxs-lookup"><span data-stu-id="43dcd-208">Minimum Android version.</span></span>|
|<span data-ttu-id="43dcd-209">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="43dcd-209">osMaximumVersion</span></span>|<span data-ttu-id="43dcd-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="43dcd-210">String</span></span>|<span data-ttu-id="43dcd-211">Maximalversion von Android</span><span class="sxs-lookup"><span data-stu-id="43dcd-211">Maximum Android version.</span></span>|
|<span data-ttu-id="43dcd-212">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="43dcd-212">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="43dcd-213">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="43dcd-213">String</span></span>|<span data-ttu-id="43dcd-214">Mindestens geforderter Sicherheitspatchlevel von Android</span><span class="sxs-lookup"><span data-stu-id="43dcd-214">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="43dcd-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="43dcd-215">storageRequireEncryption</span></span>|<span data-ttu-id="43dcd-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="43dcd-216">Boolean</span></span>|<span data-ttu-id="43dcd-217">Legt fest, dass auf Android-Geräten Verschlüsselung aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="43dcd-217">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="43dcd-218">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="43dcd-218">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="43dcd-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="43dcd-219">Boolean</span></span>|<span data-ttu-id="43dcd-220">Legt fest, dass das Gerät die SafetyNet-Basisintegritätsprüfung bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="43dcd-220">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="43dcd-221">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="43dcd-221">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="43dcd-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="43dcd-222">Boolean</span></span>|<span data-ttu-id="43dcd-223">Legt fest, dass das Gerät die Prüfung zum SafetyNet-zertifizierten Gerät bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="43dcd-223">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="43dcd-224">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="43dcd-224">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="43dcd-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="43dcd-225">Boolean</span></span>|<span data-ttu-id="43dcd-226">Legt fest, dass Google Play Services auf dem Gerät installiert und aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="43dcd-226">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="43dcd-227">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="43dcd-227">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="43dcd-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="43dcd-228">Boolean</span></span>|<span data-ttu-id="43dcd-229">Legt fest, dass die Sicherheitsanbieter des Geräts aktuell sein müssen.</span><span class="sxs-lookup"><span data-stu-id="43dcd-229">Require the device to have up to date security providers.</span></span> <span data-ttu-id="43dcd-230">Die aktuelle Version von Google Play Services muss auf dem Gerät installiert und aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="43dcd-230">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="43dcd-231">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="43dcd-231">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="43dcd-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="43dcd-232">Boolean</span></span>|<span data-ttu-id="43dcd-233">Legt fest, dass das Gerät die Laufzeitintegritätsprüfung für Unternehmensportal-Client-Apps bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="43dcd-233">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="43dcd-234">Antwort</span><span class="sxs-lookup"><span data-stu-id="43dcd-234">Response</span></span>
<span data-ttu-id="43dcd-235">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="43dcd-235">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43dcd-236">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43dcd-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="43dcd-237">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43dcd-237">Request</span></span>
<span data-ttu-id="43dcd-238">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43dcd-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1287

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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

### <a name="response"></a><span data-ttu-id="43dcd-239">Antwort</span><span class="sxs-lookup"><span data-stu-id="43dcd-239">Response</span></span>
<span data-ttu-id="43dcd-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43dcd-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1459

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
  "passwordSignInFailureCountBeforeFactoryReset": 12,
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




