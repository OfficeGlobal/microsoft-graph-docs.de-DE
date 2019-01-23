---
title: windows10CompliancePolicy erstellen
description: Erstellt neue Objekte des Typs windows10CompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2eba67635ea4e596dd9bf1881b5b5c0d7b9743df
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422740"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="8aac5-103">windows10CompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="8aac5-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="8aac5-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8aac5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8aac5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8aac5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8aac5-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8aac5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8aac5-107">Erstellt neue Objekte des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8aac5-107">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8aac5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8aac5-108">Prerequisites</span></span>
<span data-ttu-id="8aac5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8aac5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8aac5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8aac5-111">Permission type</span></span>|<span data-ttu-id="8aac5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8aac5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8aac5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8aac5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8aac5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aac5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8aac5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8aac5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8aac5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8aac5-116">Not supported.</span></span>|
|<span data-ttu-id="8aac5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8aac5-117">Application</span></span>|<span data-ttu-id="8aac5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8aac5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8aac5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8aac5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="8aac5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8aac5-120">Request headers</span></span>
|<span data-ttu-id="8aac5-121">Header</span><span class="sxs-lookup"><span data-stu-id="8aac5-121">Header</span></span>|<span data-ttu-id="8aac5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8aac5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8aac5-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8aac5-123">Authorization</span></span>|<span data-ttu-id="8aac5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8aac5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8aac5-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8aac5-125">Accept</span></span>|<span data-ttu-id="8aac5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8aac5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8aac5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8aac5-127">Request body</span></span>
<span data-ttu-id="8aac5-128">Geben Sie im Anforderungstext eine JSON-Darstellung des windows10CompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8aac5-128">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="8aac5-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10CompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8aac5-129">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="8aac5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8aac5-130">Property</span></span>|<span data-ttu-id="8aac5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8aac5-131">Type</span></span>|<span data-ttu-id="8aac5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8aac5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8aac5-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8aac5-133">roleScopeTagIds</span></span>|<span data-ttu-id="8aac5-134">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="8aac5-134">String collection</span></span>|<span data-ttu-id="8aac5-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="8aac5-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8aac5-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8aac5-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8aac5-137">id</span><span class="sxs-lookup"><span data-stu-id="8aac5-137">id</span></span>|<span data-ttu-id="8aac5-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8aac5-138">String</span></span>|<span data-ttu-id="8aac5-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8aac5-139">Key of the entity.</span></span> <span data-ttu-id="8aac5-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8aac5-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8aac5-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8aac5-141">createdDateTime</span></span>|<span data-ttu-id="8aac5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8aac5-142">DateTimeOffset</span></span>|<span data-ttu-id="8aac5-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8aac5-143">DateTime the object was created.</span></span> <span data-ttu-id="8aac5-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8aac5-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8aac5-145">description</span><span class="sxs-lookup"><span data-stu-id="8aac5-145">description</span></span>|<span data-ttu-id="8aac5-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8aac5-146">String</span></span>|<span data-ttu-id="8aac5-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8aac5-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8aac5-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8aac5-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8aac5-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8aac5-149">lastModifiedDateTime</span></span>|<span data-ttu-id="8aac5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8aac5-150">DateTimeOffset</span></span>|<span data-ttu-id="8aac5-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8aac5-151">DateTime the object was last modified.</span></span> <span data-ttu-id="8aac5-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8aac5-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8aac5-153">displayName</span><span class="sxs-lookup"><span data-stu-id="8aac5-153">displayName</span></span>|<span data-ttu-id="8aac5-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8aac5-154">String</span></span>|<span data-ttu-id="8aac5-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8aac5-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8aac5-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8aac5-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8aac5-157">Version</span><span class="sxs-lookup"><span data-stu-id="8aac5-157">version</span></span>|<span data-ttu-id="8aac5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8aac5-158">Int32</span></span>|<span data-ttu-id="8aac5-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8aac5-159">Version of the device configuration.</span></span> <span data-ttu-id="8aac5-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8aac5-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8aac5-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8aac5-161">passwordRequired</span></span>|<span data-ttu-id="8aac5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-162">Boolean</span></span>|<span data-ttu-id="8aac5-163">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="8aac5-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="8aac5-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8aac5-164">passwordBlockSimple</span></span>|<span data-ttu-id="8aac5-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-165">Boolean</span></span>|<span data-ttu-id="8aac5-166">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="8aac5-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="8aac5-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="8aac5-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="8aac5-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-168">Boolean</span></span>|<span data-ttu-id="8aac5-169">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="8aac5-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="8aac5-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8aac5-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8aac5-171">Int32</span><span class="sxs-lookup"><span data-stu-id="8aac5-171">Int32</span></span>|<span data-ttu-id="8aac5-172">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="8aac5-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="8aac5-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8aac5-173">passwordExpirationDays</span></span>|<span data-ttu-id="8aac5-174">Int32</span><span class="sxs-lookup"><span data-stu-id="8aac5-174">Int32</span></span>|<span data-ttu-id="8aac5-175">Zeitraum in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="8aac5-175">The password expiration in days.</span></span>|
|<span data-ttu-id="8aac5-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8aac5-176">passwordMinimumLength</span></span>|<span data-ttu-id="8aac5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8aac5-177">Int32</span></span>|<span data-ttu-id="8aac5-178">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="8aac5-178">The minimum password length.</span></span>|
|<span data-ttu-id="8aac5-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8aac5-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8aac5-180">Int32</span><span class="sxs-lookup"><span data-stu-id="8aac5-180">Int32</span></span>|<span data-ttu-id="8aac5-181">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="8aac5-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8aac5-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8aac5-182">passwordRequiredType</span></span>|[<span data-ttu-id="8aac5-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8aac5-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="8aac5-184">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="8aac5-184">The required password type.</span></span> <span data-ttu-id="8aac5-185">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="8aac5-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8aac5-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8aac5-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8aac5-187">Int32</span><span class="sxs-lookup"><span data-stu-id="8aac5-187">Int32</span></span>|<span data-ttu-id="8aac5-188">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="8aac5-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="8aac5-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="8aac5-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="8aac5-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-190">Boolean</span></span>|<span data-ttu-id="8aac5-191">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="8aac5-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="8aac5-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8aac5-192">osMinimumVersion</span></span>|<span data-ttu-id="8aac5-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8aac5-193">String</span></span>|<span data-ttu-id="8aac5-194">Mindestversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="8aac5-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="8aac5-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8aac5-195">osMaximumVersion</span></span>|<span data-ttu-id="8aac5-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8aac5-196">String</span></span>|<span data-ttu-id="8aac5-197">Maximalversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="8aac5-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="8aac5-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8aac5-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="8aac5-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8aac5-199">String</span></span>|<span data-ttu-id="8aac5-200">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="8aac5-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="8aac5-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8aac5-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="8aac5-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8aac5-202">String</span></span>|<span data-ttu-id="8aac5-203">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="8aac5-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="8aac5-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="8aac5-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="8aac5-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-205">Boolean</span></span>|<span data-ttu-id="8aac5-206">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="8aac5-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="8aac5-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="8aac5-207">bitLockerEnabled</span></span>|<span data-ttu-id="8aac5-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-208">Boolean</span></span>|<span data-ttu-id="8aac5-209">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="8aac5-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="8aac5-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="8aac5-210">secureBootEnabled</span></span>|<span data-ttu-id="8aac5-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-211">Boolean</span></span>|<span data-ttu-id="8aac5-212">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="8aac5-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="8aac5-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="8aac5-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="8aac5-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-214">Boolean</span></span>|<span data-ttu-id="8aac5-215">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="8aac5-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="8aac5-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="8aac5-216">storageRequireEncryption</span></span>|<span data-ttu-id="8aac5-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-217">Boolean</span></span>|<span data-ttu-id="8aac5-218">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="8aac5-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="8aac5-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="8aac5-219">activeFirewallRequired</span></span>|<span data-ttu-id="8aac5-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-220">Boolean</span></span>|<span data-ttu-id="8aac5-221">Erfordern Sie active Firewall auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="8aac5-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="8aac5-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="8aac5-222">defenderEnabled</span></span>|<span data-ttu-id="8aac5-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-223">Boolean</span></span>|<span data-ttu-id="8aac5-224">Benötigen Sie Windows Defender Modul auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="8aac5-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="8aac5-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="8aac5-225">defenderVersion</span></span>|<span data-ttu-id="8aac5-226">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8aac5-226">String</span></span>|<span data-ttu-id="8aac5-227">Benötigen Sie mindestens Version von Windows Defender Modul auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="8aac5-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="8aac5-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="8aac5-228">signatureOutOfDate</span></span>|<span data-ttu-id="8aac5-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-229">Boolean</span></span>|<span data-ttu-id="8aac5-230">Benötigen Sie Windows Defender Modul Signatur, um auf Windows-Geräten Stand sein.</span><span class="sxs-lookup"><span data-stu-id="8aac5-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="8aac5-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="8aac5-231">rtpEnabled</span></span>|<span data-ttu-id="8aac5-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-232">Boolean</span></span>|<span data-ttu-id="8aac5-233">Benötigen Sie Windows Defender Modul Real-Time Schutz auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="8aac5-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="8aac5-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="8aac5-234">antivirusRequired</span></span>|<span data-ttu-id="8aac5-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-235">Boolean</span></span>|<span data-ttu-id="8aac5-236">Erfordern Sie Antivirus-Lösung mit Windows Decurity Center befinden registriert und Überwachung (z. B. Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="8aac5-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="8aac5-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="8aac5-237">antiSpywareRequired</span></span>|<span data-ttu-id="8aac5-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-238">Boolean</span></span>|<span data-ttu-id="8aac5-239">Erfordern Sie AntiSpyware-Lösung mit Windows Decurity Center befinden registriert und Überwachung (z. B. Symantec, Windows Defender).</span><span class="sxs-lookup"><span data-stu-id="8aac5-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="8aac5-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="8aac5-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="8aac5-241">[OperatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8aac5-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="8aac5-242">Das gültige Betriebssystem erstellen Bereiche auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="8aac5-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="8aac5-243">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="8aac5-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="8aac5-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="8aac5-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="8aac5-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-245">Boolean</span></span>|<span data-ttu-id="8aac5-246">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="8aac5-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="8aac5-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8aac5-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="8aac5-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="8aac5-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="8aac5-249">Erfordern Sie Gerät Bedrohung minimalem Risiko Mail-Schutzstufe Kompatibilität vorgesehenen Unwichtigstes.</span><span class="sxs-lookup"><span data-stu-id="8aac5-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="8aac5-250">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="8aac5-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="8aac5-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="8aac5-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="8aac5-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="8aac5-252">Boolean</span></span>|<span data-ttu-id="8aac5-253">SCCM Compliance Zustand berücksichtigt für Intune Compliance Zustand berücksichtigen müssen.</span><span class="sxs-lookup"><span data-stu-id="8aac5-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="8aac5-254">Antwort</span><span class="sxs-lookup"><span data-stu-id="8aac5-254">Response</span></span>
<span data-ttu-id="8aac5-255">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8aac5-255">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8aac5-256">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8aac5-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="8aac5-257">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8aac5-257">Request</span></span>
<span data-ttu-id="8aac5-258">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8aac5-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1666

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
  "configurationManagerComplianceRequired": true
}
```

### <a name="response"></a><span data-ttu-id="8aac5-259">Antwort</span><span class="sxs-lookup"><span data-stu-id="8aac5-259">Response</span></span>
<span data-ttu-id="8aac5-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8aac5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




