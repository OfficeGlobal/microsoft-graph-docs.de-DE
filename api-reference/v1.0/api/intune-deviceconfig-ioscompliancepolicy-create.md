---
title: iosCompliancePolicy erstellen
description: Erstellen eines neuen iosCompliancePolicy-Objekts.
author: tfitzmac
ms.openlocfilehash: fd039005455c94cf55fa1afe21eee33fde9b4588
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346172"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="6d947-103">iosCompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="6d947-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="6d947-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6d947-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d947-105">Erstellen eines neuen [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6d947-105">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6d947-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6d947-106">Prerequisites</span></span>
<span data-ttu-id="6d947-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d947-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d947-109">Permission type</span></span>|<span data-ttu-id="6d947-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d947-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d947-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d947-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d947-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d947-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d947-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d947-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d947-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d947-114">Not supported.</span></span>|
|<span data-ttu-id="6d947-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6d947-115">Application</span></span>|<span data-ttu-id="6d947-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d947-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d947-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d947-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6d947-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d947-118">Request headers</span></span>
|<span data-ttu-id="6d947-119">Header</span><span class="sxs-lookup"><span data-stu-id="6d947-119">Header</span></span>|<span data-ttu-id="6d947-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6d947-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d947-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6d947-121">Authorization</span></span>|<span data-ttu-id="6d947-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6d947-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d947-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6d947-123">Accept</span></span>|<span data-ttu-id="6d947-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6d947-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d947-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6d947-125">Request body</span></span>
<span data-ttu-id="6d947-126">Geben Sie im Anforderungstext eine JSON-Darstellung des iosCompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="6d947-126">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="6d947-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosCompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6d947-127">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="6d947-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d947-128">Property</span></span>|<span data-ttu-id="6d947-129">Typ</span><span class="sxs-lookup"><span data-stu-id="6d947-129">Type</span></span>|<span data-ttu-id="6d947-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d947-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d947-131">id</span><span class="sxs-lookup"><span data-stu-id="6d947-131">id</span></span>|<span data-ttu-id="6d947-132">String</span><span class="sxs-lookup"><span data-stu-id="6d947-132">String</span></span>|<span data-ttu-id="6d947-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6d947-133">Key of the entity.</span></span> <span data-ttu-id="6d947-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6d947-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6d947-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d947-135">createdDateTime</span></span>|<span data-ttu-id="6d947-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d947-136">DateTimeOffset</span></span>|<span data-ttu-id="6d947-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6d947-137">DateTime the object was created.</span></span> <span data-ttu-id="6d947-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6d947-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6d947-139">description</span><span class="sxs-lookup"><span data-stu-id="6d947-139">description</span></span>|<span data-ttu-id="6d947-140">String</span><span class="sxs-lookup"><span data-stu-id="6d947-140">String</span></span>|<span data-ttu-id="6d947-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6d947-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6d947-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6d947-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6d947-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d947-143">lastModifiedDateTime</span></span>|<span data-ttu-id="6d947-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d947-144">DateTimeOffset</span></span>|<span data-ttu-id="6d947-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6d947-145">DateTime the object was last modified.</span></span> <span data-ttu-id="6d947-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6d947-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6d947-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6d947-147">displayName</span></span>|<span data-ttu-id="6d947-148">String</span><span class="sxs-lookup"><span data-stu-id="6d947-148">String</span></span>|<span data-ttu-id="6d947-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6d947-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6d947-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6d947-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6d947-151">Version</span><span class="sxs-lookup"><span data-stu-id="6d947-151">version</span></span>|<span data-ttu-id="6d947-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6d947-152">Int32</span></span>|<span data-ttu-id="6d947-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6d947-153">Version of the device configuration.</span></span> <span data-ttu-id="6d947-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6d947-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6d947-155">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6d947-155">passcodeBlockSimple</span></span>|<span data-ttu-id="6d947-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6d947-156">Boolean</span></span>|<span data-ttu-id="6d947-157">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="6d947-157">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="6d947-158">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6d947-158">passcodeExpirationDays</span></span>|<span data-ttu-id="6d947-159">Int32</span><span class="sxs-lookup"><span data-stu-id="6d947-159">Int32</span></span>|<span data-ttu-id="6d947-160">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="6d947-160">Number of days before the passcode expires.</span></span> <span data-ttu-id="6d947-161">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="6d947-161">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6d947-162">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6d947-162">passcodeMinimumLength</span></span>|<span data-ttu-id="6d947-163">Int32</span><span class="sxs-lookup"><span data-stu-id="6d947-163">Int32</span></span>|<span data-ttu-id="6d947-164">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="6d947-164">Minimum length of passcode.</span></span> <span data-ttu-id="6d947-165">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="6d947-165">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6d947-166">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6d947-166">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6d947-167">Int32</span><span class="sxs-lookup"><span data-stu-id="6d947-167">Int32</span></span>|<span data-ttu-id="6d947-168">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="6d947-168">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="6d947-169">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="6d947-169">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="6d947-170">Int32</span><span class="sxs-lookup"><span data-stu-id="6d947-170">Int32</span></span>|<span data-ttu-id="6d947-171">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="6d947-171">Number of previous passcodes to block.</span></span> <span data-ttu-id="6d947-172">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="6d947-172">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6d947-173">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6d947-173">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="6d947-174">Int32</span><span class="sxs-lookup"><span data-stu-id="6d947-174">Int32</span></span>|<span data-ttu-id="6d947-175">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="6d947-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6d947-176">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="6d947-176">passcodeRequiredType</span></span>|[<span data-ttu-id="6d947-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6d947-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6d947-178">Der erforderliche Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="6d947-178">The required passcode type.</span></span> <span data-ttu-id="6d947-179">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6d947-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6d947-180">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="6d947-180">passcodeRequired</span></span>|<span data-ttu-id="6d947-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6d947-181">Boolean</span></span>|<span data-ttu-id="6d947-182">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="6d947-182">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="6d947-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6d947-183">osMinimumVersion</span></span>|<span data-ttu-id="6d947-184">String</span><span class="sxs-lookup"><span data-stu-id="6d947-184">String</span></span>|<span data-ttu-id="6d947-185">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="6d947-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="6d947-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6d947-186">osMaximumVersion</span></span>|<span data-ttu-id="6d947-187">String</span><span class="sxs-lookup"><span data-stu-id="6d947-187">String</span></span>|<span data-ttu-id="6d947-188">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="6d947-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="6d947-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="6d947-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="6d947-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6d947-190">Boolean</span></span>|<span data-ttu-id="6d947-191">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="6d947-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="6d947-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6d947-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6d947-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6d947-193">Boolean</span></span>|<span data-ttu-id="6d947-194">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="6d947-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="6d947-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6d947-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6d947-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="6d947-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6d947-197">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="6d947-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6d947-198">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6d947-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6d947-199">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="6d947-199">managedEmailProfileRequired</span></span>|<span data-ttu-id="6d947-200">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6d947-200">Boolean</span></span>|<span data-ttu-id="6d947-201">Gibt an, ob ein verwaltetes E-Mail-Profil erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="6d947-201">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="6d947-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d947-202">Response</span></span>
<span data-ttu-id="6d947-203">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d947-203">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d947-204">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6d947-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="6d947-205">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d947-205">Request</span></span>
<span data-ttu-id="6d947-206">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6d947-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 745

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```

### <a name="response"></a><span data-ttu-id="6d947-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d947-207">Response</span></span>
<span data-ttu-id="6d947-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d947-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
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
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```



