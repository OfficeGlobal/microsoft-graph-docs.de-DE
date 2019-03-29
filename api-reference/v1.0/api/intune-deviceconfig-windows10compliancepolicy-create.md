---
title: windows10CompliancePolicy erstellen
description: Erstellt neue Objekte des Typs windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c03c8a3b8ce4ac43da35eba89b18bc57c5db867a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982504"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="067e1-103">windows10CompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="067e1-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="067e1-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="067e1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="067e1-105">Erstellt neue Objekte des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="067e1-105">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="067e1-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="067e1-106">Prerequisites</span></span>
<span data-ttu-id="067e1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="067e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="067e1-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="067e1-109">Permission type</span></span>|<span data-ttu-id="067e1-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="067e1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="067e1-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="067e1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="067e1-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="067e1-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="067e1-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="067e1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="067e1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="067e1-114">Not supported.</span></span>|
|<span data-ttu-id="067e1-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="067e1-115">Application</span></span>|<span data-ttu-id="067e1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="067e1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="067e1-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="067e1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="067e1-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="067e1-118">Request headers</span></span>
|<span data-ttu-id="067e1-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="067e1-119">Header</span></span>|<span data-ttu-id="067e1-120">Wert</span><span class="sxs-lookup"><span data-stu-id="067e1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="067e1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="067e1-121">Authorization</span></span>|<span data-ttu-id="067e1-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="067e1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="067e1-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="067e1-123">Accept</span></span>|<span data-ttu-id="067e1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="067e1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="067e1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="067e1-125">Request body</span></span>
<span data-ttu-id="067e1-126">Geben Sie im Anforderungstext eine JSON-Darstellung des windows10CompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="067e1-126">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="067e1-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10CompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="067e1-127">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="067e1-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="067e1-128">Property</span></span>|<span data-ttu-id="067e1-129">Typ</span><span class="sxs-lookup"><span data-stu-id="067e1-129">Type</span></span>|<span data-ttu-id="067e1-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="067e1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="067e1-131">id</span><span class="sxs-lookup"><span data-stu-id="067e1-131">id</span></span>|<span data-ttu-id="067e1-132">String</span><span class="sxs-lookup"><span data-stu-id="067e1-132">String</span></span>|<span data-ttu-id="067e1-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="067e1-133">Key of the entity.</span></span> <span data-ttu-id="067e1-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="067e1-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="067e1-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="067e1-135">createdDateTime</span></span>|<span data-ttu-id="067e1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="067e1-136">DateTimeOffset</span></span>|<span data-ttu-id="067e1-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="067e1-137">DateTime the object was created.</span></span> <span data-ttu-id="067e1-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="067e1-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="067e1-139">description</span><span class="sxs-lookup"><span data-stu-id="067e1-139">description</span></span>|<span data-ttu-id="067e1-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="067e1-140">String</span></span>|<span data-ttu-id="067e1-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="067e1-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="067e1-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="067e1-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="067e1-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="067e1-143">lastModifiedDateTime</span></span>|<span data-ttu-id="067e1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="067e1-144">DateTimeOffset</span></span>|<span data-ttu-id="067e1-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="067e1-145">DateTime the object was last modified.</span></span> <span data-ttu-id="067e1-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="067e1-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="067e1-147">displayName</span><span class="sxs-lookup"><span data-stu-id="067e1-147">displayName</span></span>|<span data-ttu-id="067e1-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="067e1-148">String</span></span>|<span data-ttu-id="067e1-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="067e1-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="067e1-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="067e1-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="067e1-151">Version</span><span class="sxs-lookup"><span data-stu-id="067e1-151">version</span></span>|<span data-ttu-id="067e1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="067e1-152">Int32</span></span>|<span data-ttu-id="067e1-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="067e1-153">Version of the device configuration.</span></span> <span data-ttu-id="067e1-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="067e1-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="067e1-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="067e1-155">passwordRequired</span></span>|<span data-ttu-id="067e1-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="067e1-156">Boolean</span></span>|<span data-ttu-id="067e1-157">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="067e1-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="067e1-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="067e1-158">passwordBlockSimple</span></span>|<span data-ttu-id="067e1-159">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="067e1-159">Boolean</span></span>|<span data-ttu-id="067e1-160">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="067e1-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="067e1-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="067e1-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="067e1-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="067e1-162">Boolean</span></span>|<span data-ttu-id="067e1-163">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="067e1-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="067e1-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="067e1-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="067e1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="067e1-165">Int32</span></span>|<span data-ttu-id="067e1-166">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="067e1-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="067e1-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="067e1-167">passwordExpirationDays</span></span>|<span data-ttu-id="067e1-168">Int32</span><span class="sxs-lookup"><span data-stu-id="067e1-168">Int32</span></span>|<span data-ttu-id="067e1-169">Zeitraum in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="067e1-169">The password expiration in days.</span></span>|
|<span data-ttu-id="067e1-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="067e1-170">passwordMinimumLength</span></span>|<span data-ttu-id="067e1-171">Int32</span><span class="sxs-lookup"><span data-stu-id="067e1-171">Int32</span></span>|<span data-ttu-id="067e1-172">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="067e1-172">The minimum password length.</span></span>|
|<span data-ttu-id="067e1-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="067e1-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="067e1-174">Int32</span><span class="sxs-lookup"><span data-stu-id="067e1-174">Int32</span></span>|<span data-ttu-id="067e1-175">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.</span><span class="sxs-lookup"><span data-stu-id="067e1-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="067e1-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="067e1-176">passwordRequiredType</span></span>|[<span data-ttu-id="067e1-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="067e1-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="067e1-178">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="067e1-178">The required password type.</span></span> <span data-ttu-id="067e1-179">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="067e1-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="067e1-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="067e1-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="067e1-181">Int32</span><span class="sxs-lookup"><span data-stu-id="067e1-181">Int32</span></span>|<span data-ttu-id="067e1-182">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="067e1-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="067e1-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="067e1-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="067e1-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="067e1-184">Boolean</span></span>|<span data-ttu-id="067e1-185">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="067e1-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="067e1-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="067e1-186">osMinimumVersion</span></span>|<span data-ttu-id="067e1-187">String</span><span class="sxs-lookup"><span data-stu-id="067e1-187">String</span></span>|<span data-ttu-id="067e1-188">Mindestversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="067e1-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="067e1-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="067e1-189">osMaximumVersion</span></span>|<span data-ttu-id="067e1-190">String</span><span class="sxs-lookup"><span data-stu-id="067e1-190">String</span></span>|<span data-ttu-id="067e1-191">Maximalversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="067e1-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="067e1-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="067e1-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="067e1-193">String</span><span class="sxs-lookup"><span data-stu-id="067e1-193">String</span></span>|<span data-ttu-id="067e1-194">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="067e1-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="067e1-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="067e1-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="067e1-196">String</span><span class="sxs-lookup"><span data-stu-id="067e1-196">String</span></span>|<span data-ttu-id="067e1-197">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="067e1-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="067e1-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="067e1-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="067e1-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="067e1-199">Boolean</span></span>|<span data-ttu-id="067e1-200">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="067e1-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="067e1-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="067e1-201">bitLockerEnabled</span></span>|<span data-ttu-id="067e1-202">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="067e1-202">Boolean</span></span>|<span data-ttu-id="067e1-203">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="067e1-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="067e1-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="067e1-204">secureBootEnabled</span></span>|<span data-ttu-id="067e1-205">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="067e1-205">Boolean</span></span>|<span data-ttu-id="067e1-206">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="067e1-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="067e1-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="067e1-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="067e1-208">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="067e1-208">Boolean</span></span>|<span data-ttu-id="067e1-209">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="067e1-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="067e1-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="067e1-210">storageRequireEncryption</span></span>|<span data-ttu-id="067e1-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="067e1-211">Boolean</span></span>|<span data-ttu-id="067e1-212">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="067e1-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="067e1-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="067e1-213">Response</span></span>
<span data-ttu-id="067e1-214">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="067e1-214">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="067e1-215">Beispiel</span><span class="sxs-lookup"><span data-stu-id="067e1-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="067e1-216">Anforderung</span><span class="sxs-lookup"><span data-stu-id="067e1-216">Request</span></span>
<span data-ttu-id="067e1-217">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="067e1-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="067e1-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="067e1-218">Response</span></span>
<span data-ttu-id="067e1-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="067e1-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



