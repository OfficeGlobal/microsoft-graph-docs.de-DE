---
title: iosCompliancePolicy aktualisieren
description: Aktualisieren der Eigenschaften eines iosCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb8b8590fd59154fce31912d6275d23929a66f94
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977478"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="86cd8-103">iosCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="86cd8-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="86cd8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="86cd8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86cd8-105">Aktualisieren der Eigenschaften eines [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="86cd8-105">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86cd8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="86cd8-106">Prerequisites</span></span>
<span data-ttu-id="86cd8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86cd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86cd8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86cd8-109">Permission type</span></span>|<span data-ttu-id="86cd8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86cd8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86cd8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86cd8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86cd8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86cd8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86cd8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="86cd8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86cd8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86cd8-114">Not supported.</span></span>|
|<span data-ttu-id="86cd8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86cd8-115">Application</span></span>|<span data-ttu-id="86cd8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86cd8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86cd8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86cd8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="86cd8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86cd8-118">Request headers</span></span>
|<span data-ttu-id="86cd8-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="86cd8-119">Header</span></span>|<span data-ttu-id="86cd8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="86cd8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86cd8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="86cd8-121">Authorization</span></span>|<span data-ttu-id="86cd8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="86cd8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86cd8-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="86cd8-123">Accept</span></span>|<span data-ttu-id="86cd8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="86cd8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86cd8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="86cd8-125">Request body</span></span>
<span data-ttu-id="86cd8-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="86cd8-126">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="86cd8-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="86cd8-127">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="86cd8-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86cd8-128">Property</span></span>|<span data-ttu-id="86cd8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="86cd8-129">Type</span></span>|<span data-ttu-id="86cd8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86cd8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86cd8-131">id</span><span class="sxs-lookup"><span data-stu-id="86cd8-131">id</span></span>|<span data-ttu-id="86cd8-132">String</span><span class="sxs-lookup"><span data-stu-id="86cd8-132">String</span></span>|<span data-ttu-id="86cd8-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="86cd8-133">Key of the entity.</span></span> <span data-ttu-id="86cd8-134">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="86cd8-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="86cd8-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86cd8-135">createdDateTime</span></span>|<span data-ttu-id="86cd8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86cd8-136">DateTimeOffset</span></span>|<span data-ttu-id="86cd8-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="86cd8-137">DateTime the object was created.</span></span> <span data-ttu-id="86cd8-138">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="86cd8-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="86cd8-139">description</span><span class="sxs-lookup"><span data-stu-id="86cd8-139">description</span></span>|<span data-ttu-id="86cd8-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86cd8-140">String</span></span>|<span data-ttu-id="86cd8-141">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="86cd8-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86cd8-142">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="86cd8-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="86cd8-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86cd8-143">lastModifiedDateTime</span></span>|<span data-ttu-id="86cd8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86cd8-144">DateTimeOffset</span></span>|<span data-ttu-id="86cd8-145">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="86cd8-145">DateTime the object was last modified.</span></span> <span data-ttu-id="86cd8-146">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="86cd8-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="86cd8-147">displayName</span><span class="sxs-lookup"><span data-stu-id="86cd8-147">displayName</span></span>|<span data-ttu-id="86cd8-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86cd8-148">String</span></span>|<span data-ttu-id="86cd8-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="86cd8-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86cd8-150">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="86cd8-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="86cd8-151">Version</span><span class="sxs-lookup"><span data-stu-id="86cd8-151">version</span></span>|<span data-ttu-id="86cd8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd8-152">Int32</span></span>|<span data-ttu-id="86cd8-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="86cd8-153">Version of the device configuration.</span></span> <span data-ttu-id="86cd8-154">Geerbt von [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="86cd8-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="86cd8-155">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="86cd8-155">passcodeBlockSimple</span></span>|<span data-ttu-id="86cd8-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="86cd8-156">Boolean</span></span>|<span data-ttu-id="86cd8-157">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="86cd8-157">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="86cd8-158">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="86cd8-158">passcodeExpirationDays</span></span>|<span data-ttu-id="86cd8-159">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd8-159">Int32</span></span>|<span data-ttu-id="86cd8-160">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="86cd8-160">Number of days before the passcode expires.</span></span> <span data-ttu-id="86cd8-161">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="86cd8-161">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="86cd8-162">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="86cd8-162">passcodeMinimumLength</span></span>|<span data-ttu-id="86cd8-163">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd8-163">Int32</span></span>|<span data-ttu-id="86cd8-164">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="86cd8-164">Minimum length of passcode.</span></span> <span data-ttu-id="86cd8-165">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="86cd8-165">Valid values 4 to 14</span></span>|
|<span data-ttu-id="86cd8-166">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="86cd8-166">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="86cd8-167">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd8-167">Int32</span></span>|<span data-ttu-id="86cd8-168">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="86cd8-168">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="86cd8-169">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="86cd8-169">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="86cd8-170">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd8-170">Int32</span></span>|<span data-ttu-id="86cd8-171">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="86cd8-171">Number of previous passcodes to block.</span></span> <span data-ttu-id="86cd8-172">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="86cd8-172">Valid values 1 to 24</span></span>|
|<span data-ttu-id="86cd8-173">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="86cd8-173">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="86cd8-174">Int32</span><span class="sxs-lookup"><span data-stu-id="86cd8-174">Int32</span></span>|<span data-ttu-id="86cd8-175">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.</span><span class="sxs-lookup"><span data-stu-id="86cd8-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="86cd8-176">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="86cd8-176">passcodeRequiredType</span></span>|[<span data-ttu-id="86cd8-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="86cd8-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="86cd8-178">Der erforderliche Kennungstyp.</span><span class="sxs-lookup"><span data-stu-id="86cd8-178">The required passcode type.</span></span> <span data-ttu-id="86cd8-179">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="86cd8-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="86cd8-180">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="86cd8-180">passcodeRequired</span></span>|<span data-ttu-id="86cd8-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="86cd8-181">Boolean</span></span>|<span data-ttu-id="86cd8-182">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="86cd8-182">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="86cd8-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="86cd8-183">osMinimumVersion</span></span>|<span data-ttu-id="86cd8-184">String</span><span class="sxs-lookup"><span data-stu-id="86cd8-184">String</span></span>|<span data-ttu-id="86cd8-185">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="86cd8-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="86cd8-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="86cd8-186">osMaximumVersion</span></span>|<span data-ttu-id="86cd8-187">String</span><span class="sxs-lookup"><span data-stu-id="86cd8-187">String</span></span>|<span data-ttu-id="86cd8-188">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="86cd8-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="86cd8-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="86cd8-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="86cd8-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="86cd8-190">Boolean</span></span>|<span data-ttu-id="86cd8-191">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="86cd8-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="86cd8-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="86cd8-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="86cd8-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="86cd8-193">Boolean</span></span>|<span data-ttu-id="86cd8-194">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="86cd8-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="86cd8-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="86cd8-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="86cd8-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="86cd8-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="86cd8-197">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="86cd8-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="86cd8-198">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="86cd8-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="86cd8-199">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="86cd8-199">managedEmailProfileRequired</span></span>|<span data-ttu-id="86cd8-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="86cd8-200">Boolean</span></span>|<span data-ttu-id="86cd8-201">Gibt an, ob ein verwaltetes E-Mail-Profil erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="86cd8-201">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="86cd8-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="86cd8-202">Response</span></span>
<span data-ttu-id="86cd8-203">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86cd8-203">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86cd8-204">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86cd8-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="86cd8-205">Anforderung</span><span class="sxs-lookup"><span data-stu-id="86cd8-205">Request</span></span>
<span data-ttu-id="86cd8-206">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86cd8-206">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="86cd8-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="86cd8-207">Response</span></span>
<span data-ttu-id="86cd8-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86cd8-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



