---
title: macOSCompliancePolicy aktualisieren
description: Aktualisieren der Eigenschaften eines macOSCompliancePolicy-Objekts.
ms.openlocfilehash: 99b4586ee0651a34630b25719425290cf700fef3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016919"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="1353e-103">macOSCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1353e-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="1353e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1353e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1353e-105">Aktualisieren der Eigenschaften eines [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1353e-105">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1353e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1353e-106">Prerequisites</span></span>
<span data-ttu-id="1353e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1353e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1353e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1353e-109">Permission type</span></span>|<span data-ttu-id="1353e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1353e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1353e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1353e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1353e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1353e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1353e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1353e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1353e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1353e-114">Not supported.</span></span>|
|<span data-ttu-id="1353e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1353e-115">Application</span></span>|<span data-ttu-id="1353e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1353e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1353e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1353e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="1353e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1353e-118">Request headers</span></span>
|<span data-ttu-id="1353e-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1353e-119">Header</span></span>|<span data-ttu-id="1353e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1353e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1353e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1353e-121">Authorization</span></span>|<span data-ttu-id="1353e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1353e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1353e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1353e-123">Accept</span></span>|<span data-ttu-id="1353e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1353e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1353e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1353e-125">Request body</span></span>
<span data-ttu-id="1353e-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1353e-126">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="1353e-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1353e-127">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="1353e-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1353e-128">Property</span></span>|<span data-ttu-id="1353e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="1353e-129">Type</span></span>|<span data-ttu-id="1353e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1353e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1353e-131">id</span><span class="sxs-lookup"><span data-stu-id="1353e-131">id</span></span>|<span data-ttu-id="1353e-132">String</span><span class="sxs-lookup"><span data-stu-id="1353e-132">String</span></span>|<span data-ttu-id="1353e-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1353e-133">Key of the entity.</span></span> <span data-ttu-id="1353e-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1353e-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1353e-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1353e-135">createdDateTime</span></span>|<span data-ttu-id="1353e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1353e-136">DateTimeOffset</span></span>|<span data-ttu-id="1353e-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1353e-137">DateTime the object was created.</span></span> <span data-ttu-id="1353e-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1353e-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1353e-139">description</span><span class="sxs-lookup"><span data-stu-id="1353e-139">description</span></span>|<span data-ttu-id="1353e-140">String</span><span class="sxs-lookup"><span data-stu-id="1353e-140">String</span></span>|<span data-ttu-id="1353e-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1353e-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1353e-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1353e-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1353e-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1353e-143">lastModifiedDateTime</span></span>|<span data-ttu-id="1353e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1353e-144">DateTimeOffset</span></span>|<span data-ttu-id="1353e-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1353e-145">DateTime the object was last modified.</span></span> <span data-ttu-id="1353e-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1353e-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1353e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="1353e-147">displayName</span></span>|<span data-ttu-id="1353e-148">String</span><span class="sxs-lookup"><span data-stu-id="1353e-148">String</span></span>|<span data-ttu-id="1353e-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1353e-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1353e-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1353e-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1353e-151">Version</span><span class="sxs-lookup"><span data-stu-id="1353e-151">version</span></span>|<span data-ttu-id="1353e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1353e-152">Int32</span></span>|<span data-ttu-id="1353e-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="1353e-153">Version of the device configuration.</span></span> <span data-ttu-id="1353e-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1353e-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1353e-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="1353e-155">passwordRequired</span></span>|<span data-ttu-id="1353e-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="1353e-156">Boolean</span></span>|<span data-ttu-id="1353e-157">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="1353e-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="1353e-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="1353e-158">passwordBlockSimple</span></span>|<span data-ttu-id="1353e-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="1353e-159">Boolean</span></span>|<span data-ttu-id="1353e-160">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="1353e-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="1353e-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1353e-161">passwordExpirationDays</span></span>|<span data-ttu-id="1353e-162">Int32</span><span class="sxs-lookup"><span data-stu-id="1353e-162">Int32</span></span>|<span data-ttu-id="1353e-163">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="1353e-163">Number of days before the password expires.</span></span> <span data-ttu-id="1353e-164">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="1353e-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="1353e-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1353e-165">passwordMinimumLength</span></span>|<span data-ttu-id="1353e-166">Int32</span><span class="sxs-lookup"><span data-stu-id="1353e-166">Int32</span></span>|<span data-ttu-id="1353e-167">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="1353e-167">Minimum length of password.</span></span> <span data-ttu-id="1353e-168">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="1353e-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="1353e-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1353e-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1353e-170">Int32</span><span class="sxs-lookup"><span data-stu-id="1353e-170">Int32</span></span>|<span data-ttu-id="1353e-171">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="1353e-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="1353e-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1353e-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1353e-173">Int32</span><span class="sxs-lookup"><span data-stu-id="1353e-173">Int32</span></span>|<span data-ttu-id="1353e-174">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="1353e-174">Number of previous passwords to block.</span></span> <span data-ttu-id="1353e-175">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="1353e-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="1353e-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="1353e-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="1353e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1353e-177">Int32</span></span>|<span data-ttu-id="1353e-178">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="1353e-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="1353e-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1353e-179">passwordRequiredType</span></span>|[<span data-ttu-id="1353e-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1353e-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="1353e-181">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="1353e-181">The required password type.</span></span> <span data-ttu-id="1353e-182">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="1353e-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="1353e-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="1353e-183">osMinimumVersion</span></span>|<span data-ttu-id="1353e-184">String</span><span class="sxs-lookup"><span data-stu-id="1353e-184">String</span></span>|<span data-ttu-id="1353e-185">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="1353e-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="1353e-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="1353e-186">osMaximumVersion</span></span>|<span data-ttu-id="1353e-187">String</span><span class="sxs-lookup"><span data-stu-id="1353e-187">String</span></span>|<span data-ttu-id="1353e-188">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="1353e-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="1353e-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="1353e-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="1353e-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="1353e-190">Boolean</span></span>|<span data-ttu-id="1353e-191">Gibt an, ob auf Geräten der Systemintegritätsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="1353e-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="1353e-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="1353e-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="1353e-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1353e-193">Boolean</span></span>|<span data-ttu-id="1353e-194">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="1353e-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="1353e-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="1353e-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="1353e-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="1353e-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="1353e-197">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="1353e-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="1353e-198">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="1353e-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="1353e-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="1353e-199">storageRequireEncryption</span></span>|<span data-ttu-id="1353e-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="1353e-200">Boolean</span></span>|<span data-ttu-id="1353e-201">Gibt an, ob auf Mac OS-Geräten die Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="1353e-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="1353e-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="1353e-202">firewallEnabled</span></span>|<span data-ttu-id="1353e-203">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1353e-203">Boolean</span></span>|<span data-ttu-id="1353e-204">Gibt an, ob die Firewall oder nicht aktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="1353e-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="1353e-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="1353e-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="1353e-206">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1353e-206">Boolean</span></span>|<span data-ttu-id="1353e-207">Entspricht der Option "Alle eingehende Verbindungen blockieren".</span><span class="sxs-lookup"><span data-stu-id="1353e-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="1353e-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="1353e-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="1353e-209">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1353e-209">Boolean</span></span>|<span data-ttu-id="1353e-210">Entspricht "Enable Tarnmodus."</span><span class="sxs-lookup"><span data-stu-id="1353e-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="1353e-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="1353e-211">Response</span></span>
<span data-ttu-id="1353e-212">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1353e-212">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1353e-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1353e-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="1353e-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1353e-214">Request</span></span>
<span data-ttu-id="1353e-215">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1353e-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 849

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
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
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="1353e-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="1353e-216">Response</span></span>
<span data-ttu-id="1353e-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1353e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1021

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
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
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```



