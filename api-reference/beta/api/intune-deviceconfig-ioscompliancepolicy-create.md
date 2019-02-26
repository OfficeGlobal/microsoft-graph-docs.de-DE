---
title: iosCompliancePolicy erstellen
description: Erstellen eines neuen iosCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 744c795a67cd240b03127419f9c00068df8e702a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166199"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="ebdca-103">iosCompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="ebdca-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="ebdca-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ebdca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebdca-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ebdca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebdca-106">Erstellen eines neuen [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ebdca-106">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebdca-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ebdca-107">Prerequisites</span></span>
<span data-ttu-id="ebdca-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ebdca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ebdca-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ebdca-110">Permission type</span></span>|<span data-ttu-id="ebdca-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ebdca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebdca-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ebdca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebdca-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebdca-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ebdca-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ebdca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebdca-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ebdca-115">Not supported.</span></span>|
|<span data-ttu-id="ebdca-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ebdca-116">Application</span></span>|<span data-ttu-id="ebdca-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ebdca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebdca-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebdca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ebdca-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ebdca-119">Request headers</span></span>
|<span data-ttu-id="ebdca-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ebdca-120">Header</span></span>|<span data-ttu-id="ebdca-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ebdca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebdca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebdca-122">Authorization</span></span>|<span data-ttu-id="ebdca-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ebdca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebdca-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ebdca-124">Accept</span></span>|<span data-ttu-id="ebdca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ebdca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebdca-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ebdca-126">Request body</span></span>
<span data-ttu-id="ebdca-127">Geben Sie im Anforderungstext eine JSON-Darstellung des iosCompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ebdca-127">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="ebdca-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosCompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ebdca-128">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="ebdca-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ebdca-129">Property</span></span>|<span data-ttu-id="ebdca-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ebdca-130">Type</span></span>|<span data-ttu-id="ebdca-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebdca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebdca-132">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="ebdca-132">roleScopeTagIds</span></span>|<span data-ttu-id="ebdca-133">String collection</span><span class="sxs-lookup"><span data-stu-id="ebdca-133">String collection</span></span>|<span data-ttu-id="ebdca-134">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="ebdca-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ebdca-135">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ebdca-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebdca-136">id</span><span class="sxs-lookup"><span data-stu-id="ebdca-136">id</span></span>|<span data-ttu-id="ebdca-137">string</span><span class="sxs-lookup"><span data-stu-id="ebdca-137">String</span></span>|<span data-ttu-id="ebdca-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ebdca-138">Key of the entity.</span></span> <span data-ttu-id="ebdca-139">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ebdca-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebdca-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ebdca-140">createdDateTime</span></span>|<span data-ttu-id="ebdca-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebdca-141">DateTimeOffset</span></span>|<span data-ttu-id="ebdca-142">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ebdca-142">DateTime the object was created.</span></span> <span data-ttu-id="ebdca-143">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ebdca-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebdca-144">description</span><span class="sxs-lookup"><span data-stu-id="ebdca-144">description</span></span>|<span data-ttu-id="ebdca-145">String</span><span class="sxs-lookup"><span data-stu-id="ebdca-145">String</span></span>|<span data-ttu-id="ebdca-146">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ebdca-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ebdca-147">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ebdca-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebdca-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebdca-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ebdca-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebdca-149">DateTimeOffset</span></span>|<span data-ttu-id="ebdca-150">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ebdca-150">DateTime the object was last modified.</span></span> <span data-ttu-id="ebdca-151">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ebdca-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebdca-152">displayName</span><span class="sxs-lookup"><span data-stu-id="ebdca-152">displayName</span></span>|<span data-ttu-id="ebdca-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebdca-153">String</span></span>|<span data-ttu-id="ebdca-154">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ebdca-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ebdca-155">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ebdca-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebdca-156">Version</span><span class="sxs-lookup"><span data-stu-id="ebdca-156">version</span></span>|<span data-ttu-id="ebdca-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ebdca-157">Int32</span></span>|<span data-ttu-id="ebdca-158">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ebdca-158">Version of the device configuration.</span></span> <span data-ttu-id="ebdca-159">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ebdca-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebdca-160">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ebdca-160">passcodeBlockSimple</span></span>|<span data-ttu-id="ebdca-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebdca-161">Boolean</span></span>|<span data-ttu-id="ebdca-162">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="ebdca-162">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="ebdca-163">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ebdca-163">passcodeExpirationDays</span></span>|<span data-ttu-id="ebdca-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ebdca-164">Int32</span></span>|<span data-ttu-id="ebdca-165">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="ebdca-165">Number of days before the passcode expires.</span></span> <span data-ttu-id="ebdca-166">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="ebdca-166">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="ebdca-167">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ebdca-167">passcodeMinimumLength</span></span>|<span data-ttu-id="ebdca-168">Int32</span><span class="sxs-lookup"><span data-stu-id="ebdca-168">Int32</span></span>|<span data-ttu-id="ebdca-169">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="ebdca-169">Minimum length of passcode.</span></span> <span data-ttu-id="ebdca-170">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="ebdca-170">Valid values 4 to 14</span></span>|
|<span data-ttu-id="ebdca-171">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ebdca-171">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ebdca-172">Int32</span><span class="sxs-lookup"><span data-stu-id="ebdca-172">Int32</span></span>|<span data-ttu-id="ebdca-173">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ebdca-173">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="ebdca-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ebdca-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ebdca-175">Int32</span><span class="sxs-lookup"><span data-stu-id="ebdca-175">Int32</span></span>|<span data-ttu-id="ebdca-176">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="ebdca-176">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ebdca-177">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="ebdca-177">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="ebdca-178">Int32</span><span class="sxs-lookup"><span data-stu-id="ebdca-178">Int32</span></span>|<span data-ttu-id="ebdca-179">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="ebdca-179">Number of previous passcodes to block.</span></span> <span data-ttu-id="ebdca-180">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="ebdca-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ebdca-181">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ebdca-181">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="ebdca-182">Int32</span><span class="sxs-lookup"><span data-stu-id="ebdca-182">Int32</span></span>|<span data-ttu-id="ebdca-183">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="ebdca-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ebdca-184">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="ebdca-184">passcodeRequiredType</span></span>|[<span data-ttu-id="ebdca-185">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ebdca-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ebdca-186">Der erforderliche Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="ebdca-186">The required passcode type.</span></span> <span data-ttu-id="ebdca-187">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ebdca-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ebdca-188">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="ebdca-188">passcodeRequired</span></span>|<span data-ttu-id="ebdca-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebdca-189">Boolean</span></span>|<span data-ttu-id="ebdca-190">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ebdca-190">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="ebdca-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ebdca-191">osMinimumVersion</span></span>|<span data-ttu-id="ebdca-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebdca-192">String</span></span>|<span data-ttu-id="ebdca-193">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="ebdca-193">Minimum IOS version.</span></span>|
|<span data-ttu-id="ebdca-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ebdca-194">osMaximumVersion</span></span>|<span data-ttu-id="ebdca-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebdca-195">String</span></span>|<span data-ttu-id="ebdca-196">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="ebdca-196">Maximum IOS version.</span></span>|
|<span data-ttu-id="ebdca-197">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="ebdca-197">osMinimumBuildVersion</span></span>|<span data-ttu-id="ebdca-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebdca-198">String</span></span>|<span data-ttu-id="ebdca-199">Mindestens IOS-Buildversion.</span><span class="sxs-lookup"><span data-stu-id="ebdca-199">Minimum IOS build version.</span></span>|
|<span data-ttu-id="ebdca-200">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="ebdca-200">osMaximumBuildVersion</span></span>|<span data-ttu-id="ebdca-201">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ebdca-201">String</span></span>|<span data-ttu-id="ebdca-202">Maximale IOS-Buildversion.</span><span class="sxs-lookup"><span data-stu-id="ebdca-202">Maximum IOS build version.</span></span>|
|<span data-ttu-id="ebdca-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="ebdca-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="ebdca-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebdca-204">Boolean</span></span>|<span data-ttu-id="ebdca-205">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="ebdca-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="ebdca-206">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ebdca-206">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="ebdca-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebdca-207">Boolean</span></span>|<span data-ttu-id="ebdca-208">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="ebdca-208">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="ebdca-209">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ebdca-209">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="ebdca-210">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="ebdca-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="ebdca-211">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="ebdca-211">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="ebdca-212">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="ebdca-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="ebdca-213">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="ebdca-213">managedEmailProfileRequired</span></span>|<span data-ttu-id="ebdca-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebdca-214">Boolean</span></span>|<span data-ttu-id="ebdca-215">Gibt an, ob ein verwaltetes E-Mail-Profil erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ebdca-215">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="ebdca-216">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="ebdca-216">restrictedApps</span></span>|<span data-ttu-id="ebdca-217">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ebdca-217">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ebdca-218">Das Gerät muss nicht über die angegebenen apps verfügen.</span><span class="sxs-lookup"><span data-stu-id="ebdca-218">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="ebdca-219">Diese Auflistung kann maximal 100 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ebdca-219">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ebdca-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebdca-220">Response</span></span>
<span data-ttu-id="ebdca-221">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebdca-221">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebdca-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ebdca-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebdca-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebdca-223">Request</span></span>
<span data-ttu-id="ebdca-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ebdca-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ebdca-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebdca-225">Response</span></span>
<span data-ttu-id="ebdca-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebdca-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




