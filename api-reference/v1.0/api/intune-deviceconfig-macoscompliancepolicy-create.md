---
title: macOSCompliancePolicy erstellen
description: Erstellen eines neuen macOSCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 113642efee7673c0d211a2f9cc5fe7c05d37607b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987881"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="0ef46-103">macOSCompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="0ef46-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="0ef46-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0ef46-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ef46-105">Erstellen eines neuen [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0ef46-105">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ef46-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0ef46-106">Prerequisites</span></span>
<span data-ttu-id="0ef46-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ef46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ef46-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0ef46-109">Permission type</span></span>|<span data-ttu-id="0ef46-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0ef46-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ef46-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0ef46-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0ef46-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ef46-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ef46-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0ef46-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ef46-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ef46-114">Not supported.</span></span>|
|<span data-ttu-id="0ef46-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0ef46-115">Application</span></span>|<span data-ttu-id="0ef46-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ef46-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ef46-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ef46-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0ef46-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0ef46-118">Request headers</span></span>
|<span data-ttu-id="0ef46-119">Header</span><span class="sxs-lookup"><span data-stu-id="0ef46-119">Header</span></span>|<span data-ttu-id="0ef46-120">Wert</span><span class="sxs-lookup"><span data-stu-id="0ef46-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ef46-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ef46-121">Authorization</span></span>|<span data-ttu-id="0ef46-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0ef46-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ef46-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0ef46-123">Accept</span></span>|<span data-ttu-id="0ef46-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0ef46-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ef46-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0ef46-125">Request body</span></span>
<span data-ttu-id="0ef46-126">Geben Sie im Anforderungstext eine JSON-Darstellung des macOSCompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0ef46-126">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="0ef46-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der macOSCompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0ef46-127">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="0ef46-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0ef46-128">Property</span></span>|<span data-ttu-id="0ef46-129">Typ</span><span class="sxs-lookup"><span data-stu-id="0ef46-129">Type</span></span>|<span data-ttu-id="0ef46-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ef46-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ef46-131">id</span><span class="sxs-lookup"><span data-stu-id="0ef46-131">id</span></span>|<span data-ttu-id="0ef46-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ef46-132">String</span></span>|<span data-ttu-id="0ef46-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0ef46-133">Key of the entity.</span></span> <span data-ttu-id="0ef46-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ef46-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0ef46-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ef46-135">createdDateTime</span></span>|<span data-ttu-id="0ef46-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ef46-136">DateTimeOffset</span></span>|<span data-ttu-id="0ef46-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0ef46-137">DateTime the object was created.</span></span> <span data-ttu-id="0ef46-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ef46-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0ef46-139">description</span><span class="sxs-lookup"><span data-stu-id="0ef46-139">description</span></span>|<span data-ttu-id="0ef46-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ef46-140">String</span></span>|<span data-ttu-id="0ef46-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0ef46-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ef46-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ef46-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0ef46-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ef46-143">lastModifiedDateTime</span></span>|<span data-ttu-id="0ef46-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ef46-144">DateTimeOffset</span></span>|<span data-ttu-id="0ef46-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0ef46-145">DateTime the object was last modified.</span></span> <span data-ttu-id="0ef46-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ef46-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0ef46-147">displayName</span><span class="sxs-lookup"><span data-stu-id="0ef46-147">displayName</span></span>|<span data-ttu-id="0ef46-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ef46-148">String</span></span>|<span data-ttu-id="0ef46-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0ef46-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ef46-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ef46-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0ef46-151">Version</span><span class="sxs-lookup"><span data-stu-id="0ef46-151">version</span></span>|<span data-ttu-id="0ef46-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0ef46-152">Int32</span></span>|<span data-ttu-id="0ef46-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0ef46-153">Version of the device configuration.</span></span> <span data-ttu-id="0ef46-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ef46-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0ef46-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0ef46-155">passwordRequired</span></span>|<span data-ttu-id="0ef46-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ef46-156">Boolean</span></span>|<span data-ttu-id="0ef46-157">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="0ef46-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="0ef46-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0ef46-158">passwordBlockSimple</span></span>|<span data-ttu-id="0ef46-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ef46-159">Boolean</span></span>|<span data-ttu-id="0ef46-160">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="0ef46-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="0ef46-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0ef46-161">passwordExpirationDays</span></span>|<span data-ttu-id="0ef46-162">Int32</span><span class="sxs-lookup"><span data-stu-id="0ef46-162">Int32</span></span>|<span data-ttu-id="0ef46-163">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="0ef46-163">Number of days before the password expires.</span></span> <span data-ttu-id="0ef46-164">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="0ef46-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="0ef46-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0ef46-165">passwordMinimumLength</span></span>|<span data-ttu-id="0ef46-166">Int32</span><span class="sxs-lookup"><span data-stu-id="0ef46-166">Int32</span></span>|<span data-ttu-id="0ef46-167">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="0ef46-167">Minimum length of password.</span></span> <span data-ttu-id="0ef46-168">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="0ef46-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="0ef46-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0ef46-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0ef46-170">Int32</span><span class="sxs-lookup"><span data-stu-id="0ef46-170">Int32</span></span>|<span data-ttu-id="0ef46-171">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="0ef46-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0ef46-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0ef46-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0ef46-173">Int32</span><span class="sxs-lookup"><span data-stu-id="0ef46-173">Int32</span></span>|<span data-ttu-id="0ef46-174">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="0ef46-174">Number of previous passwords to block.</span></span> <span data-ttu-id="0ef46-175">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="0ef46-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="0ef46-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0ef46-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0ef46-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0ef46-177">Int32</span></span>|<span data-ttu-id="0ef46-178">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="0ef46-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0ef46-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0ef46-179">passwordRequiredType</span></span>|[<span data-ttu-id="0ef46-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0ef46-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0ef46-181">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="0ef46-181">The required password type.</span></span> <span data-ttu-id="0ef46-182">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="0ef46-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0ef46-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0ef46-183">osMinimumVersion</span></span>|<span data-ttu-id="0ef46-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ef46-184">String</span></span>|<span data-ttu-id="0ef46-185">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="0ef46-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="0ef46-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0ef46-186">osMaximumVersion</span></span>|<span data-ttu-id="0ef46-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ef46-187">String</span></span>|<span data-ttu-id="0ef46-188">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="0ef46-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="0ef46-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0ef46-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="0ef46-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ef46-190">Boolean</span></span>|<span data-ttu-id="0ef46-191">Gibt an, ob auf Geräten der Systemintegritätsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="0ef46-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="0ef46-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="0ef46-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="0ef46-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0ef46-193">Boolean</span></span>|<span data-ttu-id="0ef46-194">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="0ef46-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="0ef46-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="0ef46-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="0ef46-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="0ef46-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="0ef46-197">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="0ef46-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="0ef46-198">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="0ef46-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="0ef46-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0ef46-199">storageRequireEncryption</span></span>|<span data-ttu-id="0ef46-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ef46-200">Boolean</span></span>|<span data-ttu-id="0ef46-201">Gibt an, ob auf Mac OS-Geräten die Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="0ef46-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="0ef46-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="0ef46-202">firewallEnabled</span></span>|<span data-ttu-id="0ef46-203">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0ef46-203">Boolean</span></span>|<span data-ttu-id="0ef46-204">Gibt an, ob die Firewall oder nicht aktiviert werden soll.</span><span class="sxs-lookup"><span data-stu-id="0ef46-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="0ef46-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="0ef46-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="0ef46-206">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0ef46-206">Boolean</span></span>|<span data-ttu-id="0ef46-207">Entspricht der Option "Alle eingehende Verbindungen blockieren".</span><span class="sxs-lookup"><span data-stu-id="0ef46-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="0ef46-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="0ef46-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="0ef46-209">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0ef46-209">Boolean</span></span>|<span data-ttu-id="0ef46-210">Entspricht "Enable Tarnmodus."</span><span class="sxs-lookup"><span data-stu-id="0ef46-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="0ef46-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ef46-211">Response</span></span>
<span data-ttu-id="0ef46-212">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0ef46-212">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ef46-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0ef46-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ef46-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ef46-214">Request</span></span>
<span data-ttu-id="0ef46-215">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0ef46-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ef46-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ef46-216">Response</span></span>
<span data-ttu-id="0ef46-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ef46-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



