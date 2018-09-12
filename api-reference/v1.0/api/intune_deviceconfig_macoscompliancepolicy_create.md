# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="370f6-101">macOSCompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="370f6-101">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="370f6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="370f6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="370f6-103">Erstellen eines neuen [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="370f6-103">Create a new [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="370f6-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="370f6-104">Prerequisites</span></span>
<span data-ttu-id="370f6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="370f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="370f6-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="370f6-107">Permission type</span></span>|<span data-ttu-id="370f6-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="370f6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="370f6-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="370f6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="370f6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="370f6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="370f6-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="370f6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="370f6-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="370f6-112">Not supported.</span></span>|
|<span data-ttu-id="370f6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="370f6-113">Application</span></span>|<span data-ttu-id="370f6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="370f6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="370f6-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="370f6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="370f6-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="370f6-116">Request headers</span></span>
|<span data-ttu-id="370f6-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="370f6-117">Header</span></span>|<span data-ttu-id="370f6-118">Wert</span><span class="sxs-lookup"><span data-stu-id="370f6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="370f6-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="370f6-119">Authorization</span></span>|<span data-ttu-id="370f6-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="370f6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="370f6-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="370f6-121">Accept</span></span>|<span data-ttu-id="370f6-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="370f6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="370f6-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="370f6-123">Request body</span></span>
<span data-ttu-id="370f6-124">Geben Sie im Anforderungstext eine JSON-Darstellung des macOSCompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="370f6-124">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="370f6-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der macOSCompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="370f6-125">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="370f6-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="370f6-126">Property</span></span>|<span data-ttu-id="370f6-127">Typ</span><span class="sxs-lookup"><span data-stu-id="370f6-127">Type</span></span>|<span data-ttu-id="370f6-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="370f6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="370f6-129">ID</span><span class="sxs-lookup"><span data-stu-id="370f6-129">id</span></span>|<span data-ttu-id="370f6-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="370f6-130">String</span></span>|<span data-ttu-id="370f6-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="370f6-131">Key of the entity.</span></span> <span data-ttu-id="370f6-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="370f6-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="370f6-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="370f6-133">createdDateTime</span></span>|<span data-ttu-id="370f6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="370f6-134">DateTimeOffset</span></span>|<span data-ttu-id="370f6-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="370f6-135">DateTime the object was created.</span></span> <span data-ttu-id="370f6-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="370f6-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="370f6-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="370f6-137">description</span></span>|<span data-ttu-id="370f6-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="370f6-138">String</span></span>|<span data-ttu-id="370f6-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="370f6-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="370f6-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="370f6-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="370f6-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="370f6-141">lastModifiedDateTime</span></span>|<span data-ttu-id="370f6-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="370f6-142">DateTimeOffset</span></span>|<span data-ttu-id="370f6-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="370f6-143">DateTime the object was last modified.</span></span> <span data-ttu-id="370f6-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="370f6-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="370f6-145">displayName</span><span class="sxs-lookup"><span data-stu-id="370f6-145">displayName</span></span>|<span data-ttu-id="370f6-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="370f6-146">String</span></span>|<span data-ttu-id="370f6-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="370f6-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="370f6-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="370f6-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="370f6-149">Version</span><span class="sxs-lookup"><span data-stu-id="370f6-149">version</span></span>|<span data-ttu-id="370f6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="370f6-150">Int32</span></span>|<span data-ttu-id="370f6-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="370f6-151">Version of the device configuration.</span></span> <span data-ttu-id="370f6-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="370f6-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="370f6-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="370f6-153">passwordRequired</span></span>|<span data-ttu-id="370f6-154">Boolesch</span><span class="sxs-lookup"><span data-stu-id="370f6-154">Boolean</span></span>|<span data-ttu-id="370f6-155">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="370f6-155">Whether or not to require a password.</span></span>|
|<span data-ttu-id="370f6-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="370f6-156">passwordBlockSimple</span></span>|<span data-ttu-id="370f6-157">Boolesch</span><span class="sxs-lookup"><span data-stu-id="370f6-157">Boolean</span></span>|<span data-ttu-id="370f6-158">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="370f6-158">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="370f6-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="370f6-159">passwordExpirationDays</span></span>|<span data-ttu-id="370f6-160">Int32</span><span class="sxs-lookup"><span data-stu-id="370f6-160">Int32</span></span>|<span data-ttu-id="370f6-161">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="370f6-161">Number of days before the password expires.</span></span> <span data-ttu-id="370f6-162">Gültige Werte: 1 bis 65535.</span><span class="sxs-lookup"><span data-stu-id="370f6-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="370f6-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="370f6-163">passwordMinimumLength</span></span>|<span data-ttu-id="370f6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="370f6-164">Int32</span></span>|<span data-ttu-id="370f6-165">Mindestlänge von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="370f6-165">Minimum length of password.</span></span> <span data-ttu-id="370f6-166">Gültige Werte: 4 bis 14.</span><span class="sxs-lookup"><span data-stu-id="370f6-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="370f6-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="370f6-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="370f6-168">Int32</span><span class="sxs-lookup"><span data-stu-id="370f6-168">Int32</span></span>|<span data-ttu-id="370f6-169">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="370f6-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="370f6-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="370f6-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="370f6-171">Int32</span><span class="sxs-lookup"><span data-stu-id="370f6-171">Int32</span></span>|<span data-ttu-id="370f6-172">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="370f6-172">Number of previous passwords to block.</span></span> <span data-ttu-id="370f6-173">Gültige Werte: 1 bis 24.</span><span class="sxs-lookup"><span data-stu-id="370f6-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="370f6-174">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="370f6-174">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="370f6-175">Int32</span><span class="sxs-lookup"><span data-stu-id="370f6-175">Int32</span></span>|<span data-ttu-id="370f6-176">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="370f6-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="370f6-177">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="370f6-177">passwordRequiredType</span></span>|[<span data-ttu-id="370f6-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="370f6-178">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="370f6-179">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="370f6-179">The required password type.</span></span> <span data-ttu-id="370f6-180">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="370f6-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="370f6-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="370f6-181">osMinimumVersion</span></span>|<span data-ttu-id="370f6-182">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="370f6-182">String</span></span>|<span data-ttu-id="370f6-183">Mindestversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="370f6-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="370f6-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="370f6-184">osMaximumVersion</span></span>|<span data-ttu-id="370f6-185">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="370f6-185">String</span></span>|<span data-ttu-id="370f6-186">Höchstversion von IOS.</span><span class="sxs-lookup"><span data-stu-id="370f6-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="370f6-187">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="370f6-187">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="370f6-188">Boolesch</span><span class="sxs-lookup"><span data-stu-id="370f6-188">Boolean</span></span>|<span data-ttu-id="370f6-189">Gibt an, ob auf Geräten der Systemintegritätsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="370f6-189">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="370f6-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="370f6-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="370f6-191">Boolesch</span><span class="sxs-lookup"><span data-stu-id="370f6-191">Boolean</span></span>|<span data-ttu-id="370f6-192">Legt fest, dass auf Geräten der Gerätebedrohungsschutz aktiviert sein muss.</span><span class="sxs-lookup"><span data-stu-id="370f6-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="370f6-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="370f6-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="370f6-194">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="370f6-194">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="370f6-195">Legt die Mindestrisikostufe fest, ab der Mobile Threat Protection einen Konformitätsverstoß melden soll.</span><span class="sxs-lookup"><span data-stu-id="370f6-195">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="370f6-196">Mögliche Werte sind: `unavailable`, `secured`, `low`, `medium`, `high` und `notSet`.</span><span class="sxs-lookup"><span data-stu-id="370f6-196">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="370f6-197">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="370f6-197">storageRequireEncryption</span></span>|<span data-ttu-id="370f6-198">Boolesch</span><span class="sxs-lookup"><span data-stu-id="370f6-198">Boolean</span></span>|<span data-ttu-id="370f6-199">Gibt an, ob auf Mac OS-Geräten die Verschlüsselung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="370f6-199">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="370f6-200">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="370f6-200">firewallEnabled</span></span>|<span data-ttu-id="370f6-201">Boolesch</span><span class="sxs-lookup"><span data-stu-id="370f6-201">Boolean</span></span>|<span data-ttu-id="370f6-202">Gibt an, ob die Firewall aktiviert werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="370f6-202">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="370f6-203">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="370f6-203">firewallBlockAllIncoming</span></span>|<span data-ttu-id="370f6-204">Boolesch</span><span class="sxs-lookup"><span data-stu-id="370f6-204">Boolean</span></span>|<span data-ttu-id="370f6-205">Entspricht der Option "Alle eingehende Verbindungen blockieren".</span><span class="sxs-lookup"><span data-stu-id="370f6-205">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="370f6-206">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="370f6-206">firewallEnableStealthMode</span></span>|<span data-ttu-id="370f6-207">Boolesch</span><span class="sxs-lookup"><span data-stu-id="370f6-207">Boolean</span></span>|<span data-ttu-id="370f6-208">Entspricht "Geschützten Modus aktivieren".</span><span class="sxs-lookup"><span data-stu-id="370f6-208">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="370f6-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="370f6-209">Response</span></span>
<span data-ttu-id="370f6-210">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="370f6-210">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="370f6-211">Beispiel</span><span class="sxs-lookup"><span data-stu-id="370f6-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="370f6-212">Anforderung</span><span class="sxs-lookup"><span data-stu-id="370f6-212">Request</span></span>
<span data-ttu-id="370f6-213">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="370f6-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 913

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
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="370f6-214">Antwort</span><span class="sxs-lookup"><span data-stu-id="370f6-214">Response</span></span>
<span data-ttu-id="370f6-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="370f6-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








