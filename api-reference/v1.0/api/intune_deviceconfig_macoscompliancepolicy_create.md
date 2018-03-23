# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="b0292-101">macOSCompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="b0292-101">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="b0292-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b0292-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0292-103">Erstellen eines neuen [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b0292-103">Create a new [plannerBucket](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0292-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b0292-104">Prerequisites</span></span>
<span data-ttu-id="b0292-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b0292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b0292-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b0292-107">Permission type</span></span>|<span data-ttu-id="b0292-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b0292-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0292-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b0292-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b0292-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0292-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0292-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b0292-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0292-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0292-112">Not supported.</span></span>|
|<span data-ttu-id="b0292-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b0292-113">Application</span></span>|<span data-ttu-id="b0292-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b0292-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0292-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0292-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="b0292-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b0292-116">Request headers</span></span>
|<span data-ttu-id="b0292-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b0292-117">Header</span></span>|<span data-ttu-id="b0292-118">Wert</span><span class="sxs-lookup"><span data-stu-id="b0292-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0292-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0292-119">Authorization</span></span>|<span data-ttu-id="b0292-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b0292-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b0292-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b0292-121">Accept</span></span>|<span data-ttu-id="b0292-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b0292-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0292-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b0292-123">Request body</span></span>
<span data-ttu-id="b0292-124">Geben Sie im Anforderungstext eine JSON-Darstellung des macOSCompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b0292-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="b0292-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der macOSCompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b0292-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="b0292-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b0292-126">Property</span></span>|<span data-ttu-id="b0292-127">Typ</span><span class="sxs-lookup"><span data-stu-id="b0292-127">Type</span></span>|<span data-ttu-id="b0292-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0292-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0292-129">id</span><span class="sxs-lookup"><span data-stu-id="b0292-129">id</span></span>|<span data-ttu-id="b0292-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0292-130">String</span></span>|<span data-ttu-id="b0292-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="b0292-131">Key of the setting.</span></span> <span data-ttu-id="b0292-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0292-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b0292-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0292-133">createdDateTime</span></span>|<span data-ttu-id="b0292-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0292-134">DateTimeOffset</span></span>|<span data-ttu-id="b0292-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b0292-135">DateTime the object was created.</span></span> <span data-ttu-id="b0292-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0292-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b0292-137">description</span><span class="sxs-lookup"><span data-stu-id="b0292-137">description</span></span>|<span data-ttu-id="b0292-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0292-138">String</span></span>|<span data-ttu-id="b0292-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b0292-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b0292-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0292-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b0292-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0292-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b0292-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0292-142">DateTimeOffset</span></span>|<span data-ttu-id="b0292-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b0292-143">Indicates the date the object was last modified.</span></span> <span data-ttu-id="b0292-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0292-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b0292-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b0292-145">displayName</span></span>|<span data-ttu-id="b0292-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0292-146">String</span></span>|<span data-ttu-id="b0292-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b0292-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b0292-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0292-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b0292-149">Version</span><span class="sxs-lookup"><span data-stu-id="b0292-149">version</span></span>|<span data-ttu-id="b0292-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b0292-150">Int32</span></span>|<span data-ttu-id="b0292-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b0292-151">Version of the device configuration.</span></span> <span data-ttu-id="b0292-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0292-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b0292-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b0292-153">passwordRequired</span></span>|<span data-ttu-id="b0292-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0292-154">Boolean</span></span>|<span data-ttu-id="b0292-155">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="b0292-155">Whether or not to require a password.</span></span>|
|<span data-ttu-id="b0292-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b0292-156">passwordBlockSimple</span></span>|<span data-ttu-id="b0292-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0292-157">Boolean</span></span>|<span data-ttu-id="b0292-158">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="b0292-158">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="b0292-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b0292-159">passwordExpirationDays</span></span>|<span data-ttu-id="b0292-160">Int32</span><span class="sxs-lookup"><span data-stu-id="b0292-160">Int32</span></span>|<span data-ttu-id="b0292-161">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="b0292-161">Number of days before the password expires.</span></span> <span data-ttu-id="b0292-162">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="b0292-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b0292-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b0292-163">passwordMinimumLength</span></span>|<span data-ttu-id="b0292-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b0292-164">Int32</span></span>|<span data-ttu-id="b0292-165">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="b0292-165">Minimum length of password.</span></span> <span data-ttu-id="b0292-166">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="b0292-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="b0292-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b0292-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b0292-168">Int32</span><span class="sxs-lookup"><span data-stu-id="b0292-168">Int32</span></span>|<span data-ttu-id="b0292-169">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="b0292-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b0292-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b0292-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b0292-171">Int32</span><span class="sxs-lookup"><span data-stu-id="b0292-171">Int32</span></span>|<span data-ttu-id="b0292-172">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="b0292-172">Number of previous passwords to block.</span></span> <span data-ttu-id="b0292-173">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="b0292-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b0292-174">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b0292-174">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b0292-175">Int32</span><span class="sxs-lookup"><span data-stu-id="b0292-175">Int32</span></span>|<span data-ttu-id="b0292-176">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen.</span><span class="sxs-lookup"><span data-stu-id="b0292-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b0292-177">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b0292-177">passwordRequiredType</span></span>|<span data-ttu-id="b0292-178">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0292-178">String</span></span>|<span data-ttu-id="b0292-179">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="b0292-179">The required password type.</span></span> <span data-ttu-id="b0292-180">Mögliche Werte: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b0292-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b0292-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b0292-181">osMinimumVersion</span></span>|<span data-ttu-id="b0292-182">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0292-182">String</span></span>|<span data-ttu-id="b0292-183">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="b0292-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="b0292-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b0292-184">osMaximumVersion</span></span>|<span data-ttu-id="b0292-185">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0292-185">String</span></span>|<span data-ttu-id="b0292-186">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="b0292-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="b0292-187">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b0292-187">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="b0292-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0292-188">Boolean</span></span>|<span data-ttu-id="b0292-189">Gibt an, ob auf Geräten der Systemintegritätsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="b0292-189">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="b0292-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b0292-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="b0292-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0292-191">Boolean</span></span>|<span data-ttu-id="b0292-192">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="b0292-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="b0292-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b0292-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|<span data-ttu-id="b0292-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0292-194">String</span></span>|<span data-ttu-id="b0292-195">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="b0292-195">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b0292-196">Mögliche Werte: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="b0292-196">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b0292-197">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b0292-197">storageRequireEncryption</span></span>|<span data-ttu-id="b0292-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0292-198">Boolean</span></span>|<span data-ttu-id="b0292-199">Gibt an, ob auf Mac OS-Geräten die Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b0292-199">Require encryption on Mac OS devices.</span></span>|



## <a name="response"></a><span data-ttu-id="b0292-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0292-200">Response</span></span>
<span data-ttu-id="b0292-201">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b0292-201">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_deviceconfig_macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0292-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b0292-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0292-203">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0292-203">Request</span></span>
<span data-ttu-id="b0292-204">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b0292-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 810

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
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
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="b0292-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0292-205">Response</span></span>
<span data-ttu-id="b0292-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b0292-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 918

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
  "storageRequireEncryption": true
}
```



