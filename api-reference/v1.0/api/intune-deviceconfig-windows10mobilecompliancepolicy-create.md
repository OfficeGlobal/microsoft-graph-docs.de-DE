---
title: Erstellen von „windows10MobileCompliancePolicy“
description: Diese Methode erstellt ein neues Objekt des Typs windows10MobileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a75a15155f55102c58bc2888b867ff9ae82a75d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875054"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="ad463-103">Erstellen von „windows10MobileCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="ad463-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="ad463-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ad463-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad463-105">Diese Methode erstellt ein neues Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ad463-105">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad463-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ad463-106">Prerequisites</span></span>
<span data-ttu-id="ad463-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad463-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad463-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ad463-109">Permission type</span></span>|<span data-ttu-id="ad463-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ad463-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad463-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ad463-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ad463-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad463-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ad463-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ad463-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad463-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ad463-114">Not supported.</span></span>|
|<span data-ttu-id="ad463-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ad463-115">Application</span></span>|<span data-ttu-id="ad463-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ad463-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad463-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad463-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ad463-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ad463-118">Request headers</span></span>
|<span data-ttu-id="ad463-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ad463-119">Header</span></span>|<span data-ttu-id="ad463-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ad463-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad463-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad463-121">Authorization</span></span>|<span data-ttu-id="ad463-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ad463-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad463-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ad463-123">Accept</span></span>|<span data-ttu-id="ad463-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ad463-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad463-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ad463-125">Request body</span></span>
<span data-ttu-id="ad463-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10MobileCompliancePolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="ad463-126">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="ad463-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10MobileCompliancePolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ad463-127">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="ad463-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ad463-128">Property</span></span>|<span data-ttu-id="ad463-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ad463-129">Type</span></span>|<span data-ttu-id="ad463-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad463-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad463-131">id</span><span class="sxs-lookup"><span data-stu-id="ad463-131">id</span></span>|<span data-ttu-id="ad463-132">String</span><span class="sxs-lookup"><span data-stu-id="ad463-132">String</span></span>|<span data-ttu-id="ad463-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ad463-133">Key of the entity.</span></span> <span data-ttu-id="ad463-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ad463-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ad463-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad463-135">createdDateTime</span></span>|<span data-ttu-id="ad463-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad463-136">DateTimeOffset</span></span>|<span data-ttu-id="ad463-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ad463-137">DateTime the object was created.</span></span> <span data-ttu-id="ad463-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ad463-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ad463-139">description</span><span class="sxs-lookup"><span data-stu-id="ad463-139">description</span></span>|<span data-ttu-id="ad463-140">String</span><span class="sxs-lookup"><span data-stu-id="ad463-140">String</span></span>|<span data-ttu-id="ad463-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ad463-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ad463-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ad463-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ad463-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad463-143">lastModifiedDateTime</span></span>|<span data-ttu-id="ad463-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad463-144">DateTimeOffset</span></span>|<span data-ttu-id="ad463-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ad463-145">DateTime the object was last modified.</span></span> <span data-ttu-id="ad463-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ad463-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ad463-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ad463-147">displayName</span></span>|<span data-ttu-id="ad463-148">String</span><span class="sxs-lookup"><span data-stu-id="ad463-148">String</span></span>|<span data-ttu-id="ad463-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ad463-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ad463-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ad463-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ad463-151">Version</span><span class="sxs-lookup"><span data-stu-id="ad463-151">version</span></span>|<span data-ttu-id="ad463-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ad463-152">Int32</span></span>|<span data-ttu-id="ad463-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ad463-153">Version of the device configuration.</span></span> <span data-ttu-id="ad463-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ad463-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ad463-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="ad463-155">passwordRequired</span></span>|<span data-ttu-id="ad463-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad463-156">Boolean</span></span>|<span data-ttu-id="ad463-157">Legt fest, dass zum Entsperren des Windows Phone-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ad463-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="ad463-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ad463-158">passwordBlockSimple</span></span>|<span data-ttu-id="ad463-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad463-159">Boolean</span></span>|<span data-ttu-id="ad463-160">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="ad463-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="ad463-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ad463-161">passwordMinimumLength</span></span>|<span data-ttu-id="ad463-162">Int32</span><span class="sxs-lookup"><span data-stu-id="ad463-162">Int32</span></span>|<span data-ttu-id="ad463-163">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="ad463-163">Minimum password length.</span></span> <span data-ttu-id="ad463-164">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="ad463-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="ad463-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ad463-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="ad463-166">Int32</span><span class="sxs-lookup"><span data-stu-id="ad463-166">Int32</span></span>|<span data-ttu-id="ad463-167">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="ad463-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ad463-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ad463-168">passwordRequiredType</span></span>|[<span data-ttu-id="ad463-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ad463-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ad463-170">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="ad463-170">The required password type.</span></span> <span data-ttu-id="ad463-171">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ad463-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ad463-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ad463-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ad463-173">Int32</span><span class="sxs-lookup"><span data-stu-id="ad463-173">Int32</span></span>|<span data-ttu-id="ad463-174">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="ad463-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="ad463-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ad463-175">passwordExpirationDays</span></span>|<span data-ttu-id="ad463-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ad463-176">Int32</span></span>|<span data-ttu-id="ad463-177">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="ad463-177">Number of days before password expiration.</span></span> <span data-ttu-id="ad463-178">Gültige Werte: 1 bis 255.</span><span class="sxs-lookup"><span data-stu-id="ad463-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="ad463-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ad463-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ad463-180">Int32</span><span class="sxs-lookup"><span data-stu-id="ad463-180">Int32</span></span>|<span data-ttu-id="ad463-181">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="ad463-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="ad463-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="ad463-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="ad463-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad463-183">Boolean</span></span>|<span data-ttu-id="ad463-184">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ad463-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="ad463-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ad463-185">osMinimumVersion</span></span>|<span data-ttu-id="ad463-186">String</span><span class="sxs-lookup"><span data-stu-id="ad463-186">String</span></span>|<span data-ttu-id="ad463-187">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="ad463-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="ad463-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ad463-188">osMaximumVersion</span></span>|<span data-ttu-id="ad463-189">String</span><span class="sxs-lookup"><span data-stu-id="ad463-189">String</span></span>|<span data-ttu-id="ad463-190">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="ad463-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="ad463-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="ad463-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="ad463-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad463-192">Boolean</span></span>|<span data-ttu-id="ad463-193">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="ad463-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="ad463-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="ad463-194">bitLockerEnabled</span></span>|<span data-ttu-id="ad463-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad463-195">Boolean</span></span>|<span data-ttu-id="ad463-196">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="ad463-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="ad463-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="ad463-197">secureBootEnabled</span></span>|<span data-ttu-id="ad463-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad463-198">Boolean</span></span>|<span data-ttu-id="ad463-199">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="ad463-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="ad463-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="ad463-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="ad463-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad463-201">Boolean</span></span>|<span data-ttu-id="ad463-202">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="ad463-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="ad463-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="ad463-203">storageRequireEncryption</span></span>|<span data-ttu-id="ad463-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad463-204">Boolean</span></span>|<span data-ttu-id="ad463-205">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="ad463-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="ad463-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad463-206">Response</span></span>
<span data-ttu-id="ad463-207">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ad463-207">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad463-208">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ad463-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad463-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ad463-209">Request</span></span>
<span data-ttu-id="ad463-210">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ad463-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ad463-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="ad463-211">Response</span></span>
<span data-ttu-id="ad463-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ad463-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



