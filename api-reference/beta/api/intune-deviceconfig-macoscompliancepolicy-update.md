---
title: macOSCompliancePolicy aktualisieren
description: Aktualisieren der Eigenschaften eines macOSCompliancePolicy-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 79adb9263fc1e6e8fffc341be0a3bc31b46e3480
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404015"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="003a9-103">macOSCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="003a9-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="003a9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="003a9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="003a9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="003a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="003a9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="003a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="003a9-107">Aktualisieren der Eigenschaften eines [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="003a9-107">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="003a9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="003a9-108">Prerequisites</span></span>
<span data-ttu-id="003a9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="003a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="003a9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="003a9-111">Permission type</span></span>|<span data-ttu-id="003a9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="003a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="003a9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="003a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="003a9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="003a9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="003a9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="003a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="003a9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="003a9-116">Not supported.</span></span>|
|<span data-ttu-id="003a9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="003a9-117">Application</span></span>|<span data-ttu-id="003a9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="003a9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="003a9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="003a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="003a9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="003a9-120">Request headers</span></span>
|<span data-ttu-id="003a9-121">Header</span><span class="sxs-lookup"><span data-stu-id="003a9-121">Header</span></span>|<span data-ttu-id="003a9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="003a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="003a9-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="003a9-123">Authorization</span></span>|<span data-ttu-id="003a9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="003a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="003a9-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="003a9-125">Accept</span></span>|<span data-ttu-id="003a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="003a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="003a9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="003a9-127">Request body</span></span>
<span data-ttu-id="003a9-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="003a9-128">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="003a9-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="003a9-129">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="003a9-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="003a9-130">Property</span></span>|<span data-ttu-id="003a9-131">Typ</span><span class="sxs-lookup"><span data-stu-id="003a9-131">Type</span></span>|<span data-ttu-id="003a9-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="003a9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="003a9-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="003a9-133">roleScopeTagIds</span></span>|<span data-ttu-id="003a9-134">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="003a9-134">String collection</span></span>|<span data-ttu-id="003a9-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="003a9-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="003a9-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="003a9-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="003a9-137">id</span><span class="sxs-lookup"><span data-stu-id="003a9-137">id</span></span>|<span data-ttu-id="003a9-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="003a9-138">String</span></span>|<span data-ttu-id="003a9-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="003a9-139">Key of the entity.</span></span> <span data-ttu-id="003a9-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="003a9-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="003a9-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="003a9-141">createdDateTime</span></span>|<span data-ttu-id="003a9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="003a9-142">DateTimeOffset</span></span>|<span data-ttu-id="003a9-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="003a9-143">DateTime the object was created.</span></span> <span data-ttu-id="003a9-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="003a9-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="003a9-145">description</span><span class="sxs-lookup"><span data-stu-id="003a9-145">description</span></span>|<span data-ttu-id="003a9-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="003a9-146">String</span></span>|<span data-ttu-id="003a9-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="003a9-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="003a9-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="003a9-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="003a9-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="003a9-149">lastModifiedDateTime</span></span>|<span data-ttu-id="003a9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="003a9-150">DateTimeOffset</span></span>|<span data-ttu-id="003a9-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="003a9-151">DateTime the object was last modified.</span></span> <span data-ttu-id="003a9-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="003a9-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="003a9-153">displayName</span><span class="sxs-lookup"><span data-stu-id="003a9-153">displayName</span></span>|<span data-ttu-id="003a9-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="003a9-154">String</span></span>|<span data-ttu-id="003a9-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="003a9-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="003a9-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="003a9-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="003a9-157">Version</span><span class="sxs-lookup"><span data-stu-id="003a9-157">version</span></span>|<span data-ttu-id="003a9-158">Int32</span><span class="sxs-lookup"><span data-stu-id="003a9-158">Int32</span></span>|<span data-ttu-id="003a9-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="003a9-159">Version of the device configuration.</span></span> <span data-ttu-id="003a9-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="003a9-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="003a9-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="003a9-161">passwordRequired</span></span>|<span data-ttu-id="003a9-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="003a9-162">Boolean</span></span>|<span data-ttu-id="003a9-163">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="003a9-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="003a9-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="003a9-164">passwordBlockSimple</span></span>|<span data-ttu-id="003a9-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="003a9-165">Boolean</span></span>|<span data-ttu-id="003a9-166">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="003a9-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="003a9-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="003a9-167">passwordExpirationDays</span></span>|<span data-ttu-id="003a9-168">Int32</span><span class="sxs-lookup"><span data-stu-id="003a9-168">Int32</span></span>|<span data-ttu-id="003a9-169">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="003a9-169">Number of days before the password expires.</span></span> <span data-ttu-id="003a9-170">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="003a9-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="003a9-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="003a9-171">passwordMinimumLength</span></span>|<span data-ttu-id="003a9-172">Int32</span><span class="sxs-lookup"><span data-stu-id="003a9-172">Int32</span></span>|<span data-ttu-id="003a9-173">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="003a9-173">Minimum length of password.</span></span> <span data-ttu-id="003a9-174">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="003a9-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="003a9-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="003a9-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="003a9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="003a9-176">Int32</span></span>|<span data-ttu-id="003a9-177">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="003a9-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="003a9-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="003a9-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="003a9-179">Int32</span><span class="sxs-lookup"><span data-stu-id="003a9-179">Int32</span></span>|<span data-ttu-id="003a9-180">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="003a9-180">Number of previous passwords to block.</span></span> <span data-ttu-id="003a9-181">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="003a9-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="003a9-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="003a9-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="003a9-183">Int32</span><span class="sxs-lookup"><span data-stu-id="003a9-183">Int32</span></span>|<span data-ttu-id="003a9-184">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="003a9-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="003a9-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="003a9-185">passwordRequiredType</span></span>|[<span data-ttu-id="003a9-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="003a9-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="003a9-187">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="003a9-187">The required password type.</span></span> <span data-ttu-id="003a9-188">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="003a9-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="003a9-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="003a9-189">osMinimumVersion</span></span>|<span data-ttu-id="003a9-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="003a9-190">String</span></span>|<span data-ttu-id="003a9-191">Mac OS Mindestversion.</span><span class="sxs-lookup"><span data-stu-id="003a9-191">Minimum MacOS version.</span></span>|
|<span data-ttu-id="003a9-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="003a9-192">osMaximumVersion</span></span>|<span data-ttu-id="003a9-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="003a9-193">String</span></span>|<span data-ttu-id="003a9-194">Maximale Mac OS-Version.</span><span class="sxs-lookup"><span data-stu-id="003a9-194">Maximum MacOS version.</span></span>|
|<span data-ttu-id="003a9-195">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="003a9-195">osMinimumBuildVersion</span></span>|<span data-ttu-id="003a9-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="003a9-196">String</span></span>|<span data-ttu-id="003a9-197">Minimale Mac OS Buildversion.</span><span class="sxs-lookup"><span data-stu-id="003a9-197">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="003a9-198">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="003a9-198">osMaximumBuildVersion</span></span>|<span data-ttu-id="003a9-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="003a9-199">String</span></span>|<span data-ttu-id="003a9-200">Maximale Mac OS Buildversion.</span><span class="sxs-lookup"><span data-stu-id="003a9-200">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="003a9-201">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="003a9-201">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="003a9-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="003a9-202">Boolean</span></span>|<span data-ttu-id="003a9-203">Gibt an, ob auf Geräten der Systemintegritätsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="003a9-203">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="003a9-204">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="003a9-204">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="003a9-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="003a9-205">Boolean</span></span>|<span data-ttu-id="003a9-206">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="003a9-206">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="003a9-207">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="003a9-207">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="003a9-208">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="003a9-208">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="003a9-209">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="003a9-209">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="003a9-210">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="003a9-210">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="003a9-211">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="003a9-211">storageRequireEncryption</span></span>|<span data-ttu-id="003a9-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="003a9-212">Boolean</span></span>|<span data-ttu-id="003a9-213">Gibt an, ob auf Mac OS-Geräten die Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="003a9-213">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="003a9-214">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="003a9-214">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="003a9-215">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="003a9-215">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="003a9-216">System und den Datenschutz, der bestimmt, welche Download Speicherorte apps auf einem Mac OS-Gerät aus ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="003a9-216">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="003a9-217">Mögliche Werte: sind `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers` und `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="003a9-217">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="003a9-218">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="003a9-218">firewallEnabled</span></span>|<span data-ttu-id="003a9-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="003a9-219">Boolean</span></span>|<span data-ttu-id="003a9-220">Gibt an, ob die Firewall oder nicht aktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="003a9-220">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="003a9-221">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="003a9-221">firewallBlockAllIncoming</span></span>|<span data-ttu-id="003a9-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="003a9-222">Boolean</span></span>|<span data-ttu-id="003a9-223">Entspricht der Option "Alle eingehende Verbindungen blockieren".</span><span class="sxs-lookup"><span data-stu-id="003a9-223">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="003a9-224">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="003a9-224">firewallEnableStealthMode</span></span>|<span data-ttu-id="003a9-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="003a9-225">Boolean</span></span>|<span data-ttu-id="003a9-226">Entspricht "Enable Tarnmodus."</span><span class="sxs-lookup"><span data-stu-id="003a9-226">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="003a9-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="003a9-227">Response</span></span>
<span data-ttu-id="003a9-228">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="003a9-228">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="003a9-229">Beispiel</span><span class="sxs-lookup"><span data-stu-id="003a9-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="003a9-230">Anforderung</span><span class="sxs-lookup"><span data-stu-id="003a9-230">Request</span></span>
<span data-ttu-id="003a9-231">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="003a9-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1083

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="003a9-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="003a9-232">Response</span></span>
<span data-ttu-id="003a9-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="003a9-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1255

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```




