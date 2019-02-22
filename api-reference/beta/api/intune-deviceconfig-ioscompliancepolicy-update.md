---
title: iosCompliancePolicy aktualisieren
description: Aktualisieren der Eigenschaften eines iosCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 524ffd9bbaf7b6a0e5d1e912d52af8137e59049f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167697"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="6e48d-103">iosCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6e48d-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="6e48d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6e48d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e48d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6e48d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e48d-106">Aktualisieren der Eigenschaften eines [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6e48d-106">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e48d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6e48d-107">Prerequisites</span></span>
<span data-ttu-id="6e48d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6e48d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6e48d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6e48d-110">Permission type</span></span>|<span data-ttu-id="6e48d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6e48d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e48d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6e48d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e48d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e48d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e48d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6e48d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e48d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e48d-115">Not supported.</span></span>|
|<span data-ttu-id="6e48d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6e48d-116">Application</span></span>|<span data-ttu-id="6e48d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e48d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e48d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e48d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6e48d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6e48d-119">Request headers</span></span>
|<span data-ttu-id="6e48d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6e48d-120">Header</span></span>|<span data-ttu-id="6e48d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6e48d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e48d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e48d-122">Authorization</span></span>|<span data-ttu-id="6e48d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6e48d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e48d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6e48d-124">Accept</span></span>|<span data-ttu-id="6e48d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6e48d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e48d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6e48d-126">Request body</span></span>
<span data-ttu-id="6e48d-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="6e48d-127">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="6e48d-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6e48d-128">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="6e48d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6e48d-129">Property</span></span>|<span data-ttu-id="6e48d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6e48d-130">Type</span></span>|<span data-ttu-id="6e48d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e48d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e48d-132">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="6e48d-132">roleScopeTagIds</span></span>|<span data-ttu-id="6e48d-133">String collection</span><span class="sxs-lookup"><span data-stu-id="6e48d-133">String collection</span></span>|<span data-ttu-id="6e48d-134">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="6e48d-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6e48d-135">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e48d-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e48d-136">id</span><span class="sxs-lookup"><span data-stu-id="6e48d-136">id</span></span>|<span data-ttu-id="6e48d-137">string</span><span class="sxs-lookup"><span data-stu-id="6e48d-137">String</span></span>|<span data-ttu-id="6e48d-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6e48d-138">Key of the entity.</span></span> <span data-ttu-id="6e48d-139">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e48d-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e48d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e48d-140">createdDateTime</span></span>|<span data-ttu-id="6e48d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e48d-141">DateTimeOffset</span></span>|<span data-ttu-id="6e48d-142">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6e48d-142">DateTime the object was created.</span></span> <span data-ttu-id="6e48d-143">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e48d-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e48d-144">description</span><span class="sxs-lookup"><span data-stu-id="6e48d-144">description</span></span>|<span data-ttu-id="6e48d-145">String</span><span class="sxs-lookup"><span data-stu-id="6e48d-145">String</span></span>|<span data-ttu-id="6e48d-146">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6e48d-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6e48d-147">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e48d-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e48d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e48d-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6e48d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e48d-149">DateTimeOffset</span></span>|<span data-ttu-id="6e48d-150">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6e48d-150">DateTime the object was last modified.</span></span> <span data-ttu-id="6e48d-151">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e48d-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e48d-152">displayName</span><span class="sxs-lookup"><span data-stu-id="6e48d-152">displayName</span></span>|<span data-ttu-id="6e48d-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6e48d-153">String</span></span>|<span data-ttu-id="6e48d-154">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6e48d-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6e48d-155">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e48d-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e48d-156">Version</span><span class="sxs-lookup"><span data-stu-id="6e48d-156">version</span></span>|<span data-ttu-id="6e48d-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6e48d-157">Int32</span></span>|<span data-ttu-id="6e48d-158">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6e48d-158">Version of the device configuration.</span></span> <span data-ttu-id="6e48d-159">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6e48d-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e48d-160">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6e48d-160">passcodeBlockSimple</span></span>|<span data-ttu-id="6e48d-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6e48d-161">Boolean</span></span>|<span data-ttu-id="6e48d-162">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="6e48d-162">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="6e48d-163">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6e48d-163">passcodeExpirationDays</span></span>|<span data-ttu-id="6e48d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6e48d-164">Int32</span></span>|<span data-ttu-id="6e48d-165">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="6e48d-165">Number of days before the passcode expires.</span></span> <span data-ttu-id="6e48d-166">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="6e48d-166">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6e48d-167">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6e48d-167">passcodeMinimumLength</span></span>|<span data-ttu-id="6e48d-168">Int32</span><span class="sxs-lookup"><span data-stu-id="6e48d-168">Int32</span></span>|<span data-ttu-id="6e48d-169">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="6e48d-169">Minimum length of passcode.</span></span> <span data-ttu-id="6e48d-170">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="6e48d-170">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6e48d-171">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6e48d-171">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6e48d-172">Int32</span><span class="sxs-lookup"><span data-stu-id="6e48d-172">Int32</span></span>|<span data-ttu-id="6e48d-173">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="6e48d-173">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="6e48d-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6e48d-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6e48d-175">Int32</span><span class="sxs-lookup"><span data-stu-id="6e48d-175">Int32</span></span>|<span data-ttu-id="6e48d-176">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="6e48d-176">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6e48d-177">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="6e48d-177">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="6e48d-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6e48d-178">Int32</span></span>|<span data-ttu-id="6e48d-179">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="6e48d-179">Number of previous passcodes to block.</span></span> <span data-ttu-id="6e48d-180">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="6e48d-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6e48d-181">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6e48d-181">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="6e48d-182">Int32</span><span class="sxs-lookup"><span data-stu-id="6e48d-182">Int32</span></span>|<span data-ttu-id="6e48d-183">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="6e48d-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6e48d-184">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="6e48d-184">passcodeRequiredType</span></span>|[<span data-ttu-id="6e48d-185">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6e48d-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6e48d-186">Der erforderliche Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="6e48d-186">The required passcode type.</span></span> <span data-ttu-id="6e48d-187">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6e48d-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6e48d-188">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="6e48d-188">passcodeRequired</span></span>|<span data-ttu-id="6e48d-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6e48d-189">Boolean</span></span>|<span data-ttu-id="6e48d-190">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="6e48d-190">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="6e48d-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6e48d-191">osMinimumVersion</span></span>|<span data-ttu-id="6e48d-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6e48d-192">String</span></span>|<span data-ttu-id="6e48d-193">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="6e48d-193">Minimum IOS version.</span></span>|
|<span data-ttu-id="6e48d-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6e48d-194">osMaximumVersion</span></span>|<span data-ttu-id="6e48d-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6e48d-195">String</span></span>|<span data-ttu-id="6e48d-196">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="6e48d-196">Maximum IOS version.</span></span>|
|<span data-ttu-id="6e48d-197">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="6e48d-197">osMinimumBuildVersion</span></span>|<span data-ttu-id="6e48d-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6e48d-198">String</span></span>|<span data-ttu-id="6e48d-199">Mindestens IOS-Buildversion.</span><span class="sxs-lookup"><span data-stu-id="6e48d-199">Minimum IOS build version.</span></span>|
|<span data-ttu-id="6e48d-200">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="6e48d-200">osMaximumBuildVersion</span></span>|<span data-ttu-id="6e48d-201">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6e48d-201">String</span></span>|<span data-ttu-id="6e48d-202">Maximale IOS-Buildversion.</span><span class="sxs-lookup"><span data-stu-id="6e48d-202">Maximum IOS build version.</span></span>|
|<span data-ttu-id="6e48d-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="6e48d-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="6e48d-204">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6e48d-204">Boolean</span></span>|<span data-ttu-id="6e48d-205">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="6e48d-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="6e48d-206">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6e48d-206">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6e48d-207">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6e48d-207">Boolean</span></span>|<span data-ttu-id="6e48d-208">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="6e48d-208">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="6e48d-209">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6e48d-209">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6e48d-210">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="6e48d-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6e48d-211">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="6e48d-211">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6e48d-212">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6e48d-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6e48d-213">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="6e48d-213">managedEmailProfileRequired</span></span>|<span data-ttu-id="6e48d-214">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6e48d-214">Boolean</span></span>|<span data-ttu-id="6e48d-215">Gibt an, ob ein verwaltetes E-Mail-Profil erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="6e48d-215">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="6e48d-216">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="6e48d-216">restrictedApps</span></span>|<span data-ttu-id="6e48d-217">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6e48d-217">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6e48d-218">Das Gerät muss nicht über die angegebenen apps verfügen.</span><span class="sxs-lookup"><span data-stu-id="6e48d-218">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="6e48d-219">Diese Auflistung kann maximal 100 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="6e48d-219">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6e48d-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e48d-220">Response</span></span>
<span data-ttu-id="6e48d-221">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6e48d-221">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e48d-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6e48d-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e48d-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e48d-223">Request</span></span>
<span data-ttu-id="6e48d-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6e48d-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1241

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6e48d-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e48d-225">Response</span></span>
<span data-ttu-id="6e48d-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6e48d-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1413

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```




