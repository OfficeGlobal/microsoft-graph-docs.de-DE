---
title: Erstellen von „windows10MobileCompliancePolicy“
description: Diese Methode erstellt ein neues Objekt des Typs windows10MobileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 782f81110dc5fe60fd9e8fa21249fd42be9dc4c5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155566"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="bd7a5-103">Erstellen von „windows10MobileCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="bd7a5-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="bd7a5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd7a5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd7a5-106">Diese Methode erstellt ein neues Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd7a5-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd7a5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bd7a5-107">Prerequisites</span></span>
<span data-ttu-id="bd7a5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd7a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bd7a5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd7a5-110">Permission type</span></span>|<span data-ttu-id="bd7a5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd7a5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd7a5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd7a5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bd7a5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd7a5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd7a5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd7a5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd7a5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd7a5-115">Not supported.</span></span>|
|<span data-ttu-id="bd7a5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd7a5-116">Application</span></span>|<span data-ttu-id="bd7a5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd7a5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd7a5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd7a5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="bd7a5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd7a5-119">Request headers</span></span>
|<span data-ttu-id="bd7a5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bd7a5-120">Header</span></span>|<span data-ttu-id="bd7a5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="bd7a5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd7a5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd7a5-122">Authorization</span></span>|<span data-ttu-id="bd7a5-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bd7a5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd7a5-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bd7a5-124">Accept</span></span>|<span data-ttu-id="bd7a5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bd7a5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd7a5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bd7a5-126">Request body</span></span>
<span data-ttu-id="bd7a5-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10MobileCompliancePolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="bd7a5-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10MobileCompliancePolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="bd7a5-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd7a5-129">Property</span></span>|<span data-ttu-id="bd7a5-130">Typ</span><span class="sxs-lookup"><span data-stu-id="bd7a5-130">Type</span></span>|<span data-ttu-id="bd7a5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd7a5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd7a5-132">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="bd7a5-132">roleScopeTagIds</span></span>|<span data-ttu-id="bd7a5-133">String collection</span><span class="sxs-lookup"><span data-stu-id="bd7a5-133">String collection</span></span>|<span data-ttu-id="bd7a5-134">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bd7a5-135">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd7a5-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd7a5-136">id</span><span class="sxs-lookup"><span data-stu-id="bd7a5-136">id</span></span>|<span data-ttu-id="bd7a5-137">string</span><span class="sxs-lookup"><span data-stu-id="bd7a5-137">String</span></span>|<span data-ttu-id="bd7a5-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bd7a5-138">Key of the entity.</span></span> <span data-ttu-id="bd7a5-139">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd7a5-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd7a5-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd7a5-140">createdDateTime</span></span>|<span data-ttu-id="bd7a5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd7a5-141">DateTimeOffset</span></span>|<span data-ttu-id="bd7a5-142">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-142">DateTime the object was created.</span></span> <span data-ttu-id="bd7a5-143">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd7a5-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd7a5-144">description</span><span class="sxs-lookup"><span data-stu-id="bd7a5-144">description</span></span>|<span data-ttu-id="bd7a5-145">String</span><span class="sxs-lookup"><span data-stu-id="bd7a5-145">String</span></span>|<span data-ttu-id="bd7a5-146">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bd7a5-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bd7a5-147">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd7a5-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd7a5-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd7a5-148">lastModifiedDateTime</span></span>|<span data-ttu-id="bd7a5-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd7a5-149">DateTimeOffset</span></span>|<span data-ttu-id="bd7a5-150">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-150">DateTime the object was last modified.</span></span> <span data-ttu-id="bd7a5-151">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd7a5-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd7a5-152">displayName</span><span class="sxs-lookup"><span data-stu-id="bd7a5-152">displayName</span></span>|<span data-ttu-id="bd7a5-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd7a5-153">String</span></span>|<span data-ttu-id="bd7a5-154">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bd7a5-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bd7a5-155">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd7a5-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd7a5-156">Version</span><span class="sxs-lookup"><span data-stu-id="bd7a5-156">version</span></span>|<span data-ttu-id="bd7a5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="bd7a5-157">Int32</span></span>|<span data-ttu-id="bd7a5-158">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-158">Version of the device configuration.</span></span> <span data-ttu-id="bd7a5-159">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bd7a5-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bd7a5-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bd7a5-160">passwordRequired</span></span>|<span data-ttu-id="bd7a5-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd7a5-161">Boolean</span></span>|<span data-ttu-id="bd7a5-162">Legt fest, dass zum Entsperren des Windows Phone-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-162">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="bd7a5-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="bd7a5-163">passwordBlockSimple</span></span>|<span data-ttu-id="bd7a5-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd7a5-164">Boolean</span></span>|<span data-ttu-id="bd7a5-165">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-165">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="bd7a5-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bd7a5-166">passwordMinimumLength</span></span>|<span data-ttu-id="bd7a5-167">Int32</span><span class="sxs-lookup"><span data-stu-id="bd7a5-167">Int32</span></span>|<span data-ttu-id="bd7a5-168">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-168">Minimum password length.</span></span> <span data-ttu-id="bd7a5-169">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="bd7a5-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="bd7a5-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="bd7a5-171">Int32</span><span class="sxs-lookup"><span data-stu-id="bd7a5-171">Int32</span></span>|<span data-ttu-id="bd7a5-172">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="bd7a5-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="bd7a5-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bd7a5-173">passwordRequiredType</span></span>|[<span data-ttu-id="bd7a5-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bd7a5-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="bd7a5-175">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-175">The required password type.</span></span> <span data-ttu-id="bd7a5-176">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="bd7a5-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bd7a5-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bd7a5-178">Int32</span><span class="sxs-lookup"><span data-stu-id="bd7a5-178">Int32</span></span>|<span data-ttu-id="bd7a5-179">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-179">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="bd7a5-180">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bd7a5-180">passwordExpirationDays</span></span>|<span data-ttu-id="bd7a5-181">Int32</span><span class="sxs-lookup"><span data-stu-id="bd7a5-181">Int32</span></span>|<span data-ttu-id="bd7a5-182">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-182">Number of days before password expiration.</span></span> <span data-ttu-id="bd7a5-183">Gültige Werte: 1 bis 255.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-183">Valid values 1 to 255</span></span>|
|<span data-ttu-id="bd7a5-184">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="bd7a5-184">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="bd7a5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="bd7a5-185">Int32</span></span>|<span data-ttu-id="bd7a5-186">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="bd7a5-186">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="bd7a5-187">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="bd7a5-187">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="bd7a5-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd7a5-188">Boolean</span></span>|<span data-ttu-id="bd7a5-189">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-189">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="bd7a5-190">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bd7a5-190">osMinimumVersion</span></span>|<span data-ttu-id="bd7a5-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd7a5-191">String</span></span>|<span data-ttu-id="bd7a5-192">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="bd7a5-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="bd7a5-193">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bd7a5-193">osMaximumVersion</span></span>|<span data-ttu-id="bd7a5-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd7a5-194">String</span></span>|<span data-ttu-id="bd7a5-195">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="bd7a5-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="bd7a5-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="bd7a5-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="bd7a5-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd7a5-197">Boolean</span></span>|<span data-ttu-id="bd7a5-198">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="bd7a5-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="bd7a5-199">bitLockerEnabled</span></span>|<span data-ttu-id="bd7a5-200">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd7a5-200">Boolean</span></span>|<span data-ttu-id="bd7a5-201">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="bd7a5-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="bd7a5-202">secureBootEnabled</span></span>|<span data-ttu-id="bd7a5-203">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd7a5-203">Boolean</span></span>|<span data-ttu-id="bd7a5-204">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="bd7a5-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="bd7a5-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="bd7a5-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd7a5-206">Boolean</span></span>|<span data-ttu-id="bd7a5-207">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="bd7a5-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="bd7a5-208">storageRequireEncryption</span></span>|<span data-ttu-id="bd7a5-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd7a5-209">Boolean</span></span>|<span data-ttu-id="bd7a5-210">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-210">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="bd7a5-211">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="bd7a5-211">activeFirewallRequired</span></span>|<span data-ttu-id="bd7a5-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bd7a5-212">Boolean</span></span>|<span data-ttu-id="bd7a5-213">Aktive Firewall auf Windows-Geräten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-213">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="bd7a5-214">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="bd7a5-214">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="bd7a5-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="bd7a5-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="bd7a5-216">Die gültigen buildbereiche des Betriebssystems auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-216">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="bd7a5-217">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-217">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="bd7a5-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd7a5-218">Response</span></span>
<span data-ttu-id="bd7a5-219">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-219">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd7a5-220">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bd7a5-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd7a5-221">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd7a5-221">Request</span></span>
<span data-ttu-id="bd7a5-222">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1158

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="bd7a5-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd7a5-223">Response</span></span>
<span data-ttu-id="bd7a5-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd7a5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1330

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "3d4237b0-37b0-3d42-b037-423db037423d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```




