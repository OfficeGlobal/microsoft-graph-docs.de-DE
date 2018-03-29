# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="32137-101">Erstellen von „windows10MobileCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="32137-101">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="32137-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="32137-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32137-103">Diese Methode erstellt ein neues Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32137-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32137-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="32137-104">Prerequisites</span></span>
<span data-ttu-id="32137-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="32137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="32137-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32137-107">Permission type</span></span>|<span data-ttu-id="32137-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32137-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32137-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32137-109">Delegated (work or school account)</span></span>|<span data-ttu-id="32137-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32137-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32137-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32137-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32137-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32137-112">Not supported.</span></span>|
|<span data-ttu-id="32137-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32137-113">Application</span></span>|<span data-ttu-id="32137-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32137-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32137-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32137-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="32137-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32137-116">Request headers</span></span>
|<span data-ttu-id="32137-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="32137-117">Header</span></span>|<span data-ttu-id="32137-118">Wert</span><span class="sxs-lookup"><span data-stu-id="32137-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32137-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="32137-119">Authorization</span></span>|<span data-ttu-id="32137-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="32137-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="32137-121">Accept</span><span class="sxs-lookup"><span data-stu-id="32137-121">Accept</span></span>|<span data-ttu-id="32137-122">application/json</span><span class="sxs-lookup"><span data-stu-id="32137-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32137-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="32137-123">Request body</span></span>
<span data-ttu-id="32137-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10MobileCompliancePolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="32137-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="32137-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10MobileCompliancePolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="32137-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="32137-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="32137-126">Property</span></span>|<span data-ttu-id="32137-127">Typ</span><span class="sxs-lookup"><span data-stu-id="32137-127">Type</span></span>|<span data-ttu-id="32137-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32137-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32137-129">id</span><span class="sxs-lookup"><span data-stu-id="32137-129">id</span></span>|<span data-ttu-id="32137-130">String</span><span class="sxs-lookup"><span data-stu-id="32137-130">String</span></span>|<span data-ttu-id="32137-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="32137-131">Key of the setting.</span></span> <span data-ttu-id="32137-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32137-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="32137-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32137-133">createdDateTime</span></span>|<span data-ttu-id="32137-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32137-134">DateTimeOffset</span></span>|<span data-ttu-id="32137-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="32137-135">DateTime the object was created.</span></span> <span data-ttu-id="32137-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32137-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="32137-137">description</span><span class="sxs-lookup"><span data-stu-id="32137-137">description</span></span>|<span data-ttu-id="32137-138">String</span><span class="sxs-lookup"><span data-stu-id="32137-138">String</span></span>|<span data-ttu-id="32137-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="32137-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="32137-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32137-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="32137-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32137-141">lastModifiedDateTime</span></span>|<span data-ttu-id="32137-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32137-142">DateTimeOffset</span></span>|<span data-ttu-id="32137-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="32137-143">Indicates the date the object was last modified.</span></span> <span data-ttu-id="32137-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32137-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="32137-145">displayName</span><span class="sxs-lookup"><span data-stu-id="32137-145">displayName</span></span>|<span data-ttu-id="32137-146">String</span><span class="sxs-lookup"><span data-stu-id="32137-146">String</span></span>|<span data-ttu-id="32137-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="32137-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="32137-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32137-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="32137-149">version</span><span class="sxs-lookup"><span data-stu-id="32137-149">version</span></span>|<span data-ttu-id="32137-150">Int32</span><span class="sxs-lookup"><span data-stu-id="32137-150">Int32</span></span>|<span data-ttu-id="32137-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="32137-151">Version of the device configuration.</span></span> <span data-ttu-id="32137-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="32137-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="32137-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="32137-153">passwordRequired</span></span>|<span data-ttu-id="32137-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="32137-154">Boolean</span></span>|<span data-ttu-id="32137-155">Legt fest, dass zum Entsperren des Windows Phone-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="32137-155">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="32137-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="32137-156">passwordBlockSimple</span></span>|<span data-ttu-id="32137-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="32137-157">Boolean</span></span>|<span data-ttu-id="32137-158">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="32137-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="32137-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="32137-159">passwordMinimumLength</span></span>|<span data-ttu-id="32137-160">Int32</span><span class="sxs-lookup"><span data-stu-id="32137-160">Int32</span></span>|<span data-ttu-id="32137-161">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="32137-161">Minimum password length.</span></span> <span data-ttu-id="32137-162">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="32137-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="32137-163">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="32137-163">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="32137-164">Int32</span><span class="sxs-lookup"><span data-stu-id="32137-164">Int32</span></span>|<span data-ttu-id="32137-165">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="32137-165">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="32137-166">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="32137-166">passwordRequiredType</span></span>|<span data-ttu-id="32137-167">String</span><span class="sxs-lookup"><span data-stu-id="32137-167">String</span></span>|<span data-ttu-id="32137-168">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="32137-168">The required password type.</span></span> <span data-ttu-id="32137-169">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="32137-169">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="32137-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="32137-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="32137-171">Int32</span><span class="sxs-lookup"><span data-stu-id="32137-171">Int32</span></span>|<span data-ttu-id="32137-172">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="32137-172">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="32137-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="32137-173">passwordExpirationDays</span></span>|<span data-ttu-id="32137-174">Int32</span><span class="sxs-lookup"><span data-stu-id="32137-174">Int32</span></span>|<span data-ttu-id="32137-175">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="32137-175">Number of days before password expiration.</span></span> <span data-ttu-id="32137-176">Gültige Werte: 1 bis 255.</span><span class="sxs-lookup"><span data-stu-id="32137-176">Valid values 1 to 255</span></span>|
|<span data-ttu-id="32137-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="32137-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="32137-178">Int32</span><span class="sxs-lookup"><span data-stu-id="32137-178">Int32</span></span>|<span data-ttu-id="32137-179">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="32137-179">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="32137-180">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="32137-180">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="32137-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="32137-181">Boolean</span></span>|<span data-ttu-id="32137-182">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="32137-182">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="32137-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="32137-183">osMinimumVersion</span></span>|<span data-ttu-id="32137-184">String</span><span class="sxs-lookup"><span data-stu-id="32137-184">String</span></span>|<span data-ttu-id="32137-185">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="32137-185">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="32137-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="32137-186">osMaximumVersion</span></span>|<span data-ttu-id="32137-187">String</span><span class="sxs-lookup"><span data-stu-id="32137-187">String</span></span>|<span data-ttu-id="32137-188">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="32137-188">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="32137-189">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="32137-189">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="32137-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="32137-190">Boolean</span></span>|<span data-ttu-id="32137-191">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="32137-191">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="32137-192">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="32137-192">bitLockerEnabled</span></span>|<span data-ttu-id="32137-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="32137-193">Boolean</span></span>|<span data-ttu-id="32137-194">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="32137-194">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="32137-195">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="32137-195">secureBootEnabled</span></span>|<span data-ttu-id="32137-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="32137-196">Boolean</span></span>|<span data-ttu-id="32137-197">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="32137-197">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="32137-198">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="32137-198">codeIntegrityEnabled</span></span>|<span data-ttu-id="32137-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="32137-199">Boolean</span></span>|<span data-ttu-id="32137-200">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="32137-200">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="32137-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="32137-201">storageRequireEncryption</span></span>|<span data-ttu-id="32137-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="32137-202">Boolean</span></span>|<span data-ttu-id="32137-203">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="32137-203">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="32137-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="32137-204">Response</span></span>
<span data-ttu-id="32137-205">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="32137-205">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32137-206">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32137-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="32137-207">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32137-207">Request</span></span>
<span data-ttu-id="32137-208">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="32137-208">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="32137-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="32137-209">Response</span></span>
<span data-ttu-id="32137-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32137-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



