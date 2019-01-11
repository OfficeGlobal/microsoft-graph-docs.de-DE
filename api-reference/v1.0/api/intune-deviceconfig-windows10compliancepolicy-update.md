---
title: windows10CompliancePolicy aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cd56f1f808a16bc05aa3e4f2c3fc4fb4da74a5a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892204"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="5f3d7-103">windows10CompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5f3d7-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="5f3d7-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f3d7-105">Aktualisiert die Eigenschaften von Objekten des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f3d7-105">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f3d7-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5f3d7-106">Prerequisites</span></span>
<span data-ttu-id="5f3d7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f3d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f3d7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f3d7-109">Permission type</span></span>|<span data-ttu-id="5f3d7-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f3d7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f3d7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f3d7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5f3d7-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f3d7-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5f3d7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f3d7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f3d7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f3d7-114">Not supported.</span></span>|
|<span data-ttu-id="5f3d7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f3d7-115">Application</span></span>|<span data-ttu-id="5f3d7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f3d7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f3d7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f3d7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="5f3d7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f3d7-118">Request headers</span></span>
|<span data-ttu-id="5f3d7-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5f3d7-119">Header</span></span>|<span data-ttu-id="5f3d7-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5f3d7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f3d7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f3d7-121">Authorization</span></span>|<span data-ttu-id="5f3d7-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5f3d7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f3d7-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5f3d7-123">Accept</span></span>|<span data-ttu-id="5f3d7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5f3d7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f3d7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5f3d7-125">Request body</span></span>
<span data-ttu-id="5f3d7-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-126">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="5f3d7-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-127">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="5f3d7-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f3d7-128">Property</span></span>|<span data-ttu-id="5f3d7-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5f3d7-129">Type</span></span>|<span data-ttu-id="5f3d7-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f3d7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f3d7-131">id</span><span class="sxs-lookup"><span data-stu-id="5f3d7-131">id</span></span>|<span data-ttu-id="5f3d7-132">String</span><span class="sxs-lookup"><span data-stu-id="5f3d7-132">String</span></span>|<span data-ttu-id="5f3d7-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5f3d7-133">Key of the entity.</span></span> <span data-ttu-id="5f3d7-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f3d7-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5f3d7-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f3d7-135">createdDateTime</span></span>|<span data-ttu-id="5f3d7-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f3d7-136">DateTimeOffset</span></span>|<span data-ttu-id="5f3d7-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-137">DateTime the object was created.</span></span> <span data-ttu-id="5f3d7-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f3d7-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5f3d7-139">description</span><span class="sxs-lookup"><span data-stu-id="5f3d7-139">description</span></span>|<span data-ttu-id="5f3d7-140">String</span><span class="sxs-lookup"><span data-stu-id="5f3d7-140">String</span></span>|<span data-ttu-id="5f3d7-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5f3d7-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5f3d7-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f3d7-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5f3d7-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f3d7-143">lastModifiedDateTime</span></span>|<span data-ttu-id="5f3d7-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f3d7-144">DateTimeOffset</span></span>|<span data-ttu-id="5f3d7-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-145">DateTime the object was last modified.</span></span> <span data-ttu-id="5f3d7-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f3d7-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5f3d7-147">displayName</span><span class="sxs-lookup"><span data-stu-id="5f3d7-147">displayName</span></span>|<span data-ttu-id="5f3d7-148">String</span><span class="sxs-lookup"><span data-stu-id="5f3d7-148">String</span></span>|<span data-ttu-id="5f3d7-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5f3d7-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5f3d7-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f3d7-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5f3d7-151">Version</span><span class="sxs-lookup"><span data-stu-id="5f3d7-151">version</span></span>|<span data-ttu-id="5f3d7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5f3d7-152">Int32</span></span>|<span data-ttu-id="5f3d7-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-153">Version of the device configuration.</span></span> <span data-ttu-id="5f3d7-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5f3d7-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5f3d7-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5f3d7-155">passwordRequired</span></span>|<span data-ttu-id="5f3d7-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3d7-156">Boolean</span></span>|<span data-ttu-id="5f3d7-157">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="5f3d7-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5f3d7-158">passwordBlockSimple</span></span>|<span data-ttu-id="5f3d7-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3d7-159">Boolean</span></span>|<span data-ttu-id="5f3d7-160">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="5f3d7-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="5f3d7-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="5f3d7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3d7-162">Boolean</span></span>|<span data-ttu-id="5f3d7-163">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="5f3d7-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5f3d7-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5f3d7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5f3d7-165">Int32</span></span>|<span data-ttu-id="5f3d7-166">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="5f3d7-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5f3d7-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5f3d7-167">passwordExpirationDays</span></span>|<span data-ttu-id="5f3d7-168">Int32</span><span class="sxs-lookup"><span data-stu-id="5f3d7-168">Int32</span></span>|<span data-ttu-id="5f3d7-169">Zeitraum in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="5f3d7-169">The password expiration in days.</span></span>|
|<span data-ttu-id="5f3d7-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5f3d7-170">passwordMinimumLength</span></span>|<span data-ttu-id="5f3d7-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5f3d7-171">Int32</span></span>|<span data-ttu-id="5f3d7-172">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="5f3d7-172">The minimum password length.</span></span>|
|<span data-ttu-id="5f3d7-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5f3d7-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="5f3d7-174">Int32</span><span class="sxs-lookup"><span data-stu-id="5f3d7-174">Int32</span></span>|<span data-ttu-id="5f3d7-175">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="5f3d7-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="5f3d7-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5f3d7-176">passwordRequiredType</span></span>|[<span data-ttu-id="5f3d7-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5f3d7-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5f3d7-178">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-178">The required password type.</span></span> <span data-ttu-id="5f3d7-179">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5f3d7-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5f3d7-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5f3d7-181">Int32</span><span class="sxs-lookup"><span data-stu-id="5f3d7-181">Int32</span></span>|<span data-ttu-id="5f3d7-182">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="5f3d7-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="5f3d7-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="5f3d7-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3d7-184">Boolean</span></span>|<span data-ttu-id="5f3d7-185">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="5f3d7-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5f3d7-186">osMinimumVersion</span></span>|<span data-ttu-id="5f3d7-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f3d7-187">String</span></span>|<span data-ttu-id="5f3d7-188">Mindestversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="5f3d7-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="5f3d7-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5f3d7-189">osMaximumVersion</span></span>|<span data-ttu-id="5f3d7-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f3d7-190">String</span></span>|<span data-ttu-id="5f3d7-191">Maximalversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="5f3d7-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="5f3d7-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5f3d7-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="5f3d7-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f3d7-193">String</span></span>|<span data-ttu-id="5f3d7-194">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="5f3d7-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="5f3d7-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5f3d7-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="5f3d7-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f3d7-196">String</span></span>|<span data-ttu-id="5f3d7-197">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="5f3d7-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="5f3d7-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="5f3d7-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="5f3d7-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3d7-199">Boolean</span></span>|<span data-ttu-id="5f3d7-200">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="5f3d7-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="5f3d7-201">bitLockerEnabled</span></span>|<span data-ttu-id="5f3d7-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3d7-202">Boolean</span></span>|<span data-ttu-id="5f3d7-203">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="5f3d7-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="5f3d7-204">secureBootEnabled</span></span>|<span data-ttu-id="5f3d7-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3d7-205">Boolean</span></span>|<span data-ttu-id="5f3d7-206">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="5f3d7-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="5f3d7-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="5f3d7-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3d7-208">Boolean</span></span>|<span data-ttu-id="5f3d7-209">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="5f3d7-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5f3d7-210">storageRequireEncryption</span></span>|<span data-ttu-id="5f3d7-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3d7-211">Boolean</span></span>|<span data-ttu-id="5f3d7-212">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="5f3d7-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f3d7-213">Response</span></span>
<span data-ttu-id="5f3d7-214">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-214">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f3d7-215">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f3d7-215">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f3d7-216">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f3d7-216">Request</span></span>
<span data-ttu-id="5f3d7-217">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 954

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="5f3d7-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f3d7-218">Response</span></span>
<span data-ttu-id="5f3d7-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f3d7-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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
  "storageRequireEncryption": true
}
```



