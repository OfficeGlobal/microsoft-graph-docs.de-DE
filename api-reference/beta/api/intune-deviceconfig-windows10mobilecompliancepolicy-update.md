---
title: windows10MobileCompliancePolicy aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs windows10MobileCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1627513307aeca2ab198ccd75a273a79ee3b1ea
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408502"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="0bbdf-103">windows10MobileCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0bbdf-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="0bbdf-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0bbdf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0bbdf-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bbdf-107">Aktualisiert die Eigenschaften von Objekten des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0bbdf-107">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bbdf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0bbdf-108">Prerequisites</span></span>
<span data-ttu-id="0bbdf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0bbdf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0bbdf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0bbdf-111">Permission type</span></span>|<span data-ttu-id="0bbdf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0bbdf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bbdf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0bbdf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bbdf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bbdf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0bbdf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0bbdf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bbdf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bbdf-116">Not supported.</span></span>|
|<span data-ttu-id="0bbdf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0bbdf-117">Application</span></span>|<span data-ttu-id="0bbdf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0bbdf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bbdf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bbdf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="0bbdf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0bbdf-120">Request headers</span></span>
|<span data-ttu-id="0bbdf-121">Header</span><span class="sxs-lookup"><span data-stu-id="0bbdf-121">Header</span></span>|<span data-ttu-id="0bbdf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0bbdf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bbdf-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0bbdf-123">Authorization</span></span>|<span data-ttu-id="0bbdf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0bbdf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bbdf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0bbdf-125">Accept</span></span>|<span data-ttu-id="0bbdf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bbdf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bbdf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0bbdf-127">Request body</span></span>
<span data-ttu-id="0bbdf-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-128">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="0bbdf-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-129">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="0bbdf-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0bbdf-130">Property</span></span>|<span data-ttu-id="0bbdf-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0bbdf-131">Type</span></span>|<span data-ttu-id="0bbdf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0bbdf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bbdf-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0bbdf-133">roleScopeTagIds</span></span>|<span data-ttu-id="0bbdf-134">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="0bbdf-134">String collection</span></span>|<span data-ttu-id="0bbdf-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0bbdf-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0bbdf-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0bbdf-137">id</span><span class="sxs-lookup"><span data-stu-id="0bbdf-137">id</span></span>|<span data-ttu-id="0bbdf-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bbdf-138">String</span></span>|<span data-ttu-id="0bbdf-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0bbdf-139">Key of the entity.</span></span> <span data-ttu-id="0bbdf-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0bbdf-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0bbdf-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0bbdf-141">createdDateTime</span></span>|<span data-ttu-id="0bbdf-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bbdf-142">DateTimeOffset</span></span>|<span data-ttu-id="0bbdf-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-143">DateTime the object was created.</span></span> <span data-ttu-id="0bbdf-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0bbdf-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0bbdf-145">description</span><span class="sxs-lookup"><span data-stu-id="0bbdf-145">description</span></span>|<span data-ttu-id="0bbdf-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bbdf-146">String</span></span>|<span data-ttu-id="0bbdf-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0bbdf-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0bbdf-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0bbdf-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0bbdf-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bbdf-149">lastModifiedDateTime</span></span>|<span data-ttu-id="0bbdf-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bbdf-150">DateTimeOffset</span></span>|<span data-ttu-id="0bbdf-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-151">DateTime the object was last modified.</span></span> <span data-ttu-id="0bbdf-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0bbdf-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0bbdf-153">displayName</span><span class="sxs-lookup"><span data-stu-id="0bbdf-153">displayName</span></span>|<span data-ttu-id="0bbdf-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bbdf-154">String</span></span>|<span data-ttu-id="0bbdf-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0bbdf-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0bbdf-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0bbdf-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0bbdf-157">Version</span><span class="sxs-lookup"><span data-stu-id="0bbdf-157">version</span></span>|<span data-ttu-id="0bbdf-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0bbdf-158">Int32</span></span>|<span data-ttu-id="0bbdf-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-159">Version of the device configuration.</span></span> <span data-ttu-id="0bbdf-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0bbdf-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0bbdf-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0bbdf-161">passwordRequired</span></span>|<span data-ttu-id="0bbdf-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bbdf-162">Boolean</span></span>|<span data-ttu-id="0bbdf-163">Legt fest, dass zum Entsperren des Windows Phone-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="0bbdf-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0bbdf-164">passwordBlockSimple</span></span>|<span data-ttu-id="0bbdf-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bbdf-165">Boolean</span></span>|<span data-ttu-id="0bbdf-166">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="0bbdf-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0bbdf-167">passwordMinimumLength</span></span>|<span data-ttu-id="0bbdf-168">Int32</span><span class="sxs-lookup"><span data-stu-id="0bbdf-168">Int32</span></span>|<span data-ttu-id="0bbdf-169">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-169">Minimum password length.</span></span> <span data-ttu-id="0bbdf-170">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="0bbdf-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0bbdf-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0bbdf-172">Int32</span><span class="sxs-lookup"><span data-stu-id="0bbdf-172">Int32</span></span>|<span data-ttu-id="0bbdf-173">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="0bbdf-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0bbdf-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0bbdf-174">passwordRequiredType</span></span>|[<span data-ttu-id="0bbdf-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0bbdf-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0bbdf-176">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-176">The required password type.</span></span> <span data-ttu-id="0bbdf-177">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0bbdf-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0bbdf-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0bbdf-179">Int32</span><span class="sxs-lookup"><span data-stu-id="0bbdf-179">Int32</span></span>|<span data-ttu-id="0bbdf-180">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="0bbdf-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0bbdf-181">passwordExpirationDays</span></span>|<span data-ttu-id="0bbdf-182">Int32</span><span class="sxs-lookup"><span data-stu-id="0bbdf-182">Int32</span></span>|<span data-ttu-id="0bbdf-183">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-183">Number of days before password expiration.</span></span> <span data-ttu-id="0bbdf-184">Gültige Werte: 1 bis 255.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="0bbdf-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0bbdf-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0bbdf-186">Int32</span><span class="sxs-lookup"><span data-stu-id="0bbdf-186">Int32</span></span>|<span data-ttu-id="0bbdf-187">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="0bbdf-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0bbdf-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="0bbdf-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="0bbdf-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bbdf-189">Boolean</span></span>|<span data-ttu-id="0bbdf-190">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="0bbdf-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0bbdf-191">osMinimumVersion</span></span>|<span data-ttu-id="0bbdf-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bbdf-192">String</span></span>|<span data-ttu-id="0bbdf-193">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="0bbdf-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="0bbdf-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0bbdf-194">osMaximumVersion</span></span>|<span data-ttu-id="0bbdf-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0bbdf-195">String</span></span>|<span data-ttu-id="0bbdf-196">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="0bbdf-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="0bbdf-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="0bbdf-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="0bbdf-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bbdf-198">Boolean</span></span>|<span data-ttu-id="0bbdf-199">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="0bbdf-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="0bbdf-200">bitLockerEnabled</span></span>|<span data-ttu-id="0bbdf-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bbdf-201">Boolean</span></span>|<span data-ttu-id="0bbdf-202">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="0bbdf-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="0bbdf-203">secureBootEnabled</span></span>|<span data-ttu-id="0bbdf-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bbdf-204">Boolean</span></span>|<span data-ttu-id="0bbdf-205">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="0bbdf-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="0bbdf-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="0bbdf-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bbdf-207">Boolean</span></span>|<span data-ttu-id="0bbdf-208">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="0bbdf-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0bbdf-209">storageRequireEncryption</span></span>|<span data-ttu-id="0bbdf-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bbdf-210">Boolean</span></span>|<span data-ttu-id="0bbdf-211">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="0bbdf-212">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="0bbdf-212">activeFirewallRequired</span></span>|<span data-ttu-id="0bbdf-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bbdf-213">Boolean</span></span>|<span data-ttu-id="0bbdf-214">Erfordern Sie active Firewall auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="0bbdf-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="0bbdf-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="0bbdf-216">[OperatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0bbdf-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="0bbdf-217">Das gültige Betriebssystem erstellen Bereiche auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="0bbdf-218">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0bbdf-219">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bbdf-219">Response</span></span>
<span data-ttu-id="0bbdf-220">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-220">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bbdf-221">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0bbdf-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bbdf-222">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0bbdf-222">Request</span></span>
<span data-ttu-id="0bbdf-223">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="0bbdf-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="0bbdf-224">Response</span></span>
<span data-ttu-id="0bbdf-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0bbdf-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




