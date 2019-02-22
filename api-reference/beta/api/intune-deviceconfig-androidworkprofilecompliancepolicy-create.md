---
title: AndroidWorkProfileCompliancePolicy erstellen
description: Erstellen eines neuen androidWorkProfileCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7da32de16be0e10d313b8d281afdf927f832fc90
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150267"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="48cc2-103">AndroidWorkProfileCompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="48cc2-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="48cc2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="48cc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48cc2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="48cc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48cc2-106">Erstellen eines neuen [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="48cc2-106">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48cc2-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="48cc2-107">Prerequisites</span></span>
<span data-ttu-id="48cc2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="48cc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="48cc2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48cc2-110">Permission type</span></span>|<span data-ttu-id="48cc2-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48cc2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48cc2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48cc2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48cc2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48cc2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48cc2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48cc2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48cc2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48cc2-115">Not supported.</span></span>|
|<span data-ttu-id="48cc2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48cc2-116">Application</span></span>|<span data-ttu-id="48cc2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48cc2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48cc2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48cc2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="48cc2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48cc2-119">Request headers</span></span>
|<span data-ttu-id="48cc2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="48cc2-120">Header</span></span>|<span data-ttu-id="48cc2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="48cc2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48cc2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="48cc2-122">Authorization</span></span>|<span data-ttu-id="48cc2-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="48cc2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48cc2-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="48cc2-124">Accept</span></span>|<span data-ttu-id="48cc2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48cc2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48cc2-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48cc2-126">Request body</span></span>
<span data-ttu-id="48cc2-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidWorkProfileCompliancePolicy-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="48cc2-127">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="48cc2-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidWorkProfileCompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="48cc2-128">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="48cc2-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="48cc2-129">Property</span></span>|<span data-ttu-id="48cc2-130">Typ</span><span class="sxs-lookup"><span data-stu-id="48cc2-130">Type</span></span>|<span data-ttu-id="48cc2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48cc2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48cc2-132">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="48cc2-132">roleScopeTagIds</span></span>|<span data-ttu-id="48cc2-133">String collection</span><span class="sxs-lookup"><span data-stu-id="48cc2-133">String collection</span></span>|<span data-ttu-id="48cc2-134">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="48cc2-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="48cc2-135">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="48cc2-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="48cc2-136">id</span><span class="sxs-lookup"><span data-stu-id="48cc2-136">id</span></span>|<span data-ttu-id="48cc2-137">string</span><span class="sxs-lookup"><span data-stu-id="48cc2-137">String</span></span>|<span data-ttu-id="48cc2-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="48cc2-138">Key of the entity.</span></span> <span data-ttu-id="48cc2-139">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="48cc2-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="48cc2-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48cc2-140">createdDateTime</span></span>|<span data-ttu-id="48cc2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48cc2-141">DateTimeOffset</span></span>|<span data-ttu-id="48cc2-142">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="48cc2-142">DateTime the object was created.</span></span> <span data-ttu-id="48cc2-143">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="48cc2-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="48cc2-144">description</span><span class="sxs-lookup"><span data-stu-id="48cc2-144">description</span></span>|<span data-ttu-id="48cc2-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48cc2-145">String</span></span>|<span data-ttu-id="48cc2-146">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="48cc2-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="48cc2-147">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="48cc2-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="48cc2-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48cc2-148">lastModifiedDateTime</span></span>|<span data-ttu-id="48cc2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48cc2-149">DateTimeOffset</span></span>|<span data-ttu-id="48cc2-150">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="48cc2-150">DateTime the object was last modified.</span></span> <span data-ttu-id="48cc2-151">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="48cc2-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="48cc2-152">displayName</span><span class="sxs-lookup"><span data-stu-id="48cc2-152">displayName</span></span>|<span data-ttu-id="48cc2-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48cc2-153">String</span></span>|<span data-ttu-id="48cc2-154">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="48cc2-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="48cc2-155">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="48cc2-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="48cc2-156">Version</span><span class="sxs-lookup"><span data-stu-id="48cc2-156">version</span></span>|<span data-ttu-id="48cc2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="48cc2-157">Int32</span></span>|<span data-ttu-id="48cc2-158">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="48cc2-158">Version of the device configuration.</span></span> <span data-ttu-id="48cc2-159">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="48cc2-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="48cc2-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="48cc2-160">passwordRequired</span></span>|<span data-ttu-id="48cc2-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="48cc2-161">Boolean</span></span>|<span data-ttu-id="48cc2-162">Legt fest, dass zum Entsperren des Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="48cc2-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="48cc2-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="48cc2-163">passwordMinimumLength</span></span>|<span data-ttu-id="48cc2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="48cc2-164">Int32</span></span>|<span data-ttu-id="48cc2-165">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="48cc2-165">Minimum password length.</span></span> <span data-ttu-id="48cc2-166">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="48cc2-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="48cc2-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="48cc2-167">passwordRequiredType</span></span>|[<span data-ttu-id="48cc2-168">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="48cc2-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="48cc2-169">Typ der Zeichen im Kennwort.</span><span class="sxs-lookup"><span data-stu-id="48cc2-169">Type of characters in password.</span></span> <span data-ttu-id="48cc2-170">Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="48cc2-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="48cc2-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="48cc2-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="48cc2-172">Int32</span><span class="sxs-lookup"><span data-stu-id="48cc2-172">Int32</span></span>|<span data-ttu-id="48cc2-173">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="48cc2-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="48cc2-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="48cc2-174">passwordExpirationDays</span></span>|<span data-ttu-id="48cc2-175">Int32</span><span class="sxs-lookup"><span data-stu-id="48cc2-175">Int32</span></span>|<span data-ttu-id="48cc2-176">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="48cc2-176">Number of days before the password expires.</span></span> <span data-ttu-id="48cc2-177">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="48cc2-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="48cc2-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="48cc2-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="48cc2-179">Int32</span><span class="sxs-lookup"><span data-stu-id="48cc2-179">Int32</span></span>|<span data-ttu-id="48cc2-180">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="48cc2-180">Number of previous passwords to block.</span></span> <span data-ttu-id="48cc2-181">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="48cc2-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="48cc2-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="48cc2-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="48cc2-183">Int32</span><span class="sxs-lookup"><span data-stu-id="48cc2-183">Int32</span></span>|<span data-ttu-id="48cc2-184">Anzahl der zulässigen Anmeldefehler vor dem Zurücksetzen der Factory.</span><span class="sxs-lookup"><span data-stu-id="48cc2-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="48cc2-185">Gültige Werte 1 bis 16</span><span class="sxs-lookup"><span data-stu-id="48cc2-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="48cc2-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="48cc2-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="48cc2-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="48cc2-187">Boolean</span></span>|<span data-ttu-id="48cc2-188">Legt fest, dass Geräte die Installation von Apps aus unbekannten Quellen nicht zulassen dürfen.</span><span class="sxs-lookup"><span data-stu-id="48cc2-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="48cc2-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="48cc2-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="48cc2-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="48cc2-190">Boolean</span></span>|<span data-ttu-id="48cc2-191">Deaktiviert das USB-Debuggen auf Android-Geräten.</span><span class="sxs-lookup"><span data-stu-id="48cc2-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="48cc2-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="48cc2-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="48cc2-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="48cc2-193">Boolean</span></span>|<span data-ttu-id="48cc2-194">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="48cc2-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="48cc2-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="48cc2-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="48cc2-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="48cc2-196">Boolean</span></span>|<span data-ttu-id="48cc2-197">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="48cc2-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="48cc2-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="48cc2-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="48cc2-199">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="48cc2-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="48cc2-200">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="48cc2-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="48cc2-201">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="48cc2-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="48cc2-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="48cc2-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="48cc2-203">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="48cc2-203">Boolean</span></span>|<span data-ttu-id="48cc2-204">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="48cc2-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="48cc2-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="48cc2-205">osMinimumVersion</span></span>|<span data-ttu-id="48cc2-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48cc2-206">String</span></span>|<span data-ttu-id="48cc2-207">Mindestversion von Android</span><span class="sxs-lookup"><span data-stu-id="48cc2-207">Minimum Android version.</span></span>|
|<span data-ttu-id="48cc2-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="48cc2-208">osMaximumVersion</span></span>|<span data-ttu-id="48cc2-209">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48cc2-209">String</span></span>|<span data-ttu-id="48cc2-210">Maximalversion von Android</span><span class="sxs-lookup"><span data-stu-id="48cc2-210">Maximum Android version.</span></span>|
|<span data-ttu-id="48cc2-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="48cc2-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="48cc2-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48cc2-212">String</span></span>|<span data-ttu-id="48cc2-213">Mindestens geforderter Sicherheitspatchlevel von Android</span><span class="sxs-lookup"><span data-stu-id="48cc2-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="48cc2-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="48cc2-214">storageRequireEncryption</span></span>|<span data-ttu-id="48cc2-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="48cc2-215">Boolean</span></span>|<span data-ttu-id="48cc2-216">Legt fest, dass auf Android-Geräten Verschlüsselung aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="48cc2-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="48cc2-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="48cc2-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="48cc2-218">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="48cc2-218">Boolean</span></span>|<span data-ttu-id="48cc2-219">Legt fest, dass das Gerät die SafetyNet-Basisintegritätsprüfung bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="48cc2-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="48cc2-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="48cc2-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="48cc2-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="48cc2-221">Boolean</span></span>|<span data-ttu-id="48cc2-222">Legt fest, dass das Gerät die Prüfung zum SafetyNet-zertifizierten Gerät bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="48cc2-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="48cc2-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="48cc2-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="48cc2-224">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="48cc2-224">Boolean</span></span>|<span data-ttu-id="48cc2-225">Legt fest, dass Google Play Services auf dem Gerät installiert und aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="48cc2-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="48cc2-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="48cc2-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="48cc2-227">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="48cc2-227">Boolean</span></span>|<span data-ttu-id="48cc2-228">Legt fest, dass die Sicherheitsanbieter des Geräts aktuell sein müssen.</span><span class="sxs-lookup"><span data-stu-id="48cc2-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="48cc2-229">Die aktuelle Version von Google Play Services muss auf dem Gerät installiert und aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="48cc2-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="48cc2-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="48cc2-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="48cc2-231">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="48cc2-231">Boolean</span></span>|<span data-ttu-id="48cc2-232">Legt fest, dass das Gerät die Laufzeitintegritätsprüfung für Unternehmensportal-Client-Apps bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="48cc2-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="48cc2-233">Antwort</span><span class="sxs-lookup"><span data-stu-id="48cc2-233">Response</span></span>
<span data-ttu-id="48cc2-234">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="48cc2-234">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48cc2-235">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48cc2-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="48cc2-236">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48cc2-236">Request</span></span>
<span data-ttu-id="48cc2-237">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48cc2-237">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="48cc2-238">Antwort</span><span class="sxs-lookup"><span data-stu-id="48cc2-238">Response</span></span>
<span data-ttu-id="48cc2-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48cc2-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




