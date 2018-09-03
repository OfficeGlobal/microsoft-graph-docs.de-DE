# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="6fe6a-101">Erstellen von „windows10MobileCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="6fe6a-101">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="6fe6a-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fe6a-103">Diese Methode erstellt ein neues Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6fe6a-103">Create a new [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6fe6a-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6fe6a-104">Prerequisites</span></span>
<span data-ttu-id="6fe6a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6fe6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6fe6a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6fe6a-107">Permission type</span></span>|<span data-ttu-id="6fe6a-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6fe6a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fe6a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6fe6a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6fe6a-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fe6a-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6fe6a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6fe6a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fe6a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6fe6a-112">Not supported.</span></span>|
|<span data-ttu-id="6fe6a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6fe6a-113">Application</span></span>|<span data-ttu-id="6fe6a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6fe6a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fe6a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6fe6a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6fe6a-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6fe6a-116">Request headers</span></span>
|<span data-ttu-id="6fe6a-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6fe6a-117">Header</span></span>|<span data-ttu-id="6fe6a-118">Wert</span><span class="sxs-lookup"><span data-stu-id="6fe6a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fe6a-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6fe6a-119">Authorization</span></span>|<span data-ttu-id="6fe6a-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6fe6a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fe6a-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="6fe6a-121">Accept</span></span>|<span data-ttu-id="6fe6a-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="6fe6a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fe6a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6fe6a-123">Request body</span></span>
<span data-ttu-id="6fe6a-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows10MobileCompliancePolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-124">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="6fe6a-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows10MobileCompliancePolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-125">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="6fe6a-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6fe6a-126">Property</span></span>|<span data-ttu-id="6fe6a-127">Typ</span><span class="sxs-lookup"><span data-stu-id="6fe6a-127">Type</span></span>|<span data-ttu-id="6fe6a-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6fe6a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fe6a-129">id</span><span class="sxs-lookup"><span data-stu-id="6fe6a-129">id</span></span>|<span data-ttu-id="6fe6a-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6fe6a-130">String</span></span>|<span data-ttu-id="6fe6a-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6fe6a-131">Key of the entity.</span></span> <span data-ttu-id="6fe6a-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6fe6a-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6fe6a-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fe6a-133">createdDateTime</span></span>|<span data-ttu-id="6fe6a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fe6a-134">DateTimeOffset</span></span>|<span data-ttu-id="6fe6a-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-135">DateTime the object was created.</span></span> <span data-ttu-id="6fe6a-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6fe6a-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6fe6a-137">description</span><span class="sxs-lookup"><span data-stu-id="6fe6a-137">description</span></span>|<span data-ttu-id="6fe6a-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6fe6a-138">String</span></span>|<span data-ttu-id="6fe6a-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6fe6a-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6fe6a-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6fe6a-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6fe6a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fe6a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="6fe6a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fe6a-142">DateTimeOffset</span></span>|<span data-ttu-id="6fe6a-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-143">DateTime the object was last modified.</span></span> <span data-ttu-id="6fe6a-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6fe6a-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6fe6a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6fe6a-145">displayName</span></span>|<span data-ttu-id="6fe6a-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6fe6a-146">String</span></span>|<span data-ttu-id="6fe6a-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6fe6a-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6fe6a-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6fe6a-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6fe6a-149">Version</span><span class="sxs-lookup"><span data-stu-id="6fe6a-149">version</span></span>|<span data-ttu-id="6fe6a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6fe6a-150">Int32</span></span>|<span data-ttu-id="6fe6a-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-151">Version of the device configuration.</span></span> <span data-ttu-id="6fe6a-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6fe6a-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6fe6a-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6fe6a-153">passwordRequired</span></span>|<span data-ttu-id="6fe6a-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6fe6a-154">Boolean</span></span>|<span data-ttu-id="6fe6a-155">Legt fest, dass zum Entsperren des Windows Phone-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-155">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="6fe6a-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6fe6a-156">passwordBlockSimple</span></span>|<span data-ttu-id="6fe6a-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6fe6a-157">Boolean</span></span>|<span data-ttu-id="6fe6a-158">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="6fe6a-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6fe6a-159">passwordMinimumLength</span></span>|<span data-ttu-id="6fe6a-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6fe6a-160">Int32</span></span>|<span data-ttu-id="6fe6a-161">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-161">Minimum password length.</span></span> <span data-ttu-id="6fe6a-162">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6fe6a-163">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6fe6a-163">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6fe6a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6fe6a-164">Int32</span></span>|<span data-ttu-id="6fe6a-165">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="6fe6a-165">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6fe6a-166">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6fe6a-166">passwordRequiredType</span></span>|[<span data-ttu-id="6fe6a-167">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6fe6a-167">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="6fe6a-168">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-168">The required password type.</span></span> <span data-ttu-id="6fe6a-169">Die möglichen Werte sind: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-169">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="6fe6a-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6fe6a-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6fe6a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="6fe6a-171">Int32</span></span>|<span data-ttu-id="6fe6a-172">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-172">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="6fe6a-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6fe6a-173">passwordExpirationDays</span></span>|<span data-ttu-id="6fe6a-174">Int32</span><span class="sxs-lookup"><span data-stu-id="6fe6a-174">Int32</span></span>|<span data-ttu-id="6fe6a-175">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-175">Number of days before password expiration.</span></span> <span data-ttu-id="6fe6a-176">Gültige Werte: 1 bis 255.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-176">Valid values 1 to 255</span></span>|
|<span data-ttu-id="6fe6a-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6fe6a-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6fe6a-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6fe6a-178">Int32</span></span>|<span data-ttu-id="6fe6a-179">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="6fe6a-179">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6fe6a-180">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="6fe6a-180">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="6fe6a-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6fe6a-181">Boolean</span></span>|<span data-ttu-id="6fe6a-182">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-182">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="6fe6a-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6fe6a-183">osMinimumVersion</span></span>|<span data-ttu-id="6fe6a-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6fe6a-184">String</span></span>|<span data-ttu-id="6fe6a-185">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="6fe6a-185">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="6fe6a-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6fe6a-186">osMaximumVersion</span></span>|<span data-ttu-id="6fe6a-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6fe6a-187">String</span></span>|<span data-ttu-id="6fe6a-188">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="6fe6a-188">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="6fe6a-189">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="6fe6a-189">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="6fe6a-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6fe6a-190">Boolean</span></span>|<span data-ttu-id="6fe6a-191">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-191">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="6fe6a-192">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="6fe6a-192">bitLockerEnabled</span></span>|<span data-ttu-id="6fe6a-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6fe6a-193">Boolean</span></span>|<span data-ttu-id="6fe6a-194">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-194">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="6fe6a-195">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="6fe6a-195">secureBootEnabled</span></span>|<span data-ttu-id="6fe6a-196">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6fe6a-196">Boolean</span></span>|<span data-ttu-id="6fe6a-197">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-197">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="6fe6a-198">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="6fe6a-198">codeIntegrityEnabled</span></span>|<span data-ttu-id="6fe6a-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6fe6a-199">Boolean</span></span>|<span data-ttu-id="6fe6a-200">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-200">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="6fe6a-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6fe6a-201">storageRequireEncryption</span></span>|<span data-ttu-id="6fe6a-202">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6fe6a-202">Boolean</span></span>|<span data-ttu-id="6fe6a-203">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-203">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="6fe6a-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="6fe6a-204">Response</span></span>
<span data-ttu-id="6fe6a-205">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-205">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fe6a-206">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6fe6a-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="6fe6a-207">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6fe6a-207">Request</span></span>
<span data-ttu-id="6fe6a-208">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-208">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6fe6a-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="6fe6a-209">Response</span></span>
<span data-ttu-id="6fe6a-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6fe6a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



