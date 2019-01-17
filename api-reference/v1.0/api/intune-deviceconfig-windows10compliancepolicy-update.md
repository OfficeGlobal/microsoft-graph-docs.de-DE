---
title: windows10CompliancePolicy aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 433cfe665543a8808fa91e9b441b51d960985ebc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952357"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="7116f-103">windows10CompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7116f-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="7116f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7116f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7116f-105">Aktualisiert die Eigenschaften von Objekten des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7116f-105">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7116f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7116f-106">Prerequisites</span></span>
<span data-ttu-id="7116f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7116f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7116f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7116f-109">Permission type</span></span>|<span data-ttu-id="7116f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7116f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7116f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7116f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7116f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7116f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7116f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7116f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7116f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7116f-114">Not supported.</span></span>|
|<span data-ttu-id="7116f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7116f-115">Application</span></span>|<span data-ttu-id="7116f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7116f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7116f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7116f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="7116f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7116f-118">Request headers</span></span>
|<span data-ttu-id="7116f-119">Header</span><span class="sxs-lookup"><span data-stu-id="7116f-119">Header</span></span>|<span data-ttu-id="7116f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7116f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7116f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7116f-121">Authorization</span></span>|<span data-ttu-id="7116f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7116f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7116f-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7116f-123">Accept</span></span>|<span data-ttu-id="7116f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7116f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7116f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7116f-125">Request body</span></span>
<span data-ttu-id="7116f-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7116f-126">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="7116f-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7116f-127">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="7116f-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7116f-128">Property</span></span>|<span data-ttu-id="7116f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7116f-129">Type</span></span>|<span data-ttu-id="7116f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7116f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7116f-131">id</span><span class="sxs-lookup"><span data-stu-id="7116f-131">id</span></span>|<span data-ttu-id="7116f-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7116f-132">String</span></span>|<span data-ttu-id="7116f-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7116f-133">Key of the entity.</span></span> <span data-ttu-id="7116f-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7116f-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7116f-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7116f-135">createdDateTime</span></span>|<span data-ttu-id="7116f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7116f-136">DateTimeOffset</span></span>|<span data-ttu-id="7116f-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7116f-137">DateTime the object was created.</span></span> <span data-ttu-id="7116f-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7116f-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7116f-139">description</span><span class="sxs-lookup"><span data-stu-id="7116f-139">description</span></span>|<span data-ttu-id="7116f-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7116f-140">String</span></span>|<span data-ttu-id="7116f-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7116f-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7116f-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7116f-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7116f-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7116f-143">lastModifiedDateTime</span></span>|<span data-ttu-id="7116f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7116f-144">DateTimeOffset</span></span>|<span data-ttu-id="7116f-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7116f-145">DateTime the object was last modified.</span></span> <span data-ttu-id="7116f-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7116f-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7116f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7116f-147">displayName</span></span>|<span data-ttu-id="7116f-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7116f-148">String</span></span>|<span data-ttu-id="7116f-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7116f-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7116f-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7116f-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7116f-151">Version</span><span class="sxs-lookup"><span data-stu-id="7116f-151">version</span></span>|<span data-ttu-id="7116f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7116f-152">Int32</span></span>|<span data-ttu-id="7116f-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="7116f-153">Version of the device configuration.</span></span> <span data-ttu-id="7116f-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7116f-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7116f-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7116f-155">passwordRequired</span></span>|<span data-ttu-id="7116f-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="7116f-156">Boolean</span></span>|<span data-ttu-id="7116f-157">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="7116f-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="7116f-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7116f-158">passwordBlockSimple</span></span>|<span data-ttu-id="7116f-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="7116f-159">Boolean</span></span>|<span data-ttu-id="7116f-160">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="7116f-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="7116f-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="7116f-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="7116f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7116f-162">Boolean</span></span>|<span data-ttu-id="7116f-163">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="7116f-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="7116f-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7116f-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7116f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7116f-165">Int32</span></span>|<span data-ttu-id="7116f-166">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="7116f-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7116f-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7116f-167">passwordExpirationDays</span></span>|<span data-ttu-id="7116f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="7116f-168">Int32</span></span>|<span data-ttu-id="7116f-169">Zeitraum in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="7116f-169">The password expiration in days.</span></span>|
|<span data-ttu-id="7116f-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7116f-170">passwordMinimumLength</span></span>|<span data-ttu-id="7116f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="7116f-171">Int32</span></span>|<span data-ttu-id="7116f-172">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="7116f-172">The minimum password length.</span></span>|
|<span data-ttu-id="7116f-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7116f-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="7116f-174">Int32</span><span class="sxs-lookup"><span data-stu-id="7116f-174">Int32</span></span>|<span data-ttu-id="7116f-175">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="7116f-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="7116f-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7116f-176">passwordRequiredType</span></span>|[<span data-ttu-id="7116f-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7116f-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="7116f-178">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="7116f-178">The required password type.</span></span> <span data-ttu-id="7116f-179">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="7116f-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7116f-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7116f-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7116f-181">Int32</span><span class="sxs-lookup"><span data-stu-id="7116f-181">Int32</span></span>|<span data-ttu-id="7116f-182">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="7116f-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="7116f-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="7116f-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="7116f-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="7116f-184">Boolean</span></span>|<span data-ttu-id="7116f-185">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="7116f-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="7116f-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7116f-186">osMinimumVersion</span></span>|<span data-ttu-id="7116f-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7116f-187">String</span></span>|<span data-ttu-id="7116f-188">Mindestversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="7116f-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="7116f-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7116f-189">osMaximumVersion</span></span>|<span data-ttu-id="7116f-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7116f-190">String</span></span>|<span data-ttu-id="7116f-191">Maximalversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="7116f-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="7116f-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7116f-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="7116f-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7116f-193">String</span></span>|<span data-ttu-id="7116f-194">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="7116f-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="7116f-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7116f-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="7116f-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7116f-196">String</span></span>|<span data-ttu-id="7116f-197">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="7116f-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="7116f-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="7116f-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="7116f-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7116f-199">Boolean</span></span>|<span data-ttu-id="7116f-200">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="7116f-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="7116f-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="7116f-201">bitLockerEnabled</span></span>|<span data-ttu-id="7116f-202">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7116f-202">Boolean</span></span>|<span data-ttu-id="7116f-203">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="7116f-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="7116f-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="7116f-204">secureBootEnabled</span></span>|<span data-ttu-id="7116f-205">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7116f-205">Boolean</span></span>|<span data-ttu-id="7116f-206">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="7116f-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="7116f-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="7116f-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="7116f-208">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7116f-208">Boolean</span></span>|<span data-ttu-id="7116f-209">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="7116f-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="7116f-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7116f-210">storageRequireEncryption</span></span>|<span data-ttu-id="7116f-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7116f-211">Boolean</span></span>|<span data-ttu-id="7116f-212">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="7116f-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="7116f-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="7116f-213">Response</span></span>
<span data-ttu-id="7116f-214">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7116f-214">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7116f-215">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7116f-215">Example</span></span>
### <a name="request"></a><span data-ttu-id="7116f-216">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7116f-216">Request</span></span>
<span data-ttu-id="7116f-217">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7116f-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7116f-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="7116f-218">Response</span></span>
<span data-ttu-id="7116f-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7116f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



