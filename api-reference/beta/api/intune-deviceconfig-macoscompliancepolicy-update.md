---
title: macOSCompliancePolicy aktualisieren
description: Aktualisieren der Eigenschaften eines macOSCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44d6f0e4aaddbed4ab1b4820916949397d271fee
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141895"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="0d778-103">macOSCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0d778-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="0d778-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d778-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d778-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0d778-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d778-106">Aktualisieren der Eigenschaften eines [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d778-106">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d778-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0d778-107">Prerequisites</span></span>
<span data-ttu-id="0d778-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0d778-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0d778-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d778-110">Permission type</span></span>|<span data-ttu-id="0d778-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d778-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d778-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d778-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d778-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d778-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d778-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d778-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d778-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d778-115">Not supported.</span></span>|
|<span data-ttu-id="0d778-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d778-116">Application</span></span>|<span data-ttu-id="0d778-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d778-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d778-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d778-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="0d778-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d778-119">Request headers</span></span>
|<span data-ttu-id="0d778-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0d778-120">Header</span></span>|<span data-ttu-id="0d778-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0d778-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d778-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d778-122">Authorization</span></span>|<span data-ttu-id="0d778-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0d778-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d778-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0d778-124">Accept</span></span>|<span data-ttu-id="0d778-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d778-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d778-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d778-126">Request body</span></span>
<span data-ttu-id="0d778-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0d778-127">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="0d778-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0d778-128">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="0d778-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d778-129">Property</span></span>|<span data-ttu-id="0d778-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0d778-130">Type</span></span>|<span data-ttu-id="0d778-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d778-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d778-132">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="0d778-132">roleScopeTagIds</span></span>|<span data-ttu-id="0d778-133">String collection</span><span class="sxs-lookup"><span data-stu-id="0d778-133">String collection</span></span>|<span data-ttu-id="0d778-134">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="0d778-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0d778-135">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d778-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d778-136">id</span><span class="sxs-lookup"><span data-stu-id="0d778-136">id</span></span>|<span data-ttu-id="0d778-137">string</span><span class="sxs-lookup"><span data-stu-id="0d778-137">String</span></span>|<span data-ttu-id="0d778-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0d778-138">Key of the entity.</span></span> <span data-ttu-id="0d778-139">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d778-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d778-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d778-140">createdDateTime</span></span>|<span data-ttu-id="0d778-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d778-141">DateTimeOffset</span></span>|<span data-ttu-id="0d778-142">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d778-142">DateTime the object was created.</span></span> <span data-ttu-id="0d778-143">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d778-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d778-144">description</span><span class="sxs-lookup"><span data-stu-id="0d778-144">description</span></span>|<span data-ttu-id="0d778-145">String</span><span class="sxs-lookup"><span data-stu-id="0d778-145">String</span></span>|<span data-ttu-id="0d778-146">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0d778-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0d778-147">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d778-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d778-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d778-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0d778-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d778-149">DateTimeOffset</span></span>|<span data-ttu-id="0d778-150">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d778-150">DateTime the object was last modified.</span></span> <span data-ttu-id="0d778-151">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d778-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d778-152">displayName</span><span class="sxs-lookup"><span data-stu-id="0d778-152">displayName</span></span>|<span data-ttu-id="0d778-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d778-153">String</span></span>|<span data-ttu-id="0d778-154">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0d778-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0d778-155">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d778-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d778-156">Version</span><span class="sxs-lookup"><span data-stu-id="0d778-156">version</span></span>|<span data-ttu-id="0d778-157">Int32</span><span class="sxs-lookup"><span data-stu-id="0d778-157">Int32</span></span>|<span data-ttu-id="0d778-158">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0d778-158">Version of the device configuration.</span></span> <span data-ttu-id="0d778-159">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0d778-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0d778-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0d778-160">passwordRequired</span></span>|<span data-ttu-id="0d778-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0d778-161">Boolean</span></span>|<span data-ttu-id="0d778-162">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="0d778-162">Whether or not to require a password.</span></span>|
|<span data-ttu-id="0d778-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0d778-163">passwordBlockSimple</span></span>|<span data-ttu-id="0d778-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0d778-164">Boolean</span></span>|<span data-ttu-id="0d778-165">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="0d778-165">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="0d778-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0d778-166">passwordExpirationDays</span></span>|<span data-ttu-id="0d778-167">Int32</span><span class="sxs-lookup"><span data-stu-id="0d778-167">Int32</span></span>|<span data-ttu-id="0d778-168">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="0d778-168">Number of days before the password expires.</span></span> <span data-ttu-id="0d778-169">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="0d778-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0d778-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0d778-170">passwordMinimumLength</span></span>|<span data-ttu-id="0d778-171">Int32</span><span class="sxs-lookup"><span data-stu-id="0d778-171">Int32</span></span>|<span data-ttu-id="0d778-172">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="0d778-172">Minimum length of password.</span></span> <span data-ttu-id="0d778-173">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="0d778-173">Valid values 4 to 14</span></span>|
|<span data-ttu-id="0d778-174">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0d778-174">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0d778-175">Int32</span><span class="sxs-lookup"><span data-stu-id="0d778-175">Int32</span></span>|<span data-ttu-id="0d778-176">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="0d778-176">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0d778-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0d778-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0d778-178">Int32</span><span class="sxs-lookup"><span data-stu-id="0d778-178">Int32</span></span>|<span data-ttu-id="0d778-179">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="0d778-179">Number of previous passwords to block.</span></span> <span data-ttu-id="0d778-180">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="0d778-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="0d778-181">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0d778-181">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0d778-182">Int32</span><span class="sxs-lookup"><span data-stu-id="0d778-182">Int32</span></span>|<span data-ttu-id="0d778-183">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="0d778-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0d778-184">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0d778-184">passwordRequiredType</span></span>|[<span data-ttu-id="0d778-185">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0d778-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0d778-186">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="0d778-186">The required password type.</span></span> <span data-ttu-id="0d778-187">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="0d778-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0d778-188">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0d778-188">osMinimumVersion</span></span>|<span data-ttu-id="0d778-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d778-189">String</span></span>|<span data-ttu-id="0d778-190">Mindestens MacOS-Version.</span><span class="sxs-lookup"><span data-stu-id="0d778-190">Minimum MacOS version.</span></span>|
|<span data-ttu-id="0d778-191">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0d778-191">osMaximumVersion</span></span>|<span data-ttu-id="0d778-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d778-192">String</span></span>|<span data-ttu-id="0d778-193">Maximale MacOS-Version.</span><span class="sxs-lookup"><span data-stu-id="0d778-193">Maximum MacOS version.</span></span>|
|<span data-ttu-id="0d778-194">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="0d778-194">osMinimumBuildVersion</span></span>|<span data-ttu-id="0d778-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d778-195">String</span></span>|<span data-ttu-id="0d778-196">Mindestens Version der MacOS-Buildversion.</span><span class="sxs-lookup"><span data-stu-id="0d778-196">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="0d778-197">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="0d778-197">osMaximumBuildVersion</span></span>|<span data-ttu-id="0d778-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d778-198">String</span></span>|<span data-ttu-id="0d778-199">Maximale Version des MacOS-Builds.</span><span class="sxs-lookup"><span data-stu-id="0d778-199">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="0d778-200">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0d778-200">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="0d778-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d778-201">Boolean</span></span>|<span data-ttu-id="0d778-202">Gibt an, ob auf Geräten der Systemintegritätsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="0d778-202">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="0d778-203">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0d778-203">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="0d778-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0d778-204">Boolean</span></span>|<span data-ttu-id="0d778-205">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="0d778-205">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="0d778-206">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0d778-206">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="0d778-207">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="0d778-207">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="0d778-208">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="0d778-208">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="0d778-209">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="0d778-209">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="0d778-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0d778-210">storageRequireEncryption</span></span>|<span data-ttu-id="0d778-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d778-211">Boolean</span></span>|<span data-ttu-id="0d778-212">Gibt an, ob auf Mac OS-Geräten die Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="0d778-212">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="0d778-213">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="0d778-213">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="0d778-214">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="0d778-214">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="0d778-215">System-und Datenschutzeinstellung, die bestimmt, welche Downloadspeicherorte apps auf einem macOS-Gerät ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="0d778-215">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="0d778-216">Mögliche Werte: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="0d778-216">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="0d778-217">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="0d778-217">firewallEnabled</span></span>|<span data-ttu-id="0d778-218">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0d778-218">Boolean</span></span>|<span data-ttu-id="0d778-219">Ob die Firewall aktiviert werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="0d778-219">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="0d778-220">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="0d778-220">firewallBlockAllIncoming</span></span>|<span data-ttu-id="0d778-221">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0d778-221">Boolean</span></span>|<span data-ttu-id="0d778-222">Entspricht der Option "alle eingehenden Verbindungen blockieren".</span><span class="sxs-lookup"><span data-stu-id="0d778-222">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="0d778-223">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="0d778-223">firewallEnableStealthMode</span></span>|<span data-ttu-id="0d778-224">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0d778-224">Boolean</span></span>|<span data-ttu-id="0d778-225">Entspricht "Stealth-Modus aktivieren".</span><span class="sxs-lookup"><span data-stu-id="0d778-225">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="0d778-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d778-226">Response</span></span>
<span data-ttu-id="0d778-227">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0d778-227">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d778-228">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d778-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d778-229">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d778-229">Request</span></span>
<span data-ttu-id="0d778-230">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d778-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d778-231">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d778-231">Response</span></span>
<span data-ttu-id="0d778-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d778-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




