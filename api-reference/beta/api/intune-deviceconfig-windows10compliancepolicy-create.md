---
title: windows10CompliancePolicy erstellen
description: Erstellt neue Objekte des Typs windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9af661ab4397c8096b45bea8fdd199d2c78b0bd1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973866"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="e1f36-103">windows10CompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="e1f36-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="e1f36-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e1f36-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1f36-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e1f36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1f36-106">Erstellt neue Objekte des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1f36-106">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1f36-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e1f36-107">Prerequisites</span></span>
<span data-ttu-id="e1f36-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1f36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1f36-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1f36-110">Permission type</span></span>|<span data-ttu-id="e1f36-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1f36-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1f36-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1f36-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1f36-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1f36-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1f36-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1f36-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1f36-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1f36-115">Not supported.</span></span>|
|<span data-ttu-id="e1f36-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1f36-116">Application</span></span>|<span data-ttu-id="e1f36-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1f36-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1f36-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1f36-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e1f36-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1f36-119">Request headers</span></span>
|<span data-ttu-id="e1f36-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e1f36-120">Header</span></span>|<span data-ttu-id="e1f36-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1f36-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1f36-122">Authorization</span></span>|<span data-ttu-id="e1f36-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e1f36-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1f36-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e1f36-124">Accept</span></span>|<span data-ttu-id="e1f36-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1f36-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1f36-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1f36-126">Request body</span></span>
<span data-ttu-id="e1f36-127">Geben Sie im Anforderungstext eine JSON-Darstellung des windows10CompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e1f36-127">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="e1f36-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10CompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e1f36-128">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="e1f36-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1f36-129">Property</span></span>|<span data-ttu-id="e1f36-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e1f36-130">Type</span></span>|<span data-ttu-id="e1f36-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1f36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1f36-132">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="e1f36-132">roleScopeTagIds</span></span>|<span data-ttu-id="e1f36-133">String collection</span><span class="sxs-lookup"><span data-stu-id="e1f36-133">String collection</span></span>|<span data-ttu-id="e1f36-134">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="e1f36-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e1f36-135">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1f36-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1f36-136">id</span><span class="sxs-lookup"><span data-stu-id="e1f36-136">id</span></span>|<span data-ttu-id="e1f36-137">String</span><span class="sxs-lookup"><span data-stu-id="e1f36-137">String</span></span>|<span data-ttu-id="e1f36-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e1f36-138">Key of the entity.</span></span> <span data-ttu-id="e1f36-139">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1f36-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1f36-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1f36-140">createdDateTime</span></span>|<span data-ttu-id="e1f36-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1f36-141">DateTimeOffset</span></span>|<span data-ttu-id="e1f36-142">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e1f36-142">DateTime the object was created.</span></span> <span data-ttu-id="e1f36-143">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1f36-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1f36-144">description</span><span class="sxs-lookup"><span data-stu-id="e1f36-144">description</span></span>|<span data-ttu-id="e1f36-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1f36-145">String</span></span>|<span data-ttu-id="e1f36-146">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e1f36-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e1f36-147">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1f36-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1f36-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1f36-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e1f36-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1f36-149">DateTimeOffset</span></span>|<span data-ttu-id="e1f36-150">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e1f36-150">DateTime the object was last modified.</span></span> <span data-ttu-id="e1f36-151">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1f36-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1f36-152">displayName</span><span class="sxs-lookup"><span data-stu-id="e1f36-152">displayName</span></span>|<span data-ttu-id="e1f36-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1f36-153">String</span></span>|<span data-ttu-id="e1f36-154">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e1f36-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e1f36-155">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1f36-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1f36-156">Version</span><span class="sxs-lookup"><span data-stu-id="e1f36-156">version</span></span>|<span data-ttu-id="e1f36-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e1f36-157">Int32</span></span>|<span data-ttu-id="e1f36-158">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="e1f36-158">Version of the device configuration.</span></span> <span data-ttu-id="e1f36-159">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e1f36-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e1f36-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e1f36-160">passwordRequired</span></span>|<span data-ttu-id="e1f36-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-161">Boolean</span></span>|<span data-ttu-id="e1f36-162">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e1f36-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="e1f36-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e1f36-163">passwordBlockSimple</span></span>|<span data-ttu-id="e1f36-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-164">Boolean</span></span>|<span data-ttu-id="e1f36-165">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="e1f36-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="e1f36-166">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="e1f36-166">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="e1f36-167">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-167">Boolean</span></span>|<span data-ttu-id="e1f36-168">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e1f36-168">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="e1f36-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e1f36-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e1f36-170">Int32</span><span class="sxs-lookup"><span data-stu-id="e1f36-170">Int32</span></span>|<span data-ttu-id="e1f36-171">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="e1f36-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e1f36-172">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e1f36-172">passwordExpirationDays</span></span>|<span data-ttu-id="e1f36-173">Int32</span><span class="sxs-lookup"><span data-stu-id="e1f36-173">Int32</span></span>|<span data-ttu-id="e1f36-174">Zeitraum in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="e1f36-174">The password expiration in days.</span></span>|
|<span data-ttu-id="e1f36-175">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e1f36-175">passwordMinimumLength</span></span>|<span data-ttu-id="e1f36-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e1f36-176">Int32</span></span>|<span data-ttu-id="e1f36-177">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="e1f36-177">The minimum password length.</span></span>|
|<span data-ttu-id="e1f36-178">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e1f36-178">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e1f36-179">Int32</span><span class="sxs-lookup"><span data-stu-id="e1f36-179">Int32</span></span>|<span data-ttu-id="e1f36-180">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.</span><span class="sxs-lookup"><span data-stu-id="e1f36-180">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e1f36-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e1f36-181">passwordRequiredType</span></span>|[<span data-ttu-id="e1f36-182">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e1f36-182">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e1f36-183">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="e1f36-183">The required password type.</span></span> <span data-ttu-id="e1f36-184">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e1f36-184">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e1f36-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e1f36-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e1f36-186">Int32</span><span class="sxs-lookup"><span data-stu-id="e1f36-186">Int32</span></span>|<span data-ttu-id="e1f36-187">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="e1f36-187">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="e1f36-188">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="e1f36-188">requireHealthyDeviceReport</span></span>|<span data-ttu-id="e1f36-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-189">Boolean</span></span>|<span data-ttu-id="e1f36-190">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="e1f36-190">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="e1f36-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e1f36-191">osMinimumVersion</span></span>|<span data-ttu-id="e1f36-192">String</span><span class="sxs-lookup"><span data-stu-id="e1f36-192">String</span></span>|<span data-ttu-id="e1f36-193">Mindestversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="e1f36-193">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="e1f36-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e1f36-194">osMaximumVersion</span></span>|<span data-ttu-id="e1f36-195">String</span><span class="sxs-lookup"><span data-stu-id="e1f36-195">String</span></span>|<span data-ttu-id="e1f36-196">Maximalversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="e1f36-196">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="e1f36-197">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e1f36-197">mobileOsMinimumVersion</span></span>|<span data-ttu-id="e1f36-198">String</span><span class="sxs-lookup"><span data-stu-id="e1f36-198">String</span></span>|<span data-ttu-id="e1f36-199">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="e1f36-199">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="e1f36-200">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e1f36-200">mobileOsMaximumVersion</span></span>|<span data-ttu-id="e1f36-201">String</span><span class="sxs-lookup"><span data-stu-id="e1f36-201">String</span></span>|<span data-ttu-id="e1f36-202">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="e1f36-202">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="e1f36-203">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="e1f36-203">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="e1f36-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-204">Boolean</span></span>|<span data-ttu-id="e1f36-205">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="e1f36-205">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="e1f36-206">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="e1f36-206">bitLockerEnabled</span></span>|<span data-ttu-id="e1f36-207">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-207">Boolean</span></span>|<span data-ttu-id="e1f36-208">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="e1f36-208">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="e1f36-209">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="e1f36-209">secureBootEnabled</span></span>|<span data-ttu-id="e1f36-210">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-210">Boolean</span></span>|<span data-ttu-id="e1f36-211">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="e1f36-211">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="e1f36-212">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="e1f36-212">codeIntegrityEnabled</span></span>|<span data-ttu-id="e1f36-213">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-213">Boolean</span></span>|<span data-ttu-id="e1f36-214">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="e1f36-214">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="e1f36-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e1f36-215">storageRequireEncryption</span></span>|<span data-ttu-id="e1f36-216">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-216">Boolean</span></span>|<span data-ttu-id="e1f36-217">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="e1f36-217">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="e1f36-218">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="e1f36-218">activeFirewallRequired</span></span>|<span data-ttu-id="e1f36-219">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-219">Boolean</span></span>|<span data-ttu-id="e1f36-220">Aktive Firewall auf Windows-Geräten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e1f36-220">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="e1f36-221">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="e1f36-221">defenderEnabled</span></span>|<span data-ttu-id="e1f36-222">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-222">Boolean</span></span>|<span data-ttu-id="e1f36-223">Windows Defender-Antischadsoftware auf Windows-Geräten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e1f36-223">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="e1f36-224">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="e1f36-224">defenderVersion</span></span>|<span data-ttu-id="e1f36-225">String</span><span class="sxs-lookup"><span data-stu-id="e1f36-225">String</span></span>|<span data-ttu-id="e1f36-226">Mindestversion von Windows Defender Antischadsoftware auf Windows-Geräten</span><span class="sxs-lookup"><span data-stu-id="e1f36-226">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="e1f36-227">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="e1f36-227">signatureOutOfDate</span></span>|<span data-ttu-id="e1f36-228">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-228">Boolean</span></span>|<span data-ttu-id="e1f36-229">Windows Defender-Antischadsoftware-Signatur muss auf Windows-Geräten auf dem neuesten Stand sein.</span><span class="sxs-lookup"><span data-stu-id="e1f36-229">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="e1f36-230">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="e1f36-230">rtpEnabled</span></span>|<span data-ttu-id="e1f36-231">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-231">Boolean</span></span>|<span data-ttu-id="e1f36-232">Windows Defender-Antischadsoftware-Echtzeitschutz auf Windows-Geräten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e1f36-232">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="e1f36-233">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="e1f36-233">antivirusRequired</span></span>|<span data-ttu-id="e1f36-234">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-234">Boolean</span></span>|<span data-ttu-id="e1f36-235">Erfordern Sie eine Antivirus-Lösung, die mit Windows Decurity Center registriert ist, um ein-und zu überwachen (beispielsweise Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="e1f36-235">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="e1f36-236">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="e1f36-236">antiSpywareRequired</span></span>|<span data-ttu-id="e1f36-237">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-237">Boolean</span></span>|<span data-ttu-id="e1f36-238">Fordern Sie eine beliebige antiSpywarelösung an, die mit Windows Decurity Center registriert ist, um eingeschaltet und überwacht zu werden (z. b. Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="e1f36-238">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="e1f36-239">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="e1f36-239">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="e1f36-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="e1f36-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="e1f36-241">Die gültigen buildbereiche des Betriebssystems auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="e1f36-241">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="e1f36-242">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="e1f36-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="e1f36-243">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e1f36-243">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="e1f36-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1f36-244">Boolean</span></span>|<span data-ttu-id="e1f36-245">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="e1f36-245">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="e1f36-246">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e1f36-246">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="e1f36-247">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="e1f36-247">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="e1f36-248">Mindestrisiko für Geräte Bedrohungsstufe zum Melden der Nichtkonformität.</span><span class="sxs-lookup"><span data-stu-id="e1f36-248">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="e1f36-249">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="e1f36-249">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="e1f36-250">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="e1f36-250">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="e1f36-251">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-251">Boolean</span></span>|<span data-ttu-id="e1f36-252">Beachten Sie, dass der SCCM-Konformitätsstatus für den InTune-KonformitätsStatus berücksichtigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="e1f36-252">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="e1f36-253">tpmRequired</span><span class="sxs-lookup"><span data-stu-id="e1f36-253">tpmRequired</span></span>|<span data-ttu-id="e1f36-254">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e1f36-254">Boolean</span></span>|<span data-ttu-id="e1f36-255">Es muss ein Trusted Platform Module (TPM) vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="e1f36-255">Require Trusted Platform Module(TPM) to be present.</span></span>|



## <a name="response"></a><span data-ttu-id="e1f36-256">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1f36-256">Response</span></span>
<span data-ttu-id="e1f36-257">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1f36-257">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1f36-258">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1f36-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1f36-259">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1f36-259">Request</span></span>
<span data-ttu-id="e1f36-260">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1f36-260">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1690

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true
}
```

### <a name="response"></a><span data-ttu-id="e1f36-261">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1f36-261">Response</span></span>
<span data-ttu-id="e1f36-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1f36-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1862

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true
}
```




