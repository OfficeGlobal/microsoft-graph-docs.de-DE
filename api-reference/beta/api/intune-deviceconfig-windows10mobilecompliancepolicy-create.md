---
title: Erstellen von „windows10MobileCompliancePolicy“
description: Diese Methode erstellt ein neues Objekt des Typs windows10MobileCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a22eb77108963f7ecf023f335816a4f309deadda
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807119"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="3d1b7-103">Erstellen von „windows10MobileCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="3d1b7-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="3d1b7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d1b7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d1b7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d1b7-107">Diese Methode erstellt ein neues Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3d1b7-107">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d1b7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3d1b7-108">Prerequisites</span></span>
<span data-ttu-id="3d1b7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d1b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d1b7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3d1b7-111">Permission type</span></span>|<span data-ttu-id="3d1b7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3d1b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d1b7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3d1b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d1b7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d1b7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3d1b7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3d1b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d1b7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d1b7-116">Not supported.</span></span>|
|<span data-ttu-id="3d1b7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3d1b7-117">Application</span></span>|<span data-ttu-id="3d1b7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3d1b7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d1b7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d1b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="3d1b7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3d1b7-120">Request headers</span></span>
|<span data-ttu-id="3d1b7-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3d1b7-121">Header</span></span>|<span data-ttu-id="3d1b7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3d1b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d1b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d1b7-123">Authorization</span></span>|<span data-ttu-id="3d1b7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3d1b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d1b7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3d1b7-125">Accept</span></span>|<span data-ttu-id="3d1b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d1b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d1b7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3d1b7-127">Request body</span></span>
<span data-ttu-id="3d1b7-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10MobileCompliancePolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-128">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="3d1b7-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10MobileCompliancePolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-129">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="3d1b7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d1b7-130">Property</span></span>|<span data-ttu-id="3d1b7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3d1b7-131">Type</span></span>|<span data-ttu-id="3d1b7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d1b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d1b7-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3d1b7-133">roleScopeTagIds</span></span>|<span data-ttu-id="3d1b7-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="3d1b7-134">String collection</span></span>|<span data-ttu-id="3d1b7-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3d1b7-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3d1b7-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3d1b7-137">id</span><span class="sxs-lookup"><span data-stu-id="3d1b7-137">id</span></span>|<span data-ttu-id="3d1b7-138">String</span><span class="sxs-lookup"><span data-stu-id="3d1b7-138">String</span></span>|<span data-ttu-id="3d1b7-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3d1b7-139">Key of the entity.</span></span> <span data-ttu-id="3d1b7-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3d1b7-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3d1b7-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d1b7-141">createdDateTime</span></span>|<span data-ttu-id="3d1b7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d1b7-142">DateTimeOffset</span></span>|<span data-ttu-id="3d1b7-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-143">DateTime the object was created.</span></span> <span data-ttu-id="3d1b7-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3d1b7-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3d1b7-145">description</span><span class="sxs-lookup"><span data-stu-id="3d1b7-145">description</span></span>|<span data-ttu-id="3d1b7-146">String</span><span class="sxs-lookup"><span data-stu-id="3d1b7-146">String</span></span>|<span data-ttu-id="3d1b7-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3d1b7-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3d1b7-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3d1b7-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3d1b7-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d1b7-149">lastModifiedDateTime</span></span>|<span data-ttu-id="3d1b7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d1b7-150">DateTimeOffset</span></span>|<span data-ttu-id="3d1b7-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-151">DateTime the object was last modified.</span></span> <span data-ttu-id="3d1b7-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3d1b7-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3d1b7-153">displayName</span><span class="sxs-lookup"><span data-stu-id="3d1b7-153">displayName</span></span>|<span data-ttu-id="3d1b7-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3d1b7-154">String</span></span>|<span data-ttu-id="3d1b7-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3d1b7-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3d1b7-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3d1b7-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3d1b7-157">Version</span><span class="sxs-lookup"><span data-stu-id="3d1b7-157">version</span></span>|<span data-ttu-id="3d1b7-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3d1b7-158">Int32</span></span>|<span data-ttu-id="3d1b7-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-159">Version of the device configuration.</span></span> <span data-ttu-id="3d1b7-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3d1b7-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3d1b7-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3d1b7-161">passwordRequired</span></span>|<span data-ttu-id="3d1b7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d1b7-162">Boolean</span></span>|<span data-ttu-id="3d1b7-163">Legt fest, dass zum Entsperren des Windows Phone-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="3d1b7-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3d1b7-164">passwordBlockSimple</span></span>|<span data-ttu-id="3d1b7-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d1b7-165">Boolean</span></span>|<span data-ttu-id="3d1b7-166">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="3d1b7-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3d1b7-167">passwordMinimumLength</span></span>|<span data-ttu-id="3d1b7-168">Int32</span><span class="sxs-lookup"><span data-stu-id="3d1b7-168">Int32</span></span>|<span data-ttu-id="3d1b7-169">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-169">Minimum password length.</span></span> <span data-ttu-id="3d1b7-170">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="3d1b7-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3d1b7-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="3d1b7-172">Int32</span><span class="sxs-lookup"><span data-stu-id="3d1b7-172">Int32</span></span>|<span data-ttu-id="3d1b7-173">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="3d1b7-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3d1b7-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3d1b7-174">passwordRequiredType</span></span>|[<span data-ttu-id="3d1b7-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3d1b7-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="3d1b7-176">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-176">The required password type.</span></span> <span data-ttu-id="3d1b7-177">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3d1b7-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3d1b7-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3d1b7-179">Int32</span><span class="sxs-lookup"><span data-stu-id="3d1b7-179">Int32</span></span>|<span data-ttu-id="3d1b7-180">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="3d1b7-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3d1b7-181">passwordExpirationDays</span></span>|<span data-ttu-id="3d1b7-182">Int32</span><span class="sxs-lookup"><span data-stu-id="3d1b7-182">Int32</span></span>|<span data-ttu-id="3d1b7-183">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-183">Number of days before password expiration.</span></span> <span data-ttu-id="3d1b7-184">Gültige Werte: 1 bis 255.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="3d1b7-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3d1b7-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3d1b7-186">Int32</span><span class="sxs-lookup"><span data-stu-id="3d1b7-186">Int32</span></span>|<span data-ttu-id="3d1b7-187">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="3d1b7-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="3d1b7-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="3d1b7-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="3d1b7-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d1b7-189">Boolean</span></span>|<span data-ttu-id="3d1b7-190">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="3d1b7-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3d1b7-191">osMinimumVersion</span></span>|<span data-ttu-id="3d1b7-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3d1b7-192">String</span></span>|<span data-ttu-id="3d1b7-193">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="3d1b7-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="3d1b7-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3d1b7-194">osMaximumVersion</span></span>|<span data-ttu-id="3d1b7-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3d1b7-195">String</span></span>|<span data-ttu-id="3d1b7-196">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="3d1b7-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="3d1b7-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="3d1b7-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="3d1b7-198">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3d1b7-198">Boolean</span></span>|<span data-ttu-id="3d1b7-199">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="3d1b7-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="3d1b7-200">bitLockerEnabled</span></span>|<span data-ttu-id="3d1b7-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d1b7-201">Boolean</span></span>|<span data-ttu-id="3d1b7-202">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="3d1b7-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="3d1b7-203">secureBootEnabled</span></span>|<span data-ttu-id="3d1b7-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d1b7-204">Boolean</span></span>|<span data-ttu-id="3d1b7-205">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="3d1b7-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="3d1b7-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="3d1b7-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d1b7-207">Boolean</span></span>|<span data-ttu-id="3d1b7-208">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="3d1b7-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="3d1b7-209">storageRequireEncryption</span></span>|<span data-ttu-id="3d1b7-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d1b7-210">Boolean</span></span>|<span data-ttu-id="3d1b7-211">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="3d1b7-212">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="3d1b7-212">activeFirewallRequired</span></span>|<span data-ttu-id="3d1b7-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d1b7-213">Boolean</span></span>|<span data-ttu-id="3d1b7-214">Erfordern Sie active Firewall auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="3d1b7-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="3d1b7-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="3d1b7-216">[OperatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3d1b7-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="3d1b7-217">Das gültige Betriebssystem erstellen Bereiche auf Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="3d1b7-218">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="3d1b7-219">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d1b7-219">Response</span></span>
<span data-ttu-id="3d1b7-220">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-220">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d1b7-221">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3d1b7-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d1b7-222">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3d1b7-222">Request</span></span>
<span data-ttu-id="3d1b7-223">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1222

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3d1b7-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="3d1b7-224">Response</span></span>
<span data-ttu-id="3d1b7-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3d1b7-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1330

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```





