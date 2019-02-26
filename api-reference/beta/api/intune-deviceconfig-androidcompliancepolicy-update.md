---
title: Aktualisieren von „androidCompliancePolicy“
description: Aktualisieren der Eigenschaften eines androidCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 45321b43ce282015ef0a4ae8de54606667ed2a2c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142868"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="a1218-103">Aktualisieren von „androidCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="a1218-103">Update androidCompliancePolicy</span></span>

> <span data-ttu-id="a1218-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1218-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1218-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a1218-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1218-106">Aktualisieren der Eigenschaften eines [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a1218-106">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1218-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a1218-107">Prerequisites</span></span>
<span data-ttu-id="a1218-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a1218-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a1218-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a1218-110">Permission type</span></span>|<span data-ttu-id="a1218-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a1218-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1218-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a1218-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1218-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1218-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1218-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a1218-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1218-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1218-115">Not supported.</span></span>|
|<span data-ttu-id="a1218-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a1218-116">Application</span></span>|<span data-ttu-id="a1218-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1218-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1218-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1218-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="a1218-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a1218-119">Request headers</span></span>
|<span data-ttu-id="a1218-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a1218-120">Header</span></span>|<span data-ttu-id="a1218-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a1218-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1218-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1218-122">Authorization</span></span>|<span data-ttu-id="a1218-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a1218-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1218-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a1218-124">Accept</span></span>|<span data-ttu-id="a1218-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1218-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1218-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a1218-126">Request body</span></span>
<span data-ttu-id="a1218-127">Geben Sie im Anforderungstext eine JSON Darstellung für das [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="a1218-127">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="a1218-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a1218-128">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="a1218-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a1218-129">Property</span></span>|<span data-ttu-id="a1218-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a1218-130">Type</span></span>|<span data-ttu-id="a1218-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1218-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1218-132">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="a1218-132">roleScopeTagIds</span></span>|<span data-ttu-id="a1218-133">String collection</span><span class="sxs-lookup"><span data-stu-id="a1218-133">String collection</span></span>|<span data-ttu-id="a1218-134">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="a1218-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a1218-135">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1218-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1218-136">id</span><span class="sxs-lookup"><span data-stu-id="a1218-136">id</span></span>|<span data-ttu-id="a1218-137">string</span><span class="sxs-lookup"><span data-stu-id="a1218-137">String</span></span>|<span data-ttu-id="a1218-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a1218-138">Key of the entity.</span></span> <span data-ttu-id="a1218-139">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1218-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1218-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1218-140">createdDateTime</span></span>|<span data-ttu-id="a1218-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1218-141">DateTimeOffset</span></span>|<span data-ttu-id="a1218-142">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a1218-142">DateTime the object was created.</span></span> <span data-ttu-id="a1218-143">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1218-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1218-144">description</span><span class="sxs-lookup"><span data-stu-id="a1218-144">description</span></span>|<span data-ttu-id="a1218-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1218-145">String</span></span>|<span data-ttu-id="a1218-146">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a1218-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a1218-147">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1218-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1218-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1218-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a1218-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1218-149">DateTimeOffset</span></span>|<span data-ttu-id="a1218-150">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a1218-150">DateTime the object was last modified.</span></span> <span data-ttu-id="a1218-151">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1218-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1218-152">displayName</span><span class="sxs-lookup"><span data-stu-id="a1218-152">displayName</span></span>|<span data-ttu-id="a1218-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1218-153">String</span></span>|<span data-ttu-id="a1218-154">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a1218-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a1218-155">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1218-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1218-156">Version</span><span class="sxs-lookup"><span data-stu-id="a1218-156">version</span></span>|<span data-ttu-id="a1218-157">Int32</span><span class="sxs-lookup"><span data-stu-id="a1218-157">Int32</span></span>|<span data-ttu-id="a1218-158">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a1218-158">Version of the device configuration.</span></span> <span data-ttu-id="a1218-159">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1218-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1218-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="a1218-160">passwordRequired</span></span>|<span data-ttu-id="a1218-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1218-161">Boolean</span></span>|<span data-ttu-id="a1218-162">Legt fest, dass zum Entsperren des Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a1218-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="a1218-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a1218-163">passwordMinimumLength</span></span>|<span data-ttu-id="a1218-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a1218-164">Int32</span></span>|<span data-ttu-id="a1218-165">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="a1218-165">Minimum password length.</span></span> <span data-ttu-id="a1218-166">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="a1218-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a1218-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a1218-167">passwordRequiredType</span></span>|[<span data-ttu-id="a1218-168">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a1218-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="a1218-169">Typ der Zeichen im Kennwort.</span><span class="sxs-lookup"><span data-stu-id="a1218-169">Type of characters in password.</span></span> <span data-ttu-id="a1218-170">Mögliche Werte sind: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex` und `any`.</span><span class="sxs-lookup"><span data-stu-id="a1218-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="a1218-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a1218-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a1218-172">Int32</span><span class="sxs-lookup"><span data-stu-id="a1218-172">Int32</span></span>|<span data-ttu-id="a1218-173">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="a1218-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="a1218-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a1218-174">passwordExpirationDays</span></span>|<span data-ttu-id="a1218-175">Int32</span><span class="sxs-lookup"><span data-stu-id="a1218-175">Int32</span></span>|<span data-ttu-id="a1218-176">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="a1218-176">Number of days before the password expires.</span></span> <span data-ttu-id="a1218-177">Gültige Werte: 1 bis 365.</span><span class="sxs-lookup"><span data-stu-id="a1218-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="a1218-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a1218-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a1218-179">Int32</span><span class="sxs-lookup"><span data-stu-id="a1218-179">Int32</span></span>|<span data-ttu-id="a1218-180">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="a1218-180">Number of previous passwords to block.</span></span> <span data-ttu-id="a1218-181">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="a1218-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a1218-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a1218-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a1218-183">Int32</span><span class="sxs-lookup"><span data-stu-id="a1218-183">Int32</span></span>|<span data-ttu-id="a1218-184">Anzahl der zulässigen Anmeldefehler vor dem Zurücksetzen der Factory.</span><span class="sxs-lookup"><span data-stu-id="a1218-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="a1218-185">Gültige Werte 1 bis 16</span><span class="sxs-lookup"><span data-stu-id="a1218-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="a1218-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="a1218-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="a1218-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1218-187">Boolean</span></span>|<span data-ttu-id="a1218-188">Legt fest, dass Geräte die Installation von Apps aus unbekannten Quellen nicht zulassen dürfen.</span><span class="sxs-lookup"><span data-stu-id="a1218-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="a1218-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="a1218-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="a1218-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a1218-190">Boolean</span></span>|<span data-ttu-id="a1218-191">Deaktiviert das USB-Debuggen auf Android-Geräten.</span><span class="sxs-lookup"><span data-stu-id="a1218-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="a1218-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="a1218-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="a1218-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1218-193">Boolean</span></span>|<span data-ttu-id="a1218-194">Legt fest, dass die Android-Funktion „Verify Apps“ aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="a1218-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="a1218-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a1218-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="a1218-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1218-196">Boolean</span></span>|<span data-ttu-id="a1218-197">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="a1218-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="a1218-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="a1218-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="a1218-199">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="a1218-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="a1218-200">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="a1218-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="a1218-201">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="a1218-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="a1218-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="a1218-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="a1218-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1218-203">Boolean</span></span>|<span data-ttu-id="a1218-204">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="a1218-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="a1218-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="a1218-205">osMinimumVersion</span></span>|<span data-ttu-id="a1218-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1218-206">String</span></span>|<span data-ttu-id="a1218-207">Mindestversion von Android</span><span class="sxs-lookup"><span data-stu-id="a1218-207">Minimum Android version.</span></span>|
|<span data-ttu-id="a1218-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="a1218-208">osMaximumVersion</span></span>|<span data-ttu-id="a1218-209">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1218-209">String</span></span>|<span data-ttu-id="a1218-210">Maximalversion von Android</span><span class="sxs-lookup"><span data-stu-id="a1218-210">Maximum Android version.</span></span>|
|<span data-ttu-id="a1218-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="a1218-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="a1218-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1218-212">String</span></span>|<span data-ttu-id="a1218-213">Mindestens geforderter Sicherheitspatchlevel von Android</span><span class="sxs-lookup"><span data-stu-id="a1218-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="a1218-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="a1218-214">storageRequireEncryption</span></span>|<span data-ttu-id="a1218-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1218-215">Boolean</span></span>|<span data-ttu-id="a1218-216">Legt fest, dass auf Android-Geräten Verschlüsselung aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="a1218-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="a1218-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="a1218-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="a1218-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1218-218">Boolean</span></span>|<span data-ttu-id="a1218-219">Legt fest, dass das Gerät die SafetyNet-Basisintegritätsprüfung bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="a1218-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="a1218-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="a1218-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="a1218-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1218-221">Boolean</span></span>|<span data-ttu-id="a1218-222">Legt fest, dass das Gerät die Prüfung zum SafetyNet-zertifizierten Gerät bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="a1218-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="a1218-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="a1218-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="a1218-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1218-224">Boolean</span></span>|<span data-ttu-id="a1218-225">Legt fest, dass Google Play Services auf dem Gerät installiert und aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="a1218-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="a1218-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="a1218-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="a1218-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1218-227">Boolean</span></span>|<span data-ttu-id="a1218-228">Legt fest, dass die Sicherheitsanbieter des Geräts aktuell sein müssen.</span><span class="sxs-lookup"><span data-stu-id="a1218-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="a1218-229">Die aktuelle Version von Google Play Services muss auf dem Gerät installiert und aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="a1218-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="a1218-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="a1218-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="a1218-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1218-231">Boolean</span></span>|<span data-ttu-id="a1218-232">Legt fest, dass das Gerät die Laufzeitintegritätsprüfung für Unternehmensportal-Client-Apps bestanden haben muss.</span><span class="sxs-lookup"><span data-stu-id="a1218-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="a1218-233">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="a1218-233">conditionStatementId</span></span>|<span data-ttu-id="a1218-234">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1218-234">String</span></span>|<span data-ttu-id="a1218-235">ID der Bedingungsanweisung.</span><span class="sxs-lookup"><span data-stu-id="a1218-235">Condition statement id.</span></span>|
|<span data-ttu-id="a1218-236">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="a1218-236">restrictedApps</span></span>|<span data-ttu-id="a1218-237">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="a1218-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a1218-238">Das Gerät muss nicht über die angegebenen apps verfügen.</span><span class="sxs-lookup"><span data-stu-id="a1218-238">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="a1218-239">Diese Auflistung kann maximal 100 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a1218-239">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a1218-240">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1218-240">Response</span></span>
<span data-ttu-id="a1218-241">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a1218-241">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1218-242">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1218-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1218-243">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1218-243">Request</span></span>
<span data-ttu-id="a1218-244">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a1218-244">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1588

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a1218-245">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1218-245">Response</span></span>
<span data-ttu-id="a1218-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1218-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1760

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```




