# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="590a4-101">iosCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="590a4-101">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="590a4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="590a4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="590a4-103">Aktualisieren der Eigenschaften eines [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="590a4-103">Update the properties of a [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="590a4-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="590a4-104">Prerequisites</span></span>
<span data-ttu-id="590a4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="590a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="590a4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="590a4-107">Permission type</span></span>|<span data-ttu-id="590a4-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="590a4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="590a4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="590a4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="590a4-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="590a4-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="590a4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="590a4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="590a4-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="590a4-112">Not supported.</span></span>|
|<span data-ttu-id="590a4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="590a4-113">Application</span></span>|<span data-ttu-id="590a4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="590a4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="590a4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="590a4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="590a4-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="590a4-116">Request headers</span></span>
|<span data-ttu-id="590a4-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="590a4-117">Header</span></span>|<span data-ttu-id="590a4-118">Wert</span><span class="sxs-lookup"><span data-stu-id="590a4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="590a4-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="590a4-119">Authorization</span></span>|<span data-ttu-id="590a4-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="590a4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="590a4-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="590a4-121">Accept</span></span>|<span data-ttu-id="590a4-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="590a4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="590a4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="590a4-123">Request body</span></span>
<span data-ttu-id="590a4-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="590a4-124">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="590a4-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="590a4-125">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="590a4-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="590a4-126">Property</span></span>|<span data-ttu-id="590a4-127">Typ</span><span class="sxs-lookup"><span data-stu-id="590a4-127">Type</span></span>|<span data-ttu-id="590a4-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="590a4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="590a4-129">id</span><span class="sxs-lookup"><span data-stu-id="590a4-129">id</span></span>|<span data-ttu-id="590a4-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="590a4-130">String</span></span>|<span data-ttu-id="590a4-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="590a4-131">Key of the entity.</span></span> <span data-ttu-id="590a4-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="590a4-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="590a4-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="590a4-133">createdDateTime</span></span>|<span data-ttu-id="590a4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="590a4-134">DateTimeOffset</span></span>|<span data-ttu-id="590a4-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="590a4-135">DateTime the object was created.</span></span> <span data-ttu-id="590a4-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="590a4-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="590a4-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="590a4-137">description</span></span>|<span data-ttu-id="590a4-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="590a4-138">String</span></span>|<span data-ttu-id="590a4-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="590a4-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="590a4-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="590a4-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="590a4-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="590a4-141">lastModifiedDateTime</span></span>|<span data-ttu-id="590a4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="590a4-142">DateTimeOffset</span></span>|<span data-ttu-id="590a4-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="590a4-143">DateTime the object was last modified.</span></span> <span data-ttu-id="590a4-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="590a4-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="590a4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="590a4-145">displayName</span></span>|<span data-ttu-id="590a4-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="590a4-146">String</span></span>|<span data-ttu-id="590a4-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="590a4-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="590a4-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="590a4-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="590a4-149">Version</span><span class="sxs-lookup"><span data-stu-id="590a4-149">version</span></span>|<span data-ttu-id="590a4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="590a4-150">Int32</span></span>|<span data-ttu-id="590a4-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="590a4-151">Version of the device configuration.</span></span> <span data-ttu-id="590a4-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="590a4-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="590a4-153">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="590a4-153">passcodeBlockSimple</span></span>|<span data-ttu-id="590a4-154">boolesch</span><span class="sxs-lookup"><span data-stu-id="590a4-154">Boolean</span></span>|<span data-ttu-id="590a4-155">Gibt an, ob einfache Kennungen erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="590a4-155">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="590a4-156">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="590a4-156">passcodeExpirationDays</span></span>|<span data-ttu-id="590a4-157">Int32</span><span class="sxs-lookup"><span data-stu-id="590a4-157">Int32</span></span>|<span data-ttu-id="590a4-158">Zeit in Tagen bis zum Ablaufen der Kennung.</span><span class="sxs-lookup"><span data-stu-id="590a4-158">Number of days before the passcode expires.</span></span> <span data-ttu-id="590a4-159">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="590a4-159">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="590a4-160">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="590a4-160">passcodeMinimumLength</span></span>|<span data-ttu-id="590a4-161">Int32</span><span class="sxs-lookup"><span data-stu-id="590a4-161">Int32</span></span>|<span data-ttu-id="590a4-162">Mindestlänge von Kennungen.</span><span class="sxs-lookup"><span data-stu-id="590a4-162">Minimum length of passcode.</span></span> <span data-ttu-id="590a4-163">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="590a4-163">Valid values 4 to 14</span></span>|
|<span data-ttu-id="590a4-164">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="590a4-164">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="590a4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="590a4-165">Int32</span></span>|<span data-ttu-id="590a4-166">Zeitraum von Inaktivität in Minuten, bevor die Eingabe einer Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="590a4-166">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="590a4-167">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="590a4-167">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="590a4-168">Int32</span><span class="sxs-lookup"><span data-stu-id="590a4-168">Int32</span></span>|<span data-ttu-id="590a4-169">Anzahl der zuletzt verwendeten Kennungen, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="590a4-169">Number of previous passcodes to block.</span></span> <span data-ttu-id="590a4-170">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="590a4-170">Valid values 1 to 24</span></span>|
|<span data-ttu-id="590a4-171">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="590a4-171">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="590a4-172">Int32</span><span class="sxs-lookup"><span data-stu-id="590a4-172">Int32</span></span>|<span data-ttu-id="590a4-173">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="590a4-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="590a4-174">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="590a4-174">passcodeRequiredType</span></span>|[<span data-ttu-id="590a4-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="590a4-175">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="590a4-p111">Der erforderliche Kennungsyp. Mögliche Werte: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="590a4-p111">The required passcode type. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="590a4-178">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="590a4-178">passcodeRequired</span></span>|<span data-ttu-id="590a4-179">boolesch</span><span class="sxs-lookup"><span data-stu-id="590a4-179">Boolean</span></span>|<span data-ttu-id="590a4-180">Gibt an, ob eine Kennung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="590a4-180">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="590a4-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="590a4-181">osMinimumVersion</span></span>|<span data-ttu-id="590a4-182">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="590a4-182">String</span></span>|<span data-ttu-id="590a4-183">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="590a4-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="590a4-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="590a4-184">osMaximumVersion</span></span>|<span data-ttu-id="590a4-185">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="590a4-185">String</span></span>|<span data-ttu-id="590a4-186">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="590a4-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="590a4-187">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="590a4-187">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="590a4-188">boolesch</span><span class="sxs-lookup"><span data-stu-id="590a4-188">Boolean</span></span>|<span data-ttu-id="590a4-189">Legt fest, dass weder gerootete Geräte verwendet werden dürfen noch Geräte, für die ein Jailbreak durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="590a4-189">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="590a4-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="590a4-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="590a4-191">boolesch</span><span class="sxs-lookup"><span data-stu-id="590a4-191">Boolean</span></span>|<span data-ttu-id="590a4-192">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="590a4-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="590a4-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="590a4-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="590a4-194">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="590a4-194">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="590a4-p112">Legt die Mindestrisikostufe fest, ob der Mobile Threat Protection einen Konformitätsverstoß melden soll. Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="590a4-p112">Require Mobile Threat Protection minimum risk level to report noncompliance. The possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="590a4-197">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="590a4-197">managedEmailProfileRequired</span></span>|<span data-ttu-id="590a4-198">boolesch</span><span class="sxs-lookup"><span data-stu-id="590a4-198">Boolean</span></span>|<span data-ttu-id="590a4-199">Gibt an, ob ein verwaltetes E-Mail-Profil erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="590a4-199">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="590a4-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="590a4-200">Response</span></span>
<span data-ttu-id="590a4-201">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="590a4-201">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="590a4-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="590a4-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="590a4-203">Anforderung</span><span class="sxs-lookup"><span data-stu-id="590a4-203">Request</span></span>
<span data-ttu-id="590a4-204">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="590a4-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 751

{
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

### <a name="response"></a><span data-ttu-id="590a4-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="590a4-205">Response</span></span>
<span data-ttu-id="590a4-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="590a4-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








