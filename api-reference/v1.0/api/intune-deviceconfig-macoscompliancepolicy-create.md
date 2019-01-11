---
title: macOSCompliancePolicy erstellen
description: Erstellen eines neuen macOSCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b489aaabca59513e6f14baf52bbfb0e046ac223d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811424"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="287a2-103">macOSCompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="287a2-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="287a2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="287a2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="287a2-105">Erstellen eines neuen [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="287a2-105">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="287a2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="287a2-106">Prerequisites</span></span>
<span data-ttu-id="287a2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="287a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="287a2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="287a2-109">Permission type</span></span>|<span data-ttu-id="287a2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="287a2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="287a2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="287a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="287a2-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="287a2-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="287a2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="287a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="287a2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="287a2-114">Not supported.</span></span>|
|<span data-ttu-id="287a2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="287a2-115">Application</span></span>|<span data-ttu-id="287a2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="287a2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="287a2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="287a2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="287a2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="287a2-118">Request headers</span></span>
|<span data-ttu-id="287a2-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="287a2-119">Header</span></span>|<span data-ttu-id="287a2-120">Wert</span><span class="sxs-lookup"><span data-stu-id="287a2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="287a2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="287a2-121">Authorization</span></span>|<span data-ttu-id="287a2-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="287a2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="287a2-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="287a2-123">Accept</span></span>|<span data-ttu-id="287a2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="287a2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="287a2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="287a2-125">Request body</span></span>
<span data-ttu-id="287a2-126">Geben Sie im Anforderungstext eine JSON-Darstellung des macOSCompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="287a2-126">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="287a2-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der macOSCompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="287a2-127">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="287a2-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="287a2-128">Property</span></span>|<span data-ttu-id="287a2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="287a2-129">Type</span></span>|<span data-ttu-id="287a2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="287a2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="287a2-131">id</span><span class="sxs-lookup"><span data-stu-id="287a2-131">id</span></span>|<span data-ttu-id="287a2-132">String</span><span class="sxs-lookup"><span data-stu-id="287a2-132">String</span></span>|<span data-ttu-id="287a2-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="287a2-133">Key of the entity.</span></span> <span data-ttu-id="287a2-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="287a2-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="287a2-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="287a2-135">createdDateTime</span></span>|<span data-ttu-id="287a2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="287a2-136">DateTimeOffset</span></span>|<span data-ttu-id="287a2-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="287a2-137">DateTime the object was created.</span></span> <span data-ttu-id="287a2-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="287a2-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="287a2-139">description</span><span class="sxs-lookup"><span data-stu-id="287a2-139">description</span></span>|<span data-ttu-id="287a2-140">String</span><span class="sxs-lookup"><span data-stu-id="287a2-140">String</span></span>|<span data-ttu-id="287a2-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="287a2-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="287a2-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="287a2-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="287a2-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="287a2-143">lastModifiedDateTime</span></span>|<span data-ttu-id="287a2-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="287a2-144">DateTimeOffset</span></span>|<span data-ttu-id="287a2-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="287a2-145">DateTime the object was last modified.</span></span> <span data-ttu-id="287a2-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="287a2-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="287a2-147">displayName</span><span class="sxs-lookup"><span data-stu-id="287a2-147">displayName</span></span>|<span data-ttu-id="287a2-148">String</span><span class="sxs-lookup"><span data-stu-id="287a2-148">String</span></span>|<span data-ttu-id="287a2-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="287a2-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="287a2-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="287a2-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="287a2-151">Version</span><span class="sxs-lookup"><span data-stu-id="287a2-151">version</span></span>|<span data-ttu-id="287a2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="287a2-152">Int32</span></span>|<span data-ttu-id="287a2-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="287a2-153">Version of the device configuration.</span></span> <span data-ttu-id="287a2-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="287a2-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="287a2-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="287a2-155">passwordRequired</span></span>|<span data-ttu-id="287a2-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="287a2-156">Boolean</span></span>|<span data-ttu-id="287a2-157">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="287a2-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="287a2-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="287a2-158">passwordBlockSimple</span></span>|<span data-ttu-id="287a2-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="287a2-159">Boolean</span></span>|<span data-ttu-id="287a2-160">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="287a2-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="287a2-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="287a2-161">passwordExpirationDays</span></span>|<span data-ttu-id="287a2-162">Int32</span><span class="sxs-lookup"><span data-stu-id="287a2-162">Int32</span></span>|<span data-ttu-id="287a2-163">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="287a2-163">Number of days before the password expires.</span></span> <span data-ttu-id="287a2-164">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="287a2-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="287a2-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="287a2-165">passwordMinimumLength</span></span>|<span data-ttu-id="287a2-166">Int32</span><span class="sxs-lookup"><span data-stu-id="287a2-166">Int32</span></span>|<span data-ttu-id="287a2-167">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="287a2-167">Minimum length of password.</span></span> <span data-ttu-id="287a2-168">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="287a2-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="287a2-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="287a2-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="287a2-170">Int32</span><span class="sxs-lookup"><span data-stu-id="287a2-170">Int32</span></span>|<span data-ttu-id="287a2-171">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="287a2-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="287a2-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="287a2-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="287a2-173">Int32</span><span class="sxs-lookup"><span data-stu-id="287a2-173">Int32</span></span>|<span data-ttu-id="287a2-174">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="287a2-174">Number of previous passwords to block.</span></span> <span data-ttu-id="287a2-175">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="287a2-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="287a2-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="287a2-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="287a2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="287a2-177">Int32</span></span>|<span data-ttu-id="287a2-178">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="287a2-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="287a2-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="287a2-179">passwordRequiredType</span></span>|[<span data-ttu-id="287a2-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="287a2-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="287a2-181">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="287a2-181">The required password type.</span></span> <span data-ttu-id="287a2-182">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="287a2-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="287a2-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="287a2-183">osMinimumVersion</span></span>|<span data-ttu-id="287a2-184">String</span><span class="sxs-lookup"><span data-stu-id="287a2-184">String</span></span>|<span data-ttu-id="287a2-185">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="287a2-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="287a2-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="287a2-186">osMaximumVersion</span></span>|<span data-ttu-id="287a2-187">String</span><span class="sxs-lookup"><span data-stu-id="287a2-187">String</span></span>|<span data-ttu-id="287a2-188">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="287a2-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="287a2-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="287a2-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="287a2-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="287a2-190">Boolean</span></span>|<span data-ttu-id="287a2-191">Gibt an, ob auf Geräten der Systemintegritätsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="287a2-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="287a2-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="287a2-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="287a2-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="287a2-193">Boolean</span></span>|<span data-ttu-id="287a2-194">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="287a2-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="287a2-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="287a2-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="287a2-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="287a2-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="287a2-197">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="287a2-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="287a2-198">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="287a2-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="287a2-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="287a2-199">storageRequireEncryption</span></span>|<span data-ttu-id="287a2-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="287a2-200">Boolean</span></span>|<span data-ttu-id="287a2-201">Gibt an, ob auf Mac OS-Geräten die Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="287a2-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="287a2-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="287a2-202">firewallEnabled</span></span>|<span data-ttu-id="287a2-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="287a2-203">Boolean</span></span>|<span data-ttu-id="287a2-204">Gibt an, ob die Firewall oder nicht aktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="287a2-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="287a2-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="287a2-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="287a2-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="287a2-206">Boolean</span></span>|<span data-ttu-id="287a2-207">Entspricht der Option "Alle eingehende Verbindungen blockieren".</span><span class="sxs-lookup"><span data-stu-id="287a2-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="287a2-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="287a2-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="287a2-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="287a2-209">Boolean</span></span>|<span data-ttu-id="287a2-210">Entspricht "Enable Tarnmodus."</span><span class="sxs-lookup"><span data-stu-id="287a2-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="287a2-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="287a2-211">Response</span></span>
<span data-ttu-id="287a2-212">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="287a2-212">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="287a2-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="287a2-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="287a2-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="287a2-214">Request</span></span>
<span data-ttu-id="287a2-215">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="287a2-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="287a2-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="287a2-216">Response</span></span>
<span data-ttu-id="287a2-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="287a2-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



