---
title: iosCompliancePolicy erstellen
description: Erstellen eines neuen iosCompliancePolicy-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e1fdebc75bfa98d2da83889c0e0e4cbc2ed76a23
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423055"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="e4054-103">iosCompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="e4054-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="e4054-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e4054-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e4054-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4054-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4054-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e4054-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4054-107">Erstellen eines neuen [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4054-107">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4054-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e4054-108">Prerequisites</span></span>
<span data-ttu-id="e4054-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4054-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e4054-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4054-111">Permission type</span></span>|<span data-ttu-id="e4054-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4054-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4054-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4054-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4054-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4054-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4054-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4054-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4054-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4054-116">Not supported.</span></span>|
|<span data-ttu-id="e4054-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4054-117">Application</span></span>|<span data-ttu-id="e4054-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4054-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4054-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4054-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e4054-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4054-120">Request headers</span></span>
|<span data-ttu-id="e4054-121">Header</span><span class="sxs-lookup"><span data-stu-id="e4054-121">Header</span></span>|<span data-ttu-id="e4054-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e4054-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4054-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e4054-123">Authorization</span></span>|<span data-ttu-id="e4054-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e4054-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4054-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e4054-125">Accept</span></span>|<span data-ttu-id="e4054-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4054-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4054-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4054-127">Request body</span></span>
<span data-ttu-id="e4054-128">Geben Sie im Anforderungstext eine JSON-Darstellung des iosCompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e4054-128">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="e4054-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosCompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e4054-129">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="e4054-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e4054-130">Property</span></span>|<span data-ttu-id="e4054-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e4054-131">Type</span></span>|<span data-ttu-id="e4054-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4054-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4054-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e4054-133">roleScopeTagIds</span></span>|<span data-ttu-id="e4054-134">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="e4054-134">String collection</span></span>|<span data-ttu-id="e4054-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="e4054-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e4054-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4054-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4054-137">id</span><span class="sxs-lookup"><span data-stu-id="e4054-137">id</span></span>|<span data-ttu-id="e4054-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4054-138">String</span></span>|<span data-ttu-id="e4054-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e4054-139">Key of the entity.</span></span> <span data-ttu-id="e4054-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4054-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4054-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4054-141">createdDateTime</span></span>|<span data-ttu-id="e4054-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4054-142">DateTimeOffset</span></span>|<span data-ttu-id="e4054-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4054-143">DateTime the object was created.</span></span> <span data-ttu-id="e4054-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4054-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4054-145">description</span><span class="sxs-lookup"><span data-stu-id="e4054-145">description</span></span>|<span data-ttu-id="e4054-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4054-146">String</span></span>|<span data-ttu-id="e4054-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e4054-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e4054-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4054-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4054-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4054-149">lastModifiedDateTime</span></span>|<span data-ttu-id="e4054-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4054-150">DateTimeOffset</span></span>|<span data-ttu-id="e4054-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4054-151">DateTime the object was last modified.</span></span> <span data-ttu-id="e4054-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4054-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4054-153">displayName</span><span class="sxs-lookup"><span data-stu-id="e4054-153">displayName</span></span>|<span data-ttu-id="e4054-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4054-154">String</span></span>|<span data-ttu-id="e4054-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e4054-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e4054-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4054-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4054-157">Version</span><span class="sxs-lookup"><span data-stu-id="e4054-157">version</span></span>|<span data-ttu-id="e4054-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e4054-158">Int32</span></span>|<span data-ttu-id="e4054-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="e4054-159">Version of the device configuration.</span></span> <span data-ttu-id="e4054-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4054-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4054-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e4054-161">passcodeBlockSimple</span></span>|<span data-ttu-id="e4054-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4054-162">Boolean</span></span>|<span data-ttu-id="e4054-163">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="e4054-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="e4054-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e4054-164">passcodeExpirationDays</span></span>|<span data-ttu-id="e4054-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e4054-165">Int32</span></span>|<span data-ttu-id="e4054-166">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="e4054-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="e4054-167">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="e4054-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="e4054-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e4054-168">passcodeMinimumLength</span></span>|<span data-ttu-id="e4054-169">Int32</span><span class="sxs-lookup"><span data-stu-id="e4054-169">Int32</span></span>|<span data-ttu-id="e4054-170">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="e4054-170">Minimum length of passcode.</span></span> <span data-ttu-id="e4054-171">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="e4054-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="e4054-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e4054-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e4054-173">Int32</span><span class="sxs-lookup"><span data-stu-id="e4054-173">Int32</span></span>|<span data-ttu-id="e4054-174">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e4054-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="e4054-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e4054-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e4054-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e4054-176">Int32</span></span>|<span data-ttu-id="e4054-177">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="e4054-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e4054-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="e4054-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="e4054-179">Int32</span><span class="sxs-lookup"><span data-stu-id="e4054-179">Int32</span></span>|<span data-ttu-id="e4054-180">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="e4054-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="e4054-181">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="e4054-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="e4054-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e4054-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="e4054-183">Int32</span><span class="sxs-lookup"><span data-stu-id="e4054-183">Int32</span></span>|<span data-ttu-id="e4054-184">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="e4054-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e4054-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="e4054-185">passcodeRequiredType</span></span>|[<span data-ttu-id="e4054-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e4054-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e4054-187">Der erforderliche Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="e4054-187">The required passcode type.</span></span> <span data-ttu-id="e4054-188">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e4054-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e4054-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="e4054-189">passcodeRequired</span></span>|<span data-ttu-id="e4054-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4054-190">Boolean</span></span>|<span data-ttu-id="e4054-191">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e4054-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="e4054-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e4054-192">osMinimumVersion</span></span>|<span data-ttu-id="e4054-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4054-193">String</span></span>|<span data-ttu-id="e4054-194">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="e4054-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="e4054-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e4054-195">osMaximumVersion</span></span>|<span data-ttu-id="e4054-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4054-196">String</span></span>|<span data-ttu-id="e4054-197">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="e4054-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="e4054-198">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="e4054-198">osMinimumBuildVersion</span></span>|<span data-ttu-id="e4054-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4054-199">String</span></span>|<span data-ttu-id="e4054-200">Minimale IOS Buildversion.</span><span class="sxs-lookup"><span data-stu-id="e4054-200">Minimum IOS build version.</span></span>|
|<span data-ttu-id="e4054-201">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="e4054-201">osMaximumBuildVersion</span></span>|<span data-ttu-id="e4054-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4054-202">String</span></span>|<span data-ttu-id="e4054-203">Maximale IOS Buildversion.</span><span class="sxs-lookup"><span data-stu-id="e4054-203">Maximum IOS build version.</span></span>|
|<span data-ttu-id="e4054-204">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="e4054-204">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="e4054-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4054-205">Boolean</span></span>|<span data-ttu-id="e4054-206">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="e4054-206">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="e4054-207">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e4054-207">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="e4054-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4054-208">Boolean</span></span>|<span data-ttu-id="e4054-209">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="e4054-209">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="e4054-210">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e4054-210">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="e4054-211">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="e4054-211">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="e4054-212">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="e4054-212">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="e4054-213">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="e4054-213">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="e4054-214">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="e4054-214">managedEmailProfileRequired</span></span>|<span data-ttu-id="e4054-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4054-215">Boolean</span></span>|<span data-ttu-id="e4054-216">Gibt an, ob ein verwaltetes E-Mail-Profil erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e4054-216">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="e4054-217">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="e4054-217">restrictedApps</span></span>|<span data-ttu-id="e4054-218">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="e4054-218">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e4054-219">Benötigen Sie das Gerät nicht die angegebenen apps installiert haben.</span><span class="sxs-lookup"><span data-stu-id="e4054-219">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="e4054-220">Diese Sammlung kann maximal 100 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="e4054-220">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e4054-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4054-221">Response</span></span>
<span data-ttu-id="e4054-222">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4054-222">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4054-223">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4054-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4054-224">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4054-224">Request</span></span>
<span data-ttu-id="e4054-225">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4054-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="e4054-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4054-226">Response</span></span>
<span data-ttu-id="e4054-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4054-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




