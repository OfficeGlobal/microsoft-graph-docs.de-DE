---
title: iosCompliancePolicy aktualisieren
description: Aktualisieren der Eigenschaften eines iosCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: db5f4cafa2d12fee7253e14f67d256fda2d03d0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869489"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="4b73b-103">iosCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4b73b-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="4b73b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4b73b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b73b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b73b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b73b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4b73b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b73b-107">Aktualisieren der Eigenschaften eines [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b73b-107">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b73b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4b73b-108">Prerequisites</span></span>
<span data-ttu-id="4b73b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b73b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b73b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b73b-111">Permission type</span></span>|<span data-ttu-id="4b73b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b73b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b73b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b73b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b73b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b73b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b73b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b73b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b73b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b73b-116">Not supported.</span></span>|
|<span data-ttu-id="4b73b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b73b-117">Application</span></span>|<span data-ttu-id="4b73b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b73b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b73b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b73b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="4b73b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b73b-120">Request headers</span></span>
|<span data-ttu-id="4b73b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4b73b-121">Header</span></span>|<span data-ttu-id="4b73b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4b73b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b73b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b73b-123">Authorization</span></span>|<span data-ttu-id="4b73b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4b73b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b73b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4b73b-125">Accept</span></span>|<span data-ttu-id="4b73b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b73b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b73b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b73b-127">Request body</span></span>
<span data-ttu-id="4b73b-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4b73b-128">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="4b73b-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4b73b-129">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="4b73b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b73b-130">Property</span></span>|<span data-ttu-id="4b73b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4b73b-131">Type</span></span>|<span data-ttu-id="4b73b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b73b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b73b-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4b73b-133">roleScopeTagIds</span></span>|<span data-ttu-id="4b73b-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="4b73b-134">String collection</span></span>|<span data-ttu-id="4b73b-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="4b73b-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4b73b-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4b73b-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4b73b-137">id</span><span class="sxs-lookup"><span data-stu-id="4b73b-137">id</span></span>|<span data-ttu-id="4b73b-138">String</span><span class="sxs-lookup"><span data-stu-id="4b73b-138">String</span></span>|<span data-ttu-id="4b73b-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4b73b-139">Key of the entity.</span></span> <span data-ttu-id="4b73b-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4b73b-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4b73b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b73b-141">createdDateTime</span></span>|<span data-ttu-id="4b73b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b73b-142">DateTimeOffset</span></span>|<span data-ttu-id="4b73b-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b73b-143">DateTime the object was created.</span></span> <span data-ttu-id="4b73b-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4b73b-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4b73b-145">description</span><span class="sxs-lookup"><span data-stu-id="4b73b-145">description</span></span>|<span data-ttu-id="4b73b-146">String</span><span class="sxs-lookup"><span data-stu-id="4b73b-146">String</span></span>|<span data-ttu-id="4b73b-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4b73b-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4b73b-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4b73b-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4b73b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b73b-149">lastModifiedDateTime</span></span>|<span data-ttu-id="4b73b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b73b-150">DateTimeOffset</span></span>|<span data-ttu-id="4b73b-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b73b-151">DateTime the object was last modified.</span></span> <span data-ttu-id="4b73b-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4b73b-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4b73b-153">displayName</span><span class="sxs-lookup"><span data-stu-id="4b73b-153">displayName</span></span>|<span data-ttu-id="4b73b-154">String</span><span class="sxs-lookup"><span data-stu-id="4b73b-154">String</span></span>|<span data-ttu-id="4b73b-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4b73b-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4b73b-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4b73b-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4b73b-157">Version</span><span class="sxs-lookup"><span data-stu-id="4b73b-157">version</span></span>|<span data-ttu-id="4b73b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="4b73b-158">Int32</span></span>|<span data-ttu-id="4b73b-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="4b73b-159">Version of the device configuration.</span></span> <span data-ttu-id="4b73b-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4b73b-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4b73b-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4b73b-161">passcodeBlockSimple</span></span>|<span data-ttu-id="4b73b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b73b-162">Boolean</span></span>|<span data-ttu-id="4b73b-163">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="4b73b-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="4b73b-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4b73b-164">passcodeExpirationDays</span></span>|<span data-ttu-id="4b73b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4b73b-165">Int32</span></span>|<span data-ttu-id="4b73b-166">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="4b73b-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="4b73b-167">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="4b73b-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="4b73b-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4b73b-168">passcodeMinimumLength</span></span>|<span data-ttu-id="4b73b-169">Int32</span><span class="sxs-lookup"><span data-stu-id="4b73b-169">Int32</span></span>|<span data-ttu-id="4b73b-170">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="4b73b-170">Minimum length of passcode.</span></span> <span data-ttu-id="4b73b-171">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="4b73b-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="4b73b-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4b73b-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4b73b-173">Int32</span><span class="sxs-lookup"><span data-stu-id="4b73b-173">Int32</span></span>|<span data-ttu-id="4b73b-174">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="4b73b-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="4b73b-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4b73b-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4b73b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4b73b-176">Int32</span></span>|<span data-ttu-id="4b73b-177">Zeitraum von Inaktivität in Minuten, bevor es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="4b73b-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4b73b-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="4b73b-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="4b73b-179">Int32</span><span class="sxs-lookup"><span data-stu-id="4b73b-179">Int32</span></span>|<span data-ttu-id="4b73b-180">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="4b73b-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="4b73b-181">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="4b73b-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="4b73b-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4b73b-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="4b73b-183">Int32</span><span class="sxs-lookup"><span data-stu-id="4b73b-183">Int32</span></span>|<span data-ttu-id="4b73b-184">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="4b73b-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4b73b-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="4b73b-185">passcodeRequiredType</span></span>|[<span data-ttu-id="4b73b-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4b73b-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4b73b-187">Der erforderliche Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="4b73b-187">The required passcode type.</span></span> <span data-ttu-id="4b73b-188">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4b73b-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4b73b-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="4b73b-189">passcodeRequired</span></span>|<span data-ttu-id="4b73b-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b73b-190">Boolean</span></span>|<span data-ttu-id="4b73b-191">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="4b73b-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="4b73b-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4b73b-192">osMinimumVersion</span></span>|<span data-ttu-id="4b73b-193">String</span><span class="sxs-lookup"><span data-stu-id="4b73b-193">String</span></span>|<span data-ttu-id="4b73b-194">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="4b73b-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="4b73b-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4b73b-195">osMaximumVersion</span></span>|<span data-ttu-id="4b73b-196">String</span><span class="sxs-lookup"><span data-stu-id="4b73b-196">String</span></span>|<span data-ttu-id="4b73b-197">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="4b73b-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="4b73b-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="4b73b-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="4b73b-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b73b-199">Boolean</span></span>|<span data-ttu-id="4b73b-200">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="4b73b-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="4b73b-201">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4b73b-201">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="4b73b-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b73b-202">Boolean</span></span>|<span data-ttu-id="4b73b-203">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="4b73b-203">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="4b73b-204">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4b73b-204">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="4b73b-205">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="4b73b-205">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="4b73b-206">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="4b73b-206">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="4b73b-207">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="4b73b-207">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="4b73b-208">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="4b73b-208">managedEmailProfileRequired</span></span>|<span data-ttu-id="4b73b-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b73b-209">Boolean</span></span>|<span data-ttu-id="4b73b-210">Gibt an, ob ein verwaltetes E-Mail-Profil erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="4b73b-210">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="4b73b-211">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="4b73b-211">restrictedApps</span></span>|<span data-ttu-id="4b73b-212">Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4b73b-212">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4b73b-213">Benötigen Sie das Gerät nicht die angegebenen apps installiert haben.</span><span class="sxs-lookup"><span data-stu-id="4b73b-213">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="4b73b-214">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4b73b-214">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4b73b-215">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b73b-215">Response</span></span>
<span data-ttu-id="4b73b-216">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b73b-216">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b73b-217">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b73b-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b73b-218">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b73b-218">Request</span></span>
<span data-ttu-id="4b73b-219">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b73b-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1123

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="4b73b-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b73b-220">Response</span></span>
<span data-ttu-id="4b73b-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b73b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1289

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





