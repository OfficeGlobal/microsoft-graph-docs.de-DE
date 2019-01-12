---
title: windows10CompliancePolicy aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fb689181fdc22e34bb5b85ee42c1f38e4a26905a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970143"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="520b6-103">windows10CompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="520b6-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="520b6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="520b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="520b6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="520b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="520b6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="520b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="520b6-107">Aktualisiert die Eigenschaften von Objekten des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520b6-107">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="520b6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="520b6-108">Prerequisites</span></span>
<span data-ttu-id="520b6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="520b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="520b6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="520b6-111">Permission type</span></span>|<span data-ttu-id="520b6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="520b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="520b6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="520b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="520b6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="520b6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="520b6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="520b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="520b6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="520b6-116">Not supported.</span></span>|
|<span data-ttu-id="520b6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="520b6-117">Application</span></span>|<span data-ttu-id="520b6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="520b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="520b6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="520b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="520b6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="520b6-120">Request headers</span></span>
|<span data-ttu-id="520b6-121">Header</span><span class="sxs-lookup"><span data-stu-id="520b6-121">Header</span></span>|<span data-ttu-id="520b6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="520b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="520b6-123">Authorization</span></span>|<span data-ttu-id="520b6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="520b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="520b6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="520b6-125">Accept</span></span>|<span data-ttu-id="520b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="520b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="520b6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="520b6-127">Request body</span></span>
<span data-ttu-id="520b6-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="520b6-128">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="520b6-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="520b6-129">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="520b6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="520b6-130">Property</span></span>|<span data-ttu-id="520b6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="520b6-131">Type</span></span>|<span data-ttu-id="520b6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="520b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="520b6-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="520b6-133">roleScopeTagIds</span></span>|<span data-ttu-id="520b6-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="520b6-134">String collection</span></span>|<span data-ttu-id="520b6-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="520b6-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="520b6-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520b6-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="520b6-137">id</span><span class="sxs-lookup"><span data-stu-id="520b6-137">id</span></span>|<span data-ttu-id="520b6-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="520b6-138">String</span></span>|<span data-ttu-id="520b6-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="520b6-139">Key of the entity.</span></span> <span data-ttu-id="520b6-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520b6-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="520b6-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="520b6-141">createdDateTime</span></span>|<span data-ttu-id="520b6-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="520b6-142">DateTimeOffset</span></span>|<span data-ttu-id="520b6-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="520b6-143">DateTime the object was created.</span></span> <span data-ttu-id="520b6-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520b6-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="520b6-145">description</span><span class="sxs-lookup"><span data-stu-id="520b6-145">description</span></span>|<span data-ttu-id="520b6-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="520b6-146">String</span></span>|<span data-ttu-id="520b6-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="520b6-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="520b6-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520b6-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="520b6-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="520b6-149">lastModifiedDateTime</span></span>|<span data-ttu-id="520b6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="520b6-150">DateTimeOffset</span></span>|<span data-ttu-id="520b6-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="520b6-151">DateTime the object was last modified.</span></span> <span data-ttu-id="520b6-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520b6-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="520b6-153">displayName</span><span class="sxs-lookup"><span data-stu-id="520b6-153">displayName</span></span>|<span data-ttu-id="520b6-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="520b6-154">String</span></span>|<span data-ttu-id="520b6-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="520b6-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="520b6-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520b6-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="520b6-157">Version</span><span class="sxs-lookup"><span data-stu-id="520b6-157">version</span></span>|<span data-ttu-id="520b6-158">Int32</span><span class="sxs-lookup"><span data-stu-id="520b6-158">Int32</span></span>|<span data-ttu-id="520b6-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="520b6-159">Version of the device configuration.</span></span> <span data-ttu-id="520b6-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="520b6-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="520b6-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="520b6-161">passwordRequired</span></span>|<span data-ttu-id="520b6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="520b6-162">Boolean</span></span>|<span data-ttu-id="520b6-163">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="520b6-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="520b6-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="520b6-164">passwordBlockSimple</span></span>|<span data-ttu-id="520b6-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="520b6-165">Boolean</span></span>|<span data-ttu-id="520b6-166">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="520b6-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="520b6-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="520b6-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="520b6-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="520b6-168">Boolean</span></span>|<span data-ttu-id="520b6-169">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="520b6-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="520b6-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="520b6-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="520b6-171">Int32</span><span class="sxs-lookup"><span data-stu-id="520b6-171">Int32</span></span>|<span data-ttu-id="520b6-172">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="520b6-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="520b6-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="520b6-173">passwordExpirationDays</span></span>|<span data-ttu-id="520b6-174">Int32</span><span class="sxs-lookup"><span data-stu-id="520b6-174">Int32</span></span>|<span data-ttu-id="520b6-175">Zeitraum in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="520b6-175">The password expiration in days.</span></span>|
|<span data-ttu-id="520b6-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="520b6-176">passwordMinimumLength</span></span>|<span data-ttu-id="520b6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="520b6-177">Int32</span></span>|<span data-ttu-id="520b6-178">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="520b6-178">The minimum password length.</span></span>|
|<span data-ttu-id="520b6-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="520b6-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="520b6-180">Int32</span><span class="sxs-lookup"><span data-stu-id="520b6-180">Int32</span></span>|<span data-ttu-id="520b6-181">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="520b6-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="520b6-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="520b6-182">passwordRequiredType</span></span>|[<span data-ttu-id="520b6-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="520b6-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="520b6-184">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="520b6-184">The required password type.</span></span> <span data-ttu-id="520b6-185">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="520b6-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="520b6-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="520b6-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="520b6-187">Int32</span><span class="sxs-lookup"><span data-stu-id="520b6-187">Int32</span></span>|<span data-ttu-id="520b6-188">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="520b6-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="520b6-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="520b6-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="520b6-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="520b6-190">Boolean</span></span>|<span data-ttu-id="520b6-191">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="520b6-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="520b6-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="520b6-192">osMinimumVersion</span></span>|<span data-ttu-id="520b6-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="520b6-193">String</span></span>|<span data-ttu-id="520b6-194">Mindestversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="520b6-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="520b6-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="520b6-195">osMaximumVersion</span></span>|<span data-ttu-id="520b6-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="520b6-196">String</span></span>|<span data-ttu-id="520b6-197">Maximalversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="520b6-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="520b6-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="520b6-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="520b6-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="520b6-199">String</span></span>|<span data-ttu-id="520b6-200">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="520b6-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="520b6-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="520b6-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="520b6-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="520b6-202">String</span></span>|<span data-ttu-id="520b6-203">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="520b6-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="520b6-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="520b6-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="520b6-205">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-205">Boolean</span></span>|<span data-ttu-id="520b6-206">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="520b6-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="520b6-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="520b6-207">bitLockerEnabled</span></span>|<span data-ttu-id="520b6-208">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-208">Boolean</span></span>|<span data-ttu-id="520b6-209">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="520b6-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="520b6-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="520b6-210">secureBootEnabled</span></span>|<span data-ttu-id="520b6-211">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-211">Boolean</span></span>|<span data-ttu-id="520b6-212">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="520b6-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="520b6-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="520b6-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="520b6-214">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-214">Boolean</span></span>|<span data-ttu-id="520b6-215">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="520b6-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="520b6-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="520b6-216">storageRequireEncryption</span></span>|<span data-ttu-id="520b6-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-217">Boolean</span></span>|<span data-ttu-id="520b6-218">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="520b6-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="520b6-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="520b6-219">activeFirewallRequired</span></span>|<span data-ttu-id="520b6-220">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-220">Boolean</span></span>|<span data-ttu-id="520b6-221">Erfordern Sie active Firewall auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="520b6-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="520b6-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="520b6-222">defenderEnabled</span></span>|<span data-ttu-id="520b6-223">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-223">Boolean</span></span>|<span data-ttu-id="520b6-224">Benötigen Sie Windows Defender Modul auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="520b6-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="520b6-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="520b6-225">defenderVersion</span></span>|<span data-ttu-id="520b6-226">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="520b6-226">String</span></span>|<span data-ttu-id="520b6-227">Benötigen Sie mindestens Version von Windows Defender Modul auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="520b6-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="520b6-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="520b6-228">signatureOutOfDate</span></span>|<span data-ttu-id="520b6-229">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-229">Boolean</span></span>|<span data-ttu-id="520b6-230">Benötigen Sie Windows Defender Modul Signatur, um auf Windows-Geräten Stand sein.</span><span class="sxs-lookup"><span data-stu-id="520b6-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="520b6-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="520b6-231">rtpEnabled</span></span>|<span data-ttu-id="520b6-232">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-232">Boolean</span></span>|<span data-ttu-id="520b6-233">Benötigen Sie Windows Defender Modul Real-Time Schutz auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="520b6-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="520b6-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="520b6-234">antivirusRequired</span></span>|<span data-ttu-id="520b6-235">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-235">Boolean</span></span>|<span data-ttu-id="520b6-236">Erfordern Sie Antivirus-Lösung mit Windows Decurity Center befinden registriert und Überwachung (z. B. Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="520b6-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="520b6-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="520b6-237">antiSpywareRequired</span></span>|<span data-ttu-id="520b6-238">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-238">Boolean</span></span>|<span data-ttu-id="520b6-239">Erfordern Sie AntiSpyware-Lösung mit Windows Decurity Center befinden registriert und Überwachung (z. B. Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="520b6-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="520b6-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="520b6-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="520b6-241">[OperatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="520b6-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="520b6-242">Das gültige Betriebssystem erstellen Bereiche auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="520b6-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="520b6-243">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="520b6-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="520b6-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="520b6-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="520b6-245">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-245">Boolean</span></span>|<span data-ttu-id="520b6-246">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="520b6-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="520b6-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="520b6-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="520b6-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="520b6-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="520b6-249">Erfordern Sie Gerät Bedrohung minimalem Risiko Mail-Schutzstufe Kompatibilität vorgesehenen Unwichtigstes.</span><span class="sxs-lookup"><span data-stu-id="520b6-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="520b6-250">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="520b6-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="520b6-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="520b6-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="520b6-252">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="520b6-252">Boolean</span></span>|<span data-ttu-id="520b6-253">SCCM Compliance Zustand berücksichtigt für Intune Compliance Zustand berücksichtigen müssen.</span><span class="sxs-lookup"><span data-stu-id="520b6-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="520b6-254">Antwort</span><span class="sxs-lookup"><span data-stu-id="520b6-254">Response</span></span>
<span data-ttu-id="520b6-255">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="520b6-255">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="520b6-256">Beispiel</span><span class="sxs-lookup"><span data-stu-id="520b6-256">Example</span></span>
### <a name="request"></a><span data-ttu-id="520b6-257">Anforderung</span><span class="sxs-lookup"><span data-stu-id="520b6-257">Request</span></span>
<span data-ttu-id="520b6-258">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="520b6-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1666

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
  "configurationManagerComplianceRequired": true
}
```

### <a name="response"></a><span data-ttu-id="520b6-259">Antwort</span><span class="sxs-lookup"><span data-stu-id="520b6-259">Response</span></span>
<span data-ttu-id="520b6-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="520b6-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1838

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
  "configurationManagerComplianceRequired": true
}
```





