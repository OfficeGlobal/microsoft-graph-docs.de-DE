---
title: Erstellen von „windows10MobileCompliancePolicy“
description: Diese Methode erstellt ein neues Objekt des Typs windows10MobileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 745504fa748051bf8a65de588b30295a22725b60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937208"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="b10ac-103">Erstellen von „windows10MobileCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="b10ac-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="b10ac-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b10ac-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b10ac-105">Diese Methode erstellt ein neues Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b10ac-105">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b10ac-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b10ac-106">Prerequisites</span></span>
<span data-ttu-id="b10ac-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b10ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b10ac-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b10ac-109">Permission type</span></span>|<span data-ttu-id="b10ac-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b10ac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b10ac-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b10ac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b10ac-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b10ac-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b10ac-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b10ac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b10ac-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b10ac-114">Not supported.</span></span>|
|<span data-ttu-id="b10ac-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b10ac-115">Application</span></span>|<span data-ttu-id="b10ac-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b10ac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b10ac-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b10ac-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="b10ac-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b10ac-118">Request headers</span></span>
|<span data-ttu-id="b10ac-119">Header</span><span class="sxs-lookup"><span data-stu-id="b10ac-119">Header</span></span>|<span data-ttu-id="b10ac-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b10ac-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b10ac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b10ac-121">Authorization</span></span>|<span data-ttu-id="b10ac-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b10ac-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b10ac-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b10ac-123">Accept</span></span>|<span data-ttu-id="b10ac-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b10ac-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b10ac-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b10ac-125">Request body</span></span>
<span data-ttu-id="b10ac-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10MobileCompliancePolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="b10ac-126">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="b10ac-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10MobileCompliancePolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="b10ac-127">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="b10ac-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b10ac-128">Property</span></span>|<span data-ttu-id="b10ac-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b10ac-129">Type</span></span>|<span data-ttu-id="b10ac-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b10ac-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b10ac-131">id</span><span class="sxs-lookup"><span data-stu-id="b10ac-131">id</span></span>|<span data-ttu-id="b10ac-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b10ac-132">String</span></span>|<span data-ttu-id="b10ac-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b10ac-133">Key of the entity.</span></span> <span data-ttu-id="b10ac-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b10ac-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b10ac-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b10ac-135">createdDateTime</span></span>|<span data-ttu-id="b10ac-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b10ac-136">DateTimeOffset</span></span>|<span data-ttu-id="b10ac-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b10ac-137">DateTime the object was created.</span></span> <span data-ttu-id="b10ac-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b10ac-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b10ac-139">description</span><span class="sxs-lookup"><span data-stu-id="b10ac-139">description</span></span>|<span data-ttu-id="b10ac-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b10ac-140">String</span></span>|<span data-ttu-id="b10ac-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b10ac-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b10ac-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b10ac-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b10ac-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b10ac-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b10ac-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b10ac-144">DateTimeOffset</span></span>|<span data-ttu-id="b10ac-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b10ac-145">DateTime the object was last modified.</span></span> <span data-ttu-id="b10ac-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b10ac-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b10ac-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b10ac-147">displayName</span></span>|<span data-ttu-id="b10ac-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b10ac-148">String</span></span>|<span data-ttu-id="b10ac-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b10ac-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b10ac-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b10ac-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b10ac-151">Version</span><span class="sxs-lookup"><span data-stu-id="b10ac-151">version</span></span>|<span data-ttu-id="b10ac-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b10ac-152">Int32</span></span>|<span data-ttu-id="b10ac-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b10ac-153">Version of the device configuration.</span></span> <span data-ttu-id="b10ac-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b10ac-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b10ac-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b10ac-155">passwordRequired</span></span>|<span data-ttu-id="b10ac-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b10ac-156">Boolean</span></span>|<span data-ttu-id="b10ac-157">Legt fest, dass zum Entsperren des Windows Phone-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b10ac-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="b10ac-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b10ac-158">passwordBlockSimple</span></span>|<span data-ttu-id="b10ac-159">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b10ac-159">Boolean</span></span>|<span data-ttu-id="b10ac-160">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b10ac-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="b10ac-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b10ac-161">passwordMinimumLength</span></span>|<span data-ttu-id="b10ac-162">Int32</span><span class="sxs-lookup"><span data-stu-id="b10ac-162">Int32</span></span>|<span data-ttu-id="b10ac-163">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="b10ac-163">Minimum password length.</span></span> <span data-ttu-id="b10ac-164">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="b10ac-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b10ac-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b10ac-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b10ac-166">Int32</span><span class="sxs-lookup"><span data-stu-id="b10ac-166">Int32</span></span>|<span data-ttu-id="b10ac-167">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="b10ac-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b10ac-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b10ac-168">passwordRequiredType</span></span>|[<span data-ttu-id="b10ac-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b10ac-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b10ac-170">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="b10ac-170">The required password type.</span></span> <span data-ttu-id="b10ac-171">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b10ac-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b10ac-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b10ac-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b10ac-173">Int32</span><span class="sxs-lookup"><span data-stu-id="b10ac-173">Int32</span></span>|<span data-ttu-id="b10ac-174">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="b10ac-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="b10ac-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b10ac-175">passwordExpirationDays</span></span>|<span data-ttu-id="b10ac-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b10ac-176">Int32</span></span>|<span data-ttu-id="b10ac-177">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="b10ac-177">Number of days before password expiration.</span></span> <span data-ttu-id="b10ac-178">Gültige Werte: 1 bis 255.</span><span class="sxs-lookup"><span data-stu-id="b10ac-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="b10ac-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b10ac-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b10ac-180">Int32</span><span class="sxs-lookup"><span data-stu-id="b10ac-180">Int32</span></span>|<span data-ttu-id="b10ac-181">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="b10ac-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b10ac-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="b10ac-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="b10ac-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b10ac-183">Boolean</span></span>|<span data-ttu-id="b10ac-184">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b10ac-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="b10ac-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b10ac-185">osMinimumVersion</span></span>|<span data-ttu-id="b10ac-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b10ac-186">String</span></span>|<span data-ttu-id="b10ac-187">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="b10ac-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="b10ac-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b10ac-188">osMaximumVersion</span></span>|<span data-ttu-id="b10ac-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b10ac-189">String</span></span>|<span data-ttu-id="b10ac-190">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="b10ac-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="b10ac-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="b10ac-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="b10ac-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b10ac-192">Boolean</span></span>|<span data-ttu-id="b10ac-193">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="b10ac-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="b10ac-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="b10ac-194">bitLockerEnabled</span></span>|<span data-ttu-id="b10ac-195">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b10ac-195">Boolean</span></span>|<span data-ttu-id="b10ac-196">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="b10ac-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="b10ac-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="b10ac-197">secureBootEnabled</span></span>|<span data-ttu-id="b10ac-198">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b10ac-198">Boolean</span></span>|<span data-ttu-id="b10ac-199">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="b10ac-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="b10ac-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="b10ac-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="b10ac-201">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b10ac-201">Boolean</span></span>|<span data-ttu-id="b10ac-202">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="b10ac-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="b10ac-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b10ac-203">storageRequireEncryption</span></span>|<span data-ttu-id="b10ac-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b10ac-204">Boolean</span></span>|<span data-ttu-id="b10ac-205">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="b10ac-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="b10ac-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="b10ac-206">Response</span></span>
<span data-ttu-id="b10ac-207">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b10ac-207">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b10ac-208">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b10ac-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="b10ac-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b10ac-209">Request</span></span>
<span data-ttu-id="b10ac-210">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b10ac-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b10ac-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="b10ac-211">Response</span></span>
<span data-ttu-id="b10ac-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b10ac-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



