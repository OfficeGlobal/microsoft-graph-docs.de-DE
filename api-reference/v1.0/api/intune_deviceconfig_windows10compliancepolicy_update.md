# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="de007-101">windows10CompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="de007-101">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="de007-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="de007-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de007-103">Aktualisiert die Eigenschaften von Objekten des Typs [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de007-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de007-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="de007-104">Prerequisites</span></span>
<span data-ttu-id="de007-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="de007-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="de007-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="de007-107">Permission type</span></span>|<span data-ttu-id="de007-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="de007-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de007-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="de007-109">Delegated (work or school account)</span></span>|<span data-ttu-id="de007-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de007-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de007-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="de007-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de007-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de007-112">Not supported.</span></span>|
|<span data-ttu-id="de007-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="de007-113">Application</span></span>|<span data-ttu-id="de007-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="de007-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de007-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="de007-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="de007-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="de007-116">Request headers</span></span>
|<span data-ttu-id="de007-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="de007-117">Header</span></span>|<span data-ttu-id="de007-118">Wert</span><span class="sxs-lookup"><span data-stu-id="de007-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de007-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="de007-119">Authorization</span></span>|<span data-ttu-id="de007-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="de007-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="de007-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="de007-121">Accept</span></span>|<span data-ttu-id="de007-122">application/json</span><span class="sxs-lookup"><span data-stu-id="de007-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de007-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="de007-123">Request body</span></span>
<span data-ttu-id="de007-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="de007-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="de007-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="de007-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="de007-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="de007-126">Property</span></span>|<span data-ttu-id="de007-127">Typ</span><span class="sxs-lookup"><span data-stu-id="de007-127">Type</span></span>|<span data-ttu-id="de007-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de007-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de007-129">id</span><span class="sxs-lookup"><span data-stu-id="de007-129">id</span></span>|<span data-ttu-id="de007-130">String</span><span class="sxs-lookup"><span data-stu-id="de007-130">String</span></span>|<span data-ttu-id="de007-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="de007-131">Key of the setting.</span></span> <span data-ttu-id="de007-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de007-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="de007-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de007-133">createdDateTime</span></span>|<span data-ttu-id="de007-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de007-134">DateTimeOffset</span></span>|<span data-ttu-id="de007-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="de007-135">DateTime the object was created.</span></span> <span data-ttu-id="de007-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de007-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="de007-137">description</span><span class="sxs-lookup"><span data-stu-id="de007-137">description</span></span>|<span data-ttu-id="de007-138">String</span><span class="sxs-lookup"><span data-stu-id="de007-138">String</span></span>|<span data-ttu-id="de007-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="de007-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="de007-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de007-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="de007-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de007-141">lastModifiedDateTime</span></span>|<span data-ttu-id="de007-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de007-142">DateTimeOffset</span></span>|<span data-ttu-id="de007-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="de007-143">Indicates the date the object was last modified.</span></span> <span data-ttu-id="de007-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de007-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="de007-145">displayName</span><span class="sxs-lookup"><span data-stu-id="de007-145">displayName</span></span>|<span data-ttu-id="de007-146">String</span><span class="sxs-lookup"><span data-stu-id="de007-146">String</span></span>|<span data-ttu-id="de007-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="de007-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="de007-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de007-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="de007-149">Version</span><span class="sxs-lookup"><span data-stu-id="de007-149">version</span></span>|<span data-ttu-id="de007-150">Int32</span><span class="sxs-lookup"><span data-stu-id="de007-150">Int32</span></span>|<span data-ttu-id="de007-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="de007-151">Version of the device configuration.</span></span> <span data-ttu-id="de007-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="de007-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="de007-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="de007-153">passwordRequired</span></span>|<span data-ttu-id="de007-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="de007-154">Boolean</span></span>|<span data-ttu-id="de007-155">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="de007-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="de007-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="de007-156">passwordBlockSimple</span></span>|<span data-ttu-id="de007-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="de007-157">Boolean</span></span>|<span data-ttu-id="de007-158">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="de007-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="de007-159">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="de007-159">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="de007-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="de007-160">Boolean</span></span>|<span data-ttu-id="de007-161">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="de007-161">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="de007-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="de007-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="de007-163">Int32</span><span class="sxs-lookup"><span data-stu-id="de007-163">Int32</span></span>|<span data-ttu-id="de007-164">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="de007-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="de007-165">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="de007-165">passwordExpirationDays</span></span>|<span data-ttu-id="de007-166">Int32</span><span class="sxs-lookup"><span data-stu-id="de007-166">Int32</span></span>|<span data-ttu-id="de007-167">Zeitraum in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="de007-167">The password expiration in days.</span></span>|
|<span data-ttu-id="de007-168">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="de007-168">passwordMinimumLength</span></span>|<span data-ttu-id="de007-169">Int32</span><span class="sxs-lookup"><span data-stu-id="de007-169">Int32</span></span>|<span data-ttu-id="de007-170">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="de007-170">The minimum password length.</span></span>|
|<span data-ttu-id="de007-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="de007-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="de007-172">Int32</span><span class="sxs-lookup"><span data-stu-id="de007-172">Int32</span></span>|<span data-ttu-id="de007-173">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="de007-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="de007-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="de007-174">passwordRequiredType</span></span>|<span data-ttu-id="de007-175">String</span><span class="sxs-lookup"><span data-stu-id="de007-175">String</span></span>|<span data-ttu-id="de007-176">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="de007-176">The required password type.</span></span> <span data-ttu-id="de007-177">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="de007-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="de007-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="de007-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="de007-179">Int32</span><span class="sxs-lookup"><span data-stu-id="de007-179">Int32</span></span>|<span data-ttu-id="de007-180">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="de007-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="de007-181">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="de007-181">requireHealthyDeviceReport</span></span>|<span data-ttu-id="de007-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="de007-182">Boolean</span></span>|<span data-ttu-id="de007-183">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="de007-183">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="de007-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="de007-184">osMinimumVersion</span></span>|<span data-ttu-id="de007-185">String</span><span class="sxs-lookup"><span data-stu-id="de007-185">String</span></span>|<span data-ttu-id="de007-186">Mindestversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="de007-186">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="de007-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="de007-187">osMaximumVersion</span></span>|<span data-ttu-id="de007-188">String</span><span class="sxs-lookup"><span data-stu-id="de007-188">String</span></span>|<span data-ttu-id="de007-189">Maximalversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="de007-189">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="de007-190">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="de007-190">mobileOsMinimumVersion</span></span>|<span data-ttu-id="de007-191">String</span><span class="sxs-lookup"><span data-stu-id="de007-191">String</span></span>|<span data-ttu-id="de007-192">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="de007-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="de007-193">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="de007-193">mobileOsMaximumVersion</span></span>|<span data-ttu-id="de007-194">String</span><span class="sxs-lookup"><span data-stu-id="de007-194">String</span></span>|<span data-ttu-id="de007-195">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="de007-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="de007-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="de007-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="de007-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="de007-197">Boolean</span></span>|<span data-ttu-id="de007-198">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="de007-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="de007-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="de007-199">bitLockerEnabled</span></span>|<span data-ttu-id="de007-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="de007-200">Boolean</span></span>|<span data-ttu-id="de007-201">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="de007-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="de007-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="de007-202">secureBootEnabled</span></span>|<span data-ttu-id="de007-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="de007-203">Boolean</span></span>|<span data-ttu-id="de007-204">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="de007-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="de007-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="de007-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="de007-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="de007-206">Boolean</span></span>|<span data-ttu-id="de007-207">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="de007-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="de007-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="de007-208">storageRequireEncryption</span></span>|<span data-ttu-id="de007-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="de007-209">Boolean</span></span>|<span data-ttu-id="de007-210">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="de007-210">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="de007-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="de007-211">Response</span></span>
<span data-ttu-id="de007-212">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de007-212">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de007-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de007-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="de007-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="de007-214">Request</span></span>
<span data-ttu-id="de007-215">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="de007-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 954

{
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="de007-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="de007-216">Response</span></span>
<span data-ttu-id="de007-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de007-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```



