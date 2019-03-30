---
title: Erstellen von „windows10MobileCompliancePolicy“
description: Erstellen eines neuen windows10MobileCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0ca0d60f4385c8fdc6d3b98183c348685469698
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989456"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="e81a8-103">Erstellen von „windows10MobileCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="e81a8-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="e81a8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e81a8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e81a8-105">Diese Methode erstellt ein neues Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e81a8-105">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e81a8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e81a8-106">Prerequisites</span></span>
<span data-ttu-id="e81a8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e81a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e81a8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e81a8-109">Permission type</span></span>|<span data-ttu-id="e81a8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e81a8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e81a8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e81a8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e81a8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e81a8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e81a8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e81a8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e81a8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e81a8-114">Not supported.</span></span>|
|<span data-ttu-id="e81a8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e81a8-115">Application</span></span>|<span data-ttu-id="e81a8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e81a8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e81a8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e81a8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e81a8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e81a8-118">Request headers</span></span>
|<span data-ttu-id="e81a8-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e81a8-119">Header</span></span>|<span data-ttu-id="e81a8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e81a8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e81a8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e81a8-121">Authorization</span></span>|<span data-ttu-id="e81a8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e81a8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e81a8-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e81a8-123">Accept</span></span>|<span data-ttu-id="e81a8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e81a8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e81a8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e81a8-125">Request body</span></span>
<span data-ttu-id="e81a8-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10MobileCompliancePolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="e81a8-126">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="e81a8-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10MobileCompliancePolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="e81a8-127">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="e81a8-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e81a8-128">Property</span></span>|<span data-ttu-id="e81a8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e81a8-129">Type</span></span>|<span data-ttu-id="e81a8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e81a8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e81a8-131">id</span><span class="sxs-lookup"><span data-stu-id="e81a8-131">id</span></span>|<span data-ttu-id="e81a8-132">String</span><span class="sxs-lookup"><span data-stu-id="e81a8-132">String</span></span>|<span data-ttu-id="e81a8-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e81a8-133">Key of the entity.</span></span> <span data-ttu-id="e81a8-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e81a8-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e81a8-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e81a8-135">createdDateTime</span></span>|<span data-ttu-id="e81a8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e81a8-136">DateTimeOffset</span></span>|<span data-ttu-id="e81a8-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e81a8-137">DateTime the object was created.</span></span> <span data-ttu-id="e81a8-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e81a8-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e81a8-139">description</span><span class="sxs-lookup"><span data-stu-id="e81a8-139">description</span></span>|<span data-ttu-id="e81a8-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e81a8-140">String</span></span>|<span data-ttu-id="e81a8-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e81a8-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e81a8-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e81a8-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e81a8-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e81a8-143">lastModifiedDateTime</span></span>|<span data-ttu-id="e81a8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e81a8-144">DateTimeOffset</span></span>|<span data-ttu-id="e81a8-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e81a8-145">DateTime the object was last modified.</span></span> <span data-ttu-id="e81a8-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e81a8-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e81a8-147">displayName</span><span class="sxs-lookup"><span data-stu-id="e81a8-147">displayName</span></span>|<span data-ttu-id="e81a8-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e81a8-148">String</span></span>|<span data-ttu-id="e81a8-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e81a8-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e81a8-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e81a8-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e81a8-151">Version</span><span class="sxs-lookup"><span data-stu-id="e81a8-151">version</span></span>|<span data-ttu-id="e81a8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e81a8-152">Int32</span></span>|<span data-ttu-id="e81a8-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="e81a8-153">Version of the device configuration.</span></span> <span data-ttu-id="e81a8-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e81a8-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e81a8-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e81a8-155">passwordRequired</span></span>|<span data-ttu-id="e81a8-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="e81a8-156">Boolean</span></span>|<span data-ttu-id="e81a8-157">Legt fest, dass zum Entsperren des Windows Phone-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e81a8-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="e81a8-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e81a8-158">passwordBlockSimple</span></span>|<span data-ttu-id="e81a8-159">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e81a8-159">Boolean</span></span>|<span data-ttu-id="e81a8-160">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="e81a8-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="e81a8-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e81a8-161">passwordMinimumLength</span></span>|<span data-ttu-id="e81a8-162">Int32</span><span class="sxs-lookup"><span data-stu-id="e81a8-162">Int32</span></span>|<span data-ttu-id="e81a8-163">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="e81a8-163">Minimum password length.</span></span> <span data-ttu-id="e81a8-164">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="e81a8-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e81a8-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e81a8-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e81a8-166">Int32</span><span class="sxs-lookup"><span data-stu-id="e81a8-166">Int32</span></span>|<span data-ttu-id="e81a8-167">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.</span><span class="sxs-lookup"><span data-stu-id="e81a8-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e81a8-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e81a8-168">passwordRequiredType</span></span>|[<span data-ttu-id="e81a8-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e81a8-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e81a8-170">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="e81a8-170">The required password type.</span></span> <span data-ttu-id="e81a8-171">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e81a8-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e81a8-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e81a8-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e81a8-173">Int32</span><span class="sxs-lookup"><span data-stu-id="e81a8-173">Int32</span></span>|<span data-ttu-id="e81a8-174">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="e81a8-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="e81a8-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e81a8-175">passwordExpirationDays</span></span>|<span data-ttu-id="e81a8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e81a8-176">Int32</span></span>|<span data-ttu-id="e81a8-177">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="e81a8-177">Number of days before password expiration.</span></span> <span data-ttu-id="e81a8-178">Gültige Werte: 1 bis 255.</span><span class="sxs-lookup"><span data-stu-id="e81a8-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="e81a8-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e81a8-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e81a8-180">Int32</span><span class="sxs-lookup"><span data-stu-id="e81a8-180">Int32</span></span>|<span data-ttu-id="e81a8-181">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="e81a8-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e81a8-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="e81a8-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="e81a8-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="e81a8-183">Boolean</span></span>|<span data-ttu-id="e81a8-184">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e81a8-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="e81a8-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e81a8-185">osMinimumVersion</span></span>|<span data-ttu-id="e81a8-186">String</span><span class="sxs-lookup"><span data-stu-id="e81a8-186">String</span></span>|<span data-ttu-id="e81a8-187">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="e81a8-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="e81a8-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e81a8-188">osMaximumVersion</span></span>|<span data-ttu-id="e81a8-189">String</span><span class="sxs-lookup"><span data-stu-id="e81a8-189">String</span></span>|<span data-ttu-id="e81a8-190">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="e81a8-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="e81a8-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="e81a8-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="e81a8-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e81a8-192">Boolean</span></span>|<span data-ttu-id="e81a8-193">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="e81a8-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="e81a8-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="e81a8-194">bitLockerEnabled</span></span>|<span data-ttu-id="e81a8-195">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e81a8-195">Boolean</span></span>|<span data-ttu-id="e81a8-196">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="e81a8-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="e81a8-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="e81a8-197">secureBootEnabled</span></span>|<span data-ttu-id="e81a8-198">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e81a8-198">Boolean</span></span>|<span data-ttu-id="e81a8-199">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="e81a8-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="e81a8-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="e81a8-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="e81a8-201">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e81a8-201">Boolean</span></span>|<span data-ttu-id="e81a8-202">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="e81a8-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="e81a8-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e81a8-203">storageRequireEncryption</span></span>|<span data-ttu-id="e81a8-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e81a8-204">Boolean</span></span>|<span data-ttu-id="e81a8-205">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="e81a8-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="e81a8-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="e81a8-206">Response</span></span>
<span data-ttu-id="e81a8-207">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e81a8-207">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e81a8-208">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e81a8-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="e81a8-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e81a8-209">Request</span></span>
<span data-ttu-id="e81a8-210">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e81a8-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 792

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
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
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="e81a8-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="e81a8-211">Response</span></span>
<span data-ttu-id="e81a8-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e81a8-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
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
  "storageRequireEncryption": true
}
```



