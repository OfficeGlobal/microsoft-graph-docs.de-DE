---
title: macOSCompliancePolicy aktualisieren
description: Aktualisieren der Eigenschaften eines macOSCompliancePolicy-Objekts.
author: tfitzmac
ms.openlocfilehash: 412e77f3c0c62f61ce0ab687861dd3cac4931c59
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348378"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="aa72b-103">macOSCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="aa72b-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="aa72b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aa72b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa72b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aa72b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa72b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aa72b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa72b-107">Aktualisieren der Eigenschaften eines [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa72b-107">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aa72b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="aa72b-108">Prerequisites</span></span>
<span data-ttu-id="aa72b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa72b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa72b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aa72b-111">Permission type</span></span>|<span data-ttu-id="aa72b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aa72b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa72b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aa72b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa72b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa72b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aa72b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aa72b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa72b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa72b-116">Not supported.</span></span>|
|<span data-ttu-id="aa72b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aa72b-117">Application</span></span>|<span data-ttu-id="aa72b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa72b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa72b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa72b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="aa72b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aa72b-120">Request headers</span></span>
|<span data-ttu-id="aa72b-121">Header</span><span class="sxs-lookup"><span data-stu-id="aa72b-121">Header</span></span>|<span data-ttu-id="aa72b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="aa72b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa72b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="aa72b-123">Authorization</span></span>|<span data-ttu-id="aa72b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="aa72b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa72b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aa72b-125">Accept</span></span>|<span data-ttu-id="aa72b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa72b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa72b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aa72b-127">Request body</span></span>
<span data-ttu-id="aa72b-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="aa72b-128">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="aa72b-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="aa72b-129">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="aa72b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aa72b-130">Property</span></span>|<span data-ttu-id="aa72b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="aa72b-131">Type</span></span>|<span data-ttu-id="aa72b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa72b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa72b-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aa72b-133">roleScopeTagIds</span></span>|<span data-ttu-id="aa72b-134">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="aa72b-134">String collection</span></span>|<span data-ttu-id="aa72b-135">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="aa72b-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aa72b-136">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aa72b-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa72b-137">id</span><span class="sxs-lookup"><span data-stu-id="aa72b-137">id</span></span>|<span data-ttu-id="aa72b-138">String</span><span class="sxs-lookup"><span data-stu-id="aa72b-138">String</span></span>|<span data-ttu-id="aa72b-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="aa72b-139">Key of the entity.</span></span> <span data-ttu-id="aa72b-140">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aa72b-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa72b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa72b-141">createdDateTime</span></span>|<span data-ttu-id="aa72b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa72b-142">DateTimeOffset</span></span>|<span data-ttu-id="aa72b-143">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa72b-143">DateTime the object was created.</span></span> <span data-ttu-id="aa72b-144">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aa72b-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa72b-145">description</span><span class="sxs-lookup"><span data-stu-id="aa72b-145">description</span></span>|<span data-ttu-id="aa72b-146">String</span><span class="sxs-lookup"><span data-stu-id="aa72b-146">String</span></span>|<span data-ttu-id="aa72b-147">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="aa72b-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aa72b-148">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aa72b-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa72b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa72b-149">lastModifiedDateTime</span></span>|<span data-ttu-id="aa72b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa72b-150">DateTimeOffset</span></span>|<span data-ttu-id="aa72b-151">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa72b-151">DateTime the object was last modified.</span></span> <span data-ttu-id="aa72b-152">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aa72b-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa72b-153">displayName</span><span class="sxs-lookup"><span data-stu-id="aa72b-153">displayName</span></span>|<span data-ttu-id="aa72b-154">String</span><span class="sxs-lookup"><span data-stu-id="aa72b-154">String</span></span>|<span data-ttu-id="aa72b-155">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="aa72b-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aa72b-156">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aa72b-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa72b-157">Version</span><span class="sxs-lookup"><span data-stu-id="aa72b-157">version</span></span>|<span data-ttu-id="aa72b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="aa72b-158">Int32</span></span>|<span data-ttu-id="aa72b-159">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="aa72b-159">Version of the device configuration.</span></span> <span data-ttu-id="aa72b-160">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aa72b-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa72b-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="aa72b-161">passwordRequired</span></span>|<span data-ttu-id="aa72b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa72b-162">Boolean</span></span>|<span data-ttu-id="aa72b-163">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="aa72b-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="aa72b-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="aa72b-164">passwordBlockSimple</span></span>|<span data-ttu-id="aa72b-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa72b-165">Boolean</span></span>|<span data-ttu-id="aa72b-166">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="aa72b-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="aa72b-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="aa72b-167">passwordExpirationDays</span></span>|<span data-ttu-id="aa72b-168">Int32</span><span class="sxs-lookup"><span data-stu-id="aa72b-168">Int32</span></span>|<span data-ttu-id="aa72b-169">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="aa72b-169">Number of days before the password expires.</span></span> <span data-ttu-id="aa72b-170">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="aa72b-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="aa72b-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="aa72b-171">passwordMinimumLength</span></span>|<span data-ttu-id="aa72b-172">Int32</span><span class="sxs-lookup"><span data-stu-id="aa72b-172">Int32</span></span>|<span data-ttu-id="aa72b-173">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="aa72b-173">Minimum length of password.</span></span> <span data-ttu-id="aa72b-174">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="aa72b-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="aa72b-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="aa72b-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="aa72b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="aa72b-176">Int32</span></span>|<span data-ttu-id="aa72b-177">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="aa72b-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="aa72b-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="aa72b-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="aa72b-179">Int32</span><span class="sxs-lookup"><span data-stu-id="aa72b-179">Int32</span></span>|<span data-ttu-id="aa72b-180">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="aa72b-180">Number of previous passwords to block.</span></span> <span data-ttu-id="aa72b-181">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="aa72b-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="aa72b-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="aa72b-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="aa72b-183">Int32</span><span class="sxs-lookup"><span data-stu-id="aa72b-183">Int32</span></span>|<span data-ttu-id="aa72b-184">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="aa72b-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="aa72b-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="aa72b-185">passwordRequiredType</span></span>|[<span data-ttu-id="aa72b-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="aa72b-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="aa72b-187">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="aa72b-187">The required password type.</span></span> <span data-ttu-id="aa72b-188">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="aa72b-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="aa72b-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="aa72b-189">osMinimumVersion</span></span>|<span data-ttu-id="aa72b-190">String</span><span class="sxs-lookup"><span data-stu-id="aa72b-190">String</span></span>|<span data-ttu-id="aa72b-191">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="aa72b-191">Minimum IOS version.</span></span>|
|<span data-ttu-id="aa72b-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="aa72b-192">osMaximumVersion</span></span>|<span data-ttu-id="aa72b-193">String</span><span class="sxs-lookup"><span data-stu-id="aa72b-193">String</span></span>|<span data-ttu-id="aa72b-194">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="aa72b-194">Maximum IOS version.</span></span>|
|<span data-ttu-id="aa72b-195">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="aa72b-195">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="aa72b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa72b-196">Boolean</span></span>|<span data-ttu-id="aa72b-197">Gibt an, ob auf Geräten der Systemintegritätsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="aa72b-197">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="aa72b-198">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="aa72b-198">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="aa72b-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="aa72b-199">Boolean</span></span>|<span data-ttu-id="aa72b-200">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="aa72b-200">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="aa72b-201">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="aa72b-201">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="aa72b-202">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="aa72b-202">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="aa72b-203">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="aa72b-203">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="aa72b-204">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="aa72b-204">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="aa72b-205">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="aa72b-205">storageRequireEncryption</span></span>|<span data-ttu-id="aa72b-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa72b-206">Boolean</span></span>|<span data-ttu-id="aa72b-207">Gibt an, ob auf Mac OS-Geräten die Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="aa72b-207">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="aa72b-208">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="aa72b-208">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="aa72b-209">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="aa72b-209">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="aa72b-210">System und den Datenschutz, der bestimmt, welche Download Speicherorte apps auf einem Mac OS-Gerät aus ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="aa72b-210">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="aa72b-211">Mögliche Werte: sind `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers` und `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="aa72b-211">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="aa72b-212">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="aa72b-212">firewallEnabled</span></span>|<span data-ttu-id="aa72b-213">Boolesch</span><span class="sxs-lookup"><span data-stu-id="aa72b-213">Boolean</span></span>|<span data-ttu-id="aa72b-214">Gibt an, ob die Firewall oder nicht aktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="aa72b-214">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="aa72b-215">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="aa72b-215">firewallBlockAllIncoming</span></span>|<span data-ttu-id="aa72b-216">Boolesch</span><span class="sxs-lookup"><span data-stu-id="aa72b-216">Boolean</span></span>|<span data-ttu-id="aa72b-217">Entspricht der Option "Alle eingehende Verbindungen blockieren".</span><span class="sxs-lookup"><span data-stu-id="aa72b-217">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="aa72b-218">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="aa72b-218">firewallEnableStealthMode</span></span>|<span data-ttu-id="aa72b-219">Boolesch</span><span class="sxs-lookup"><span data-stu-id="aa72b-219">Boolean</span></span>|<span data-ttu-id="aa72b-220">Entspricht "Enable Tarnmodus."</span><span class="sxs-lookup"><span data-stu-id="aa72b-220">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="aa72b-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa72b-221">Response</span></span>
<span data-ttu-id="aa72b-222">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="aa72b-222">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa72b-223">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa72b-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa72b-224">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa72b-224">Request</span></span>
<span data-ttu-id="aa72b-225">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa72b-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 963

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
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
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

### <a name="response"></a><span data-ttu-id="aa72b-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa72b-226">Response</span></span>
<span data-ttu-id="aa72b-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa72b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1131

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





