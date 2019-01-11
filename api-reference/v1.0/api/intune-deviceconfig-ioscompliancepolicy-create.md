---
title: iosCompliancePolicy erstellen
description: Erstellen eines neuen iosCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: df69e8512a1f8e900f1e3751d5943f4ea8e6a215
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834461"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="a1519-103">iosCompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="a1519-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="a1519-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a1519-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1519-105">Erstellen eines neuen [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a1519-105">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1519-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a1519-106">Prerequisites</span></span>
<span data-ttu-id="a1519-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1519-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1519-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a1519-109">Permission type</span></span>|<span data-ttu-id="a1519-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a1519-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1519-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a1519-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a1519-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1519-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1519-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a1519-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1519-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1519-114">Not supported.</span></span>|
|<span data-ttu-id="a1519-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a1519-115">Application</span></span>|<span data-ttu-id="a1519-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1519-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1519-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1519-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a1519-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a1519-118">Request headers</span></span>
|<span data-ttu-id="a1519-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a1519-119">Header</span></span>|<span data-ttu-id="a1519-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a1519-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1519-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1519-121">Authorization</span></span>|<span data-ttu-id="a1519-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a1519-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1519-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a1519-123">Accept</span></span>|<span data-ttu-id="a1519-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a1519-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1519-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a1519-125">Request body</span></span>
<span data-ttu-id="a1519-126">Geben Sie im Anforderungstext eine JSON-Darstellung des iosCompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a1519-126">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="a1519-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosCompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a1519-127">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="a1519-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a1519-128">Property</span></span>|<span data-ttu-id="a1519-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a1519-129">Type</span></span>|<span data-ttu-id="a1519-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1519-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1519-131">id</span><span class="sxs-lookup"><span data-stu-id="a1519-131">id</span></span>|<span data-ttu-id="a1519-132">String</span><span class="sxs-lookup"><span data-stu-id="a1519-132">String</span></span>|<span data-ttu-id="a1519-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a1519-133">Key of the entity.</span></span> <span data-ttu-id="a1519-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1519-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1519-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1519-135">createdDateTime</span></span>|<span data-ttu-id="a1519-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1519-136">DateTimeOffset</span></span>|<span data-ttu-id="a1519-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a1519-137">DateTime the object was created.</span></span> <span data-ttu-id="a1519-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1519-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1519-139">description</span><span class="sxs-lookup"><span data-stu-id="a1519-139">description</span></span>|<span data-ttu-id="a1519-140">String</span><span class="sxs-lookup"><span data-stu-id="a1519-140">String</span></span>|<span data-ttu-id="a1519-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a1519-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a1519-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1519-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1519-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1519-143">lastModifiedDateTime</span></span>|<span data-ttu-id="a1519-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1519-144">DateTimeOffset</span></span>|<span data-ttu-id="a1519-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a1519-145">DateTime the object was last modified.</span></span> <span data-ttu-id="a1519-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1519-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1519-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a1519-147">displayName</span></span>|<span data-ttu-id="a1519-148">String</span><span class="sxs-lookup"><span data-stu-id="a1519-148">String</span></span>|<span data-ttu-id="a1519-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a1519-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a1519-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1519-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1519-151">Version</span><span class="sxs-lookup"><span data-stu-id="a1519-151">version</span></span>|<span data-ttu-id="a1519-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a1519-152">Int32</span></span>|<span data-ttu-id="a1519-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a1519-153">Version of the device configuration.</span></span> <span data-ttu-id="a1519-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a1519-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a1519-155">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="a1519-155">passcodeBlockSimple</span></span>|<span data-ttu-id="a1519-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1519-156">Boolean</span></span>|<span data-ttu-id="a1519-157">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="a1519-157">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="a1519-158">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a1519-158">passcodeExpirationDays</span></span>|<span data-ttu-id="a1519-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a1519-159">Int32</span></span>|<span data-ttu-id="a1519-160">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="a1519-160">Number of days before the passcode expires.</span></span> <span data-ttu-id="a1519-161">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="a1519-161">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="a1519-162">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a1519-162">passcodeMinimumLength</span></span>|<span data-ttu-id="a1519-163">Int32</span><span class="sxs-lookup"><span data-stu-id="a1519-163">Int32</span></span>|<span data-ttu-id="a1519-164">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="a1519-164">Minimum length of passcode.</span></span> <span data-ttu-id="a1519-165">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="a1519-165">Valid values 4 to 14</span></span>|
|<span data-ttu-id="a1519-166">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a1519-166">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a1519-167">Int32</span><span class="sxs-lookup"><span data-stu-id="a1519-167">Int32</span></span>|<span data-ttu-id="a1519-168">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a1519-168">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="a1519-169">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="a1519-169">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="a1519-170">Int32</span><span class="sxs-lookup"><span data-stu-id="a1519-170">Int32</span></span>|<span data-ttu-id="a1519-171">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="a1519-171">Number of previous passcodes to block.</span></span> <span data-ttu-id="a1519-172">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="a1519-172">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a1519-173">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a1519-173">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="a1519-174">Int32</span><span class="sxs-lookup"><span data-stu-id="a1519-174">Int32</span></span>|<span data-ttu-id="a1519-175">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="a1519-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="a1519-176">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="a1519-176">passcodeRequiredType</span></span>|[<span data-ttu-id="a1519-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a1519-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="a1519-178">Der erforderliche Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="a1519-178">The required passcode type.</span></span> <span data-ttu-id="a1519-179">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="a1519-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a1519-180">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="a1519-180">passcodeRequired</span></span>|<span data-ttu-id="a1519-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1519-181">Boolean</span></span>|<span data-ttu-id="a1519-182">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a1519-182">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="a1519-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="a1519-183">osMinimumVersion</span></span>|<span data-ttu-id="a1519-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1519-184">String</span></span>|<span data-ttu-id="a1519-185">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="a1519-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="a1519-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="a1519-186">osMaximumVersion</span></span>|<span data-ttu-id="a1519-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1519-187">String</span></span>|<span data-ttu-id="a1519-188">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="a1519-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="a1519-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="a1519-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="a1519-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1519-190">Boolean</span></span>|<span data-ttu-id="a1519-191">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="a1519-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="a1519-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a1519-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="a1519-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a1519-193">Boolean</span></span>|<span data-ttu-id="a1519-194">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="a1519-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="a1519-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="a1519-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="a1519-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="a1519-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="a1519-197">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="a1519-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="a1519-198">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="a1519-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="a1519-199">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="a1519-199">managedEmailProfileRequired</span></span>|<span data-ttu-id="a1519-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1519-200">Boolean</span></span>|<span data-ttu-id="a1519-201">Gibt an, ob ein verwaltetes E-Mail-Profil erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="a1519-201">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="a1519-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1519-202">Response</span></span>
<span data-ttu-id="a1519-203">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1519-203">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1519-204">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1519-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1519-205">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1519-205">Request</span></span>
<span data-ttu-id="a1519-206">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a1519-206">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1519-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1519-207">Response</span></span>
<span data-ttu-id="a1519-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1519-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



