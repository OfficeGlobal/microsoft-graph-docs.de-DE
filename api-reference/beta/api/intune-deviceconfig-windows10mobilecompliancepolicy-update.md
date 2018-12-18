---
title: windows10MobileCompliancePolicy aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs windows10MobileCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: f9a040ab544d112cbe98e579eebc918c52b6f46b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341965"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="d6347-103">windows10MobileCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d6347-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="d6347-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d6347-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6347-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d6347-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6347-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d6347-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6347-107">Aktualisiert die Eigenschaften von Objekten des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6347-107">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6347-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d6347-108">Prerequisites</span></span>
<span data-ttu-id="d6347-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6347-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6347-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d6347-111">Permission type</span></span>|<span data-ttu-id="d6347-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d6347-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6347-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d6347-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6347-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6347-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6347-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d6347-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6347-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6347-116">Not supported.</span></span>|
|<span data-ttu-id="d6347-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d6347-117">Application</span></span>|<span data-ttu-id="d6347-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6347-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6347-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6347-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="d6347-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d6347-120">Request headers</span></span>
|<span data-ttu-id="d6347-121">Header</span><span class="sxs-lookup"><span data-stu-id="d6347-121">Header</span></span>|<span data-ttu-id="d6347-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d6347-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6347-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d6347-123">Authorization</span></span>|<span data-ttu-id="d6347-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d6347-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6347-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6347-125">Accept</span></span>|<span data-ttu-id="d6347-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6347-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6347-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d6347-127">Request body</span></span>
<span data-ttu-id="d6347-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d6347-128">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="d6347-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d6347-129">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="d6347-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d6347-130">Property</span></span>|<span data-ttu-id="d6347-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d6347-131">Type</span></span>|<span data-ttu-id="d6347-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6347-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6347-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d6347-133">roleScopeTagIds</span></span>|<span data-ttu-id="d6347-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="d6347-134">String collection</span></span>|<span data-ttu-id="d6347-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="d6347-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d6347-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6347-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d6347-137">id</span><span class="sxs-lookup"><span data-stu-id="d6347-137">id</span></span>|<span data-ttu-id="d6347-138">String</span><span class="sxs-lookup"><span data-stu-id="d6347-138">String</span></span>|<span data-ttu-id="d6347-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d6347-139">Key of the entity.</span></span> <span data-ttu-id="d6347-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6347-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d6347-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6347-141">createdDateTime</span></span>|<span data-ttu-id="d6347-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6347-142">DateTimeOffset</span></span>|<span data-ttu-id="d6347-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d6347-143">DateTime the object was created.</span></span> <span data-ttu-id="d6347-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6347-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d6347-145">description</span><span class="sxs-lookup"><span data-stu-id="d6347-145">description</span></span>|<span data-ttu-id="d6347-146">String</span><span class="sxs-lookup"><span data-stu-id="d6347-146">String</span></span>|<span data-ttu-id="d6347-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d6347-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d6347-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6347-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d6347-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6347-149">lastModifiedDateTime</span></span>|<span data-ttu-id="d6347-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6347-150">DateTimeOffset</span></span>|<span data-ttu-id="d6347-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="d6347-151">DateTime the object was last modified.</span></span> <span data-ttu-id="d6347-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6347-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d6347-153">displayName</span><span class="sxs-lookup"><span data-stu-id="d6347-153">displayName</span></span>|<span data-ttu-id="d6347-154">String</span><span class="sxs-lookup"><span data-stu-id="d6347-154">String</span></span>|<span data-ttu-id="d6347-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="d6347-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d6347-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6347-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d6347-157">Version</span><span class="sxs-lookup"><span data-stu-id="d6347-157">version</span></span>|<span data-ttu-id="d6347-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d6347-158">Int32</span></span>|<span data-ttu-id="d6347-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="d6347-159">Version of the device configuration.</span></span> <span data-ttu-id="d6347-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d6347-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d6347-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="d6347-161">passwordRequired</span></span>|<span data-ttu-id="d6347-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d6347-162">Boolean</span></span>|<span data-ttu-id="d6347-163">Legt fest, dass zum Entsperren des Windows Phone-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d6347-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="d6347-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d6347-164">passwordBlockSimple</span></span>|<span data-ttu-id="d6347-165">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d6347-165">Boolean</span></span>|<span data-ttu-id="d6347-166">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6347-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="d6347-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d6347-167">passwordMinimumLength</span></span>|<span data-ttu-id="d6347-168">Int32</span><span class="sxs-lookup"><span data-stu-id="d6347-168">Int32</span></span>|<span data-ttu-id="d6347-169">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="d6347-169">Minimum password length.</span></span> <span data-ttu-id="d6347-170">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="d6347-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="d6347-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d6347-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="d6347-172">Int32</span><span class="sxs-lookup"><span data-stu-id="d6347-172">Int32</span></span>|<span data-ttu-id="d6347-173">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="d6347-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="d6347-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d6347-174">passwordRequiredType</span></span>|[<span data-ttu-id="d6347-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d6347-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="d6347-176">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="d6347-176">The required password type.</span></span> <span data-ttu-id="d6347-177">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="d6347-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d6347-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d6347-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d6347-179">Int32</span><span class="sxs-lookup"><span data-stu-id="d6347-179">Int32</span></span>|<span data-ttu-id="d6347-180">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="d6347-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="d6347-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d6347-181">passwordExpirationDays</span></span>|<span data-ttu-id="d6347-182">Int32</span><span class="sxs-lookup"><span data-stu-id="d6347-182">Int32</span></span>|<span data-ttu-id="d6347-183">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="d6347-183">Number of days before password expiration.</span></span> <span data-ttu-id="d6347-184">Gültige Werte: 1 bis 255.</span><span class="sxs-lookup"><span data-stu-id="d6347-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="d6347-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d6347-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d6347-186">Int32</span><span class="sxs-lookup"><span data-stu-id="d6347-186">Int32</span></span>|<span data-ttu-id="d6347-187">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="d6347-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="d6347-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="d6347-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="d6347-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d6347-189">Boolean</span></span>|<span data-ttu-id="d6347-190">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="d6347-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="d6347-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d6347-191">osMinimumVersion</span></span>|<span data-ttu-id="d6347-192">String</span><span class="sxs-lookup"><span data-stu-id="d6347-192">String</span></span>|<span data-ttu-id="d6347-193">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="d6347-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="d6347-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d6347-194">osMaximumVersion</span></span>|<span data-ttu-id="d6347-195">String</span><span class="sxs-lookup"><span data-stu-id="d6347-195">String</span></span>|<span data-ttu-id="d6347-196">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="d6347-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="d6347-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="d6347-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="d6347-198">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d6347-198">Boolean</span></span>|<span data-ttu-id="d6347-199">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="d6347-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="d6347-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="d6347-200">bitLockerEnabled</span></span>|<span data-ttu-id="d6347-201">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d6347-201">Boolean</span></span>|<span data-ttu-id="d6347-202">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="d6347-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="d6347-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="d6347-203">secureBootEnabled</span></span>|<span data-ttu-id="d6347-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d6347-204">Boolean</span></span>|<span data-ttu-id="d6347-205">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="d6347-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="d6347-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="d6347-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="d6347-207">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d6347-207">Boolean</span></span>|<span data-ttu-id="d6347-208">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="d6347-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="d6347-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="d6347-209">storageRequireEncryption</span></span>|<span data-ttu-id="d6347-210">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d6347-210">Boolean</span></span>|<span data-ttu-id="d6347-211">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="d6347-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="d6347-212">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="d6347-212">activeFirewallRequired</span></span>|<span data-ttu-id="d6347-213">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d6347-213">Boolean</span></span>|<span data-ttu-id="d6347-214">Erfordern Sie active Firewall auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="d6347-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="d6347-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="d6347-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="d6347-216">[OperatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d6347-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="d6347-217">Das gültige Betriebssystem erstellen Bereiche auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="d6347-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="d6347-218">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="d6347-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d6347-219">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6347-219">Response</span></span>
<span data-ttu-id="d6347-220">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d6347-220">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6347-221">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d6347-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6347-222">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6347-222">Request</span></span>
<span data-ttu-id="d6347-223">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d6347-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1152

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="d6347-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6347-224">Response</span></span>
<span data-ttu-id="d6347-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d6347-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





