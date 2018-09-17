# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="97617-101">Erstellen von „windows10MobileCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="97617-101">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="97617-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="97617-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97617-103">Diese Methode erstellt ein neues Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="97617-103">Create a new [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97617-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="97617-104">Prerequisites</span></span>
<span data-ttu-id="97617-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97617-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97617-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97617-107">Permission type</span></span>|<span data-ttu-id="97617-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97617-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97617-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97617-109">Delegated (work or school account)</span></span>|<span data-ttu-id="97617-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97617-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97617-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97617-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97617-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97617-112">Not supported.</span></span>|
|<span data-ttu-id="97617-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97617-113">Application</span></span>|<span data-ttu-id="97617-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97617-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97617-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97617-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="97617-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97617-116">Request headers</span></span>
|<span data-ttu-id="97617-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="97617-117">Header</span></span>|<span data-ttu-id="97617-118">Wert</span><span class="sxs-lookup"><span data-stu-id="97617-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97617-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="97617-119">Authorization</span></span>|<span data-ttu-id="97617-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="97617-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97617-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="97617-121">Accept</span></span>|<span data-ttu-id="97617-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="97617-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97617-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97617-123">Request body</span></span>
<span data-ttu-id="97617-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10MobileCompliancePolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="97617-124">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="97617-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10MobileCompliancePolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="97617-125">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="97617-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="97617-126">Property</span></span>|<span data-ttu-id="97617-127">Typ</span><span class="sxs-lookup"><span data-stu-id="97617-127">Type</span></span>|<span data-ttu-id="97617-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97617-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97617-129">id</span><span class="sxs-lookup"><span data-stu-id="97617-129">id</span></span>|<span data-ttu-id="97617-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97617-130">String</span></span>|<span data-ttu-id="97617-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="97617-131">Key of the entity.</span></span> <span data-ttu-id="97617-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="97617-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="97617-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97617-133">createdDateTime</span></span>|<span data-ttu-id="97617-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97617-134">DateTimeOffset</span></span>|<span data-ttu-id="97617-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="97617-135">DateTime the object was created.</span></span> <span data-ttu-id="97617-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="97617-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="97617-137">description</span><span class="sxs-lookup"><span data-stu-id="97617-137">description</span></span>|<span data-ttu-id="97617-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97617-138">String</span></span>|<span data-ttu-id="97617-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="97617-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="97617-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="97617-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="97617-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97617-141">lastModifiedDateTime</span></span>|<span data-ttu-id="97617-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97617-142">DateTimeOffset</span></span>|<span data-ttu-id="97617-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="97617-143">DateTime the object was last modified.</span></span> <span data-ttu-id="97617-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="97617-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="97617-145">displayName</span><span class="sxs-lookup"><span data-stu-id="97617-145">displayName</span></span>|<span data-ttu-id="97617-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97617-146">String</span></span>|<span data-ttu-id="97617-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="97617-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="97617-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="97617-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="97617-149">Version</span><span class="sxs-lookup"><span data-stu-id="97617-149">version</span></span>|<span data-ttu-id="97617-150">Int32</span><span class="sxs-lookup"><span data-stu-id="97617-150">Int32</span></span>|<span data-ttu-id="97617-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="97617-151">Version of the device configuration.</span></span> <span data-ttu-id="97617-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="97617-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="97617-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="97617-153">passwordRequired</span></span>|<span data-ttu-id="97617-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="97617-154">Boolean</span></span>|<span data-ttu-id="97617-155">Legt fest, dass zum Entsperren des Windows Phone-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="97617-155">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="97617-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="97617-156">passwordBlockSimple</span></span>|<span data-ttu-id="97617-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="97617-157">Boolean</span></span>|<span data-ttu-id="97617-158">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="97617-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="97617-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="97617-159">passwordMinimumLength</span></span>|<span data-ttu-id="97617-160">Int32</span><span class="sxs-lookup"><span data-stu-id="97617-160">Int32</span></span>|<span data-ttu-id="97617-161">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="97617-161">Minimum password length.</span></span> <span data-ttu-id="97617-162">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="97617-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="97617-163">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="97617-163">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="97617-164">Int32</span><span class="sxs-lookup"><span data-stu-id="97617-164">Int32</span></span>|<span data-ttu-id="97617-165">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="97617-165">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="97617-166">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="97617-166">passwordRequiredType</span></span>|[<span data-ttu-id="97617-167">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="97617-167">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="97617-p109">Der erforderliche Kennworttyp. Mögliche Werte: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="97617-p109">The required password type. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="97617-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="97617-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="97617-171">Int32</span><span class="sxs-lookup"><span data-stu-id="97617-171">Int32</span></span>|<span data-ttu-id="97617-172">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="97617-172">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="97617-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="97617-173">passwordExpirationDays</span></span>|<span data-ttu-id="97617-174">Int32</span><span class="sxs-lookup"><span data-stu-id="97617-174">Int32</span></span>|<span data-ttu-id="97617-175">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="97617-175">Number of days before password expiration.</span></span> <span data-ttu-id="97617-176">Gültige Werte: 1 bis 255.</span><span class="sxs-lookup"><span data-stu-id="97617-176">Valid values 1 to 255</span></span>|
|<span data-ttu-id="97617-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="97617-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="97617-178">Int32</span><span class="sxs-lookup"><span data-stu-id="97617-178">Int32</span></span>|<span data-ttu-id="97617-179">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="97617-179">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="97617-180">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="97617-180">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="97617-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="97617-181">Boolean</span></span>|<span data-ttu-id="97617-182">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="97617-182">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="97617-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="97617-183">osMinimumVersion</span></span>|<span data-ttu-id="97617-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97617-184">String</span></span>|<span data-ttu-id="97617-185">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="97617-185">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="97617-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="97617-186">osMaximumVersion</span></span>|<span data-ttu-id="97617-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97617-187">String</span></span>|<span data-ttu-id="97617-188">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="97617-188">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="97617-189">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="97617-189">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="97617-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="97617-190">Boolean</span></span>|<span data-ttu-id="97617-191">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="97617-191">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="97617-192">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="97617-192">bitLockerEnabled</span></span>|<span data-ttu-id="97617-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="97617-193">Boolean</span></span>|<span data-ttu-id="97617-194">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="97617-194">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="97617-195">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="97617-195">secureBootEnabled</span></span>|<span data-ttu-id="97617-196">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="97617-196">Boolean</span></span>|<span data-ttu-id="97617-197">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="97617-197">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="97617-198">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="97617-198">codeIntegrityEnabled</span></span>|<span data-ttu-id="97617-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="97617-199">Boolean</span></span>|<span data-ttu-id="97617-200">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="97617-200">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="97617-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="97617-201">storageRequireEncryption</span></span>|<span data-ttu-id="97617-202">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="97617-202">Boolean</span></span>|<span data-ttu-id="97617-203">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="97617-203">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="97617-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="97617-204">Response</span></span>
<span data-ttu-id="97617-205">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="97617-205">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97617-206">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97617-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="97617-207">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97617-207">Request</span></span>
<span data-ttu-id="97617-208">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97617-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 856

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="97617-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="97617-209">Response</span></span>
<span data-ttu-id="97617-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97617-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "id": "3d4237b0-37b0-3d42-b037-423db037423d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```








