---
title: windows10CompliancePolicy aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4bf282178554c5408fbdc0675eafbc5daa95079d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973691"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="2acdf-103">windows10CompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2acdf-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="2acdf-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2acdf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2acdf-105">Aktualisiert die Eigenschaften von Objekten des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2acdf-105">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2acdf-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2acdf-106">Prerequisites</span></span>
<span data-ttu-id="2acdf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2acdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2acdf-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2acdf-109">Permission type</span></span>|<span data-ttu-id="2acdf-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2acdf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2acdf-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2acdf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2acdf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2acdf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2acdf-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2acdf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2acdf-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2acdf-114">Not supported.</span></span>|
|<span data-ttu-id="2acdf-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2acdf-115">Application</span></span>|<span data-ttu-id="2acdf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2acdf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2acdf-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2acdf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="2acdf-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2acdf-118">Request headers</span></span>
|<span data-ttu-id="2acdf-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2acdf-119">Header</span></span>|<span data-ttu-id="2acdf-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2acdf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2acdf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2acdf-121">Authorization</span></span>|<span data-ttu-id="2acdf-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2acdf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2acdf-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2acdf-123">Accept</span></span>|<span data-ttu-id="2acdf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2acdf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2acdf-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2acdf-125">Request body</span></span>
<span data-ttu-id="2acdf-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2acdf-126">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="2acdf-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2acdf-127">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="2acdf-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2acdf-128">Property</span></span>|<span data-ttu-id="2acdf-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2acdf-129">Type</span></span>|<span data-ttu-id="2acdf-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2acdf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2acdf-131">id</span><span class="sxs-lookup"><span data-stu-id="2acdf-131">id</span></span>|<span data-ttu-id="2acdf-132">String</span><span class="sxs-lookup"><span data-stu-id="2acdf-132">String</span></span>|<span data-ttu-id="2acdf-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2acdf-133">Key of the entity.</span></span> <span data-ttu-id="2acdf-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2acdf-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2acdf-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2acdf-135">createdDateTime</span></span>|<span data-ttu-id="2acdf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2acdf-136">DateTimeOffset</span></span>|<span data-ttu-id="2acdf-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="2acdf-137">DateTime the object was created.</span></span> <span data-ttu-id="2acdf-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2acdf-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2acdf-139">description</span><span class="sxs-lookup"><span data-stu-id="2acdf-139">description</span></span>|<span data-ttu-id="2acdf-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2acdf-140">String</span></span>|<span data-ttu-id="2acdf-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="2acdf-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2acdf-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2acdf-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2acdf-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2acdf-143">lastModifiedDateTime</span></span>|<span data-ttu-id="2acdf-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2acdf-144">DateTimeOffset</span></span>|<span data-ttu-id="2acdf-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="2acdf-145">DateTime the object was last modified.</span></span> <span data-ttu-id="2acdf-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2acdf-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2acdf-147">displayName</span><span class="sxs-lookup"><span data-stu-id="2acdf-147">displayName</span></span>|<span data-ttu-id="2acdf-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2acdf-148">String</span></span>|<span data-ttu-id="2acdf-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="2acdf-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2acdf-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2acdf-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2acdf-151">Version</span><span class="sxs-lookup"><span data-stu-id="2acdf-151">version</span></span>|<span data-ttu-id="2acdf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2acdf-152">Int32</span></span>|<span data-ttu-id="2acdf-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="2acdf-153">Version of the device configuration.</span></span> <span data-ttu-id="2acdf-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2acdf-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2acdf-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2acdf-155">passwordRequired</span></span>|<span data-ttu-id="2acdf-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2acdf-156">Boolean</span></span>|<span data-ttu-id="2acdf-157">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="2acdf-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="2acdf-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="2acdf-158">passwordBlockSimple</span></span>|<span data-ttu-id="2acdf-159">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2acdf-159">Boolean</span></span>|<span data-ttu-id="2acdf-160">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="2acdf-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="2acdf-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="2acdf-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="2acdf-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2acdf-162">Boolean</span></span>|<span data-ttu-id="2acdf-163">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="2acdf-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="2acdf-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2acdf-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2acdf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2acdf-165">Int32</span></span>|<span data-ttu-id="2acdf-166">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="2acdf-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="2acdf-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2acdf-167">passwordExpirationDays</span></span>|<span data-ttu-id="2acdf-168">Int32</span><span class="sxs-lookup"><span data-stu-id="2acdf-168">Int32</span></span>|<span data-ttu-id="2acdf-169">Zeitraum in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="2acdf-169">The password expiration in days.</span></span>|
|<span data-ttu-id="2acdf-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2acdf-170">passwordMinimumLength</span></span>|<span data-ttu-id="2acdf-171">Int32</span><span class="sxs-lookup"><span data-stu-id="2acdf-171">Int32</span></span>|<span data-ttu-id="2acdf-172">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="2acdf-172">The minimum password length.</span></span>|
|<span data-ttu-id="2acdf-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2acdf-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="2acdf-174">Int32</span><span class="sxs-lookup"><span data-stu-id="2acdf-174">Int32</span></span>|<span data-ttu-id="2acdf-175">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.</span><span class="sxs-lookup"><span data-stu-id="2acdf-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="2acdf-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2acdf-176">passwordRequiredType</span></span>|[<span data-ttu-id="2acdf-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2acdf-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2acdf-178">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="2acdf-178">The required password type.</span></span> <span data-ttu-id="2acdf-179">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="2acdf-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2acdf-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2acdf-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2acdf-181">Int32</span><span class="sxs-lookup"><span data-stu-id="2acdf-181">Int32</span></span>|<span data-ttu-id="2acdf-182">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="2acdf-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="2acdf-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="2acdf-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="2acdf-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2acdf-184">Boolean</span></span>|<span data-ttu-id="2acdf-185">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="2acdf-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="2acdf-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2acdf-186">osMinimumVersion</span></span>|<span data-ttu-id="2acdf-187">String</span><span class="sxs-lookup"><span data-stu-id="2acdf-187">String</span></span>|<span data-ttu-id="2acdf-188">Mindestversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="2acdf-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="2acdf-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2acdf-189">osMaximumVersion</span></span>|<span data-ttu-id="2acdf-190">String</span><span class="sxs-lookup"><span data-stu-id="2acdf-190">String</span></span>|<span data-ttu-id="2acdf-191">Maximalversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="2acdf-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="2acdf-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2acdf-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="2acdf-193">String</span><span class="sxs-lookup"><span data-stu-id="2acdf-193">String</span></span>|<span data-ttu-id="2acdf-194">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="2acdf-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="2acdf-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2acdf-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="2acdf-196">String</span><span class="sxs-lookup"><span data-stu-id="2acdf-196">String</span></span>|<span data-ttu-id="2acdf-197">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="2acdf-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="2acdf-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="2acdf-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="2acdf-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2acdf-199">Boolean</span></span>|<span data-ttu-id="2acdf-200">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="2acdf-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="2acdf-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="2acdf-201">bitLockerEnabled</span></span>|<span data-ttu-id="2acdf-202">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2acdf-202">Boolean</span></span>|<span data-ttu-id="2acdf-203">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="2acdf-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="2acdf-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="2acdf-204">secureBootEnabled</span></span>|<span data-ttu-id="2acdf-205">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2acdf-205">Boolean</span></span>|<span data-ttu-id="2acdf-206">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="2acdf-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="2acdf-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="2acdf-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="2acdf-208">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2acdf-208">Boolean</span></span>|<span data-ttu-id="2acdf-209">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="2acdf-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="2acdf-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="2acdf-210">storageRequireEncryption</span></span>|<span data-ttu-id="2acdf-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2acdf-211">Boolean</span></span>|<span data-ttu-id="2acdf-212">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="2acdf-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="2acdf-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="2acdf-213">Response</span></span>
<span data-ttu-id="2acdf-214">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2acdf-214">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2acdf-215">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2acdf-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="2acdf-216">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2acdf-216">Request</span></span>
<span data-ttu-id="2acdf-217">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2acdf-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2acdf-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="2acdf-218">Response</span></span>
<span data-ttu-id="2acdf-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2acdf-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



