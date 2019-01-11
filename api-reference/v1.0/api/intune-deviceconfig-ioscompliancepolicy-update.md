---
title: iosCompliancePolicy aktualisieren
description: Aktualisieren der Eigenschaften eines iosCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9e87f118033ff4bd72ea6da18f89d9c8698464b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858128"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="de763-103">iosCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="de763-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="de763-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="de763-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de763-105">Aktualisieren der Eigenschaften eines [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="de763-105">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de763-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="de763-106">Prerequisites</span></span>
<span data-ttu-id="de763-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de763-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de763-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="de763-109">Permission type</span></span>|<span data-ttu-id="de763-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="de763-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de763-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="de763-111">Delegated (work or school account)</span></span>|<span data-ttu-id="de763-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de763-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de763-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="de763-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de763-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de763-114">Not supported.</span></span>|
|<span data-ttu-id="de763-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="de763-115">Application</span></span>|<span data-ttu-id="de763-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de763-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de763-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="de763-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="de763-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="de763-118">Request headers</span></span>
|<span data-ttu-id="de763-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="de763-119">Header</span></span>|<span data-ttu-id="de763-120">Wert</span><span class="sxs-lookup"><span data-stu-id="de763-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de763-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="de763-121">Authorization</span></span>|<span data-ttu-id="de763-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="de763-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de763-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="de763-123">Accept</span></span>|<span data-ttu-id="de763-124">application/json</span><span class="sxs-lookup"><span data-stu-id="de763-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de763-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="de763-125">Request body</span></span>
<span data-ttu-id="de763-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="de763-126">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="de763-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="de763-127">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="de763-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="de763-128">Property</span></span>|<span data-ttu-id="de763-129">Typ</span><span class="sxs-lookup"><span data-stu-id="de763-129">Type</span></span>|<span data-ttu-id="de763-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de763-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de763-131">id</span><span class="sxs-lookup"><span data-stu-id="de763-131">id</span></span>|<span data-ttu-id="de763-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de763-132">String</span></span>|<span data-ttu-id="de763-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="de763-133">Key of the entity.</span></span> <span data-ttu-id="de763-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de763-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="de763-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de763-135">createdDateTime</span></span>|<span data-ttu-id="de763-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de763-136">DateTimeOffset</span></span>|<span data-ttu-id="de763-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="de763-137">DateTime the object was created.</span></span> <span data-ttu-id="de763-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de763-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="de763-139">description</span><span class="sxs-lookup"><span data-stu-id="de763-139">description</span></span>|<span data-ttu-id="de763-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de763-140">String</span></span>|<span data-ttu-id="de763-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="de763-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="de763-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de763-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="de763-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de763-143">lastModifiedDateTime</span></span>|<span data-ttu-id="de763-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de763-144">DateTimeOffset</span></span>|<span data-ttu-id="de763-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="de763-145">DateTime the object was last modified.</span></span> <span data-ttu-id="de763-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de763-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="de763-147">displayName</span><span class="sxs-lookup"><span data-stu-id="de763-147">displayName</span></span>|<span data-ttu-id="de763-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de763-148">String</span></span>|<span data-ttu-id="de763-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="de763-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="de763-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de763-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="de763-151">Version</span><span class="sxs-lookup"><span data-stu-id="de763-151">version</span></span>|<span data-ttu-id="de763-152">Int32</span><span class="sxs-lookup"><span data-stu-id="de763-152">Int32</span></span>|<span data-ttu-id="de763-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="de763-153">Version of the device configuration.</span></span> <span data-ttu-id="de763-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de763-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="de763-155">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="de763-155">passcodeBlockSimple</span></span>|<span data-ttu-id="de763-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de763-156">Boolean</span></span>|<span data-ttu-id="de763-157">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="de763-157">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="de763-158">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="de763-158">passcodeExpirationDays</span></span>|<span data-ttu-id="de763-159">Int32</span><span class="sxs-lookup"><span data-stu-id="de763-159">Int32</span></span>|<span data-ttu-id="de763-160">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="de763-160">Number of days before the passcode expires.</span></span> <span data-ttu-id="de763-161">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="de763-161">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="de763-162">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="de763-162">passcodeMinimumLength</span></span>|<span data-ttu-id="de763-163">Int32</span><span class="sxs-lookup"><span data-stu-id="de763-163">Int32</span></span>|<span data-ttu-id="de763-164">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="de763-164">Minimum length of passcode.</span></span> <span data-ttu-id="de763-165">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="de763-165">Valid values 4 to 14</span></span>|
|<span data-ttu-id="de763-166">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="de763-166">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="de763-167">Int32</span><span class="sxs-lookup"><span data-stu-id="de763-167">Int32</span></span>|<span data-ttu-id="de763-168">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="de763-168">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="de763-169">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="de763-169">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="de763-170">Int32</span><span class="sxs-lookup"><span data-stu-id="de763-170">Int32</span></span>|<span data-ttu-id="de763-171">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="de763-171">Number of previous passcodes to block.</span></span> <span data-ttu-id="de763-172">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="de763-172">Valid values 1 to 24</span></span>|
|<span data-ttu-id="de763-173">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="de763-173">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="de763-174">Int32</span><span class="sxs-lookup"><span data-stu-id="de763-174">Int32</span></span>|<span data-ttu-id="de763-175">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="de763-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="de763-176">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="de763-176">passcodeRequiredType</span></span>|[<span data-ttu-id="de763-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="de763-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="de763-178">Der erforderliche Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="de763-178">The required passcode type.</span></span> <span data-ttu-id="de763-179">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="de763-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="de763-180">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="de763-180">passcodeRequired</span></span>|<span data-ttu-id="de763-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de763-181">Boolean</span></span>|<span data-ttu-id="de763-182">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="de763-182">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="de763-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="de763-183">osMinimumVersion</span></span>|<span data-ttu-id="de763-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de763-184">String</span></span>|<span data-ttu-id="de763-185">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="de763-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="de763-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="de763-186">osMaximumVersion</span></span>|<span data-ttu-id="de763-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="de763-187">String</span></span>|<span data-ttu-id="de763-188">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="de763-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="de763-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="de763-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="de763-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de763-190">Boolean</span></span>|<span data-ttu-id="de763-191">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="de763-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="de763-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="de763-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="de763-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de763-193">Boolean</span></span>|<span data-ttu-id="de763-194">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="de763-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="de763-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="de763-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="de763-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="de763-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="de763-197">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="de763-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="de763-198">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="de763-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="de763-199">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="de763-199">managedEmailProfileRequired</span></span>|<span data-ttu-id="de763-200">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="de763-200">Boolean</span></span>|<span data-ttu-id="de763-201">Gibt an, ob ein verwaltetes E-Mail-Profil erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="de763-201">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="de763-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="de763-202">Response</span></span>
<span data-ttu-id="de763-203">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de763-203">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de763-204">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de763-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="de763-205">Anforderung</span><span class="sxs-lookup"><span data-stu-id="de763-205">Request</span></span>
<span data-ttu-id="de763-206">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="de763-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="de763-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="de763-207">Response</span></span>
<span data-ttu-id="de763-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de763-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



