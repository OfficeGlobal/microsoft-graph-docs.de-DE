# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="8d744-101">windows10CompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="8d744-101">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="8d744-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8d744-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d744-103">Erstellt neue Objekte des Typs [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8d744-103">Create a new [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d744-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8d744-104">Prerequisites</span></span>
<span data-ttu-id="8d744-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8d744-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8d744-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8d744-107">Permission type</span></span>|<span data-ttu-id="8d744-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8d744-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d744-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8d744-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8d744-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d744-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d744-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8d744-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d744-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d744-112">Not supported.</span></span>|
|<span data-ttu-id="8d744-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8d744-113">Application</span></span>|<span data-ttu-id="8d744-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8d744-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d744-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d744-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="8d744-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8d744-116">Request headers</span></span>
|<span data-ttu-id="8d744-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8d744-117">Header</span></span>|<span data-ttu-id="8d744-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8d744-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d744-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8d744-119">Authorization</span></span>|<span data-ttu-id="8d744-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8d744-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d744-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="8d744-121">Accept</span></span>|<span data-ttu-id="8d744-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="8d744-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d744-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8d744-123">Request body</span></span>
<span data-ttu-id="8d744-124">Geben Sie im Anforderungstext eine JSON-Darstellung des windows10CompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8d744-124">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="8d744-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10CompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8d744-125">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="8d744-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8d744-126">Property</span></span>|<span data-ttu-id="8d744-127">Typ</span><span class="sxs-lookup"><span data-stu-id="8d744-127">Type</span></span>|<span data-ttu-id="8d744-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d744-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d744-129">id</span><span class="sxs-lookup"><span data-stu-id="8d744-129">id</span></span>|<span data-ttu-id="8d744-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d744-130">String</span></span>|<span data-ttu-id="8d744-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8d744-131">Key of the entity.</span></span> <span data-ttu-id="8d744-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8d744-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8d744-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d744-133">createdDateTime</span></span>|<span data-ttu-id="8d744-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d744-134">DateTimeOffset</span></span>|<span data-ttu-id="8d744-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8d744-135">DateTime the object was created.</span></span> <span data-ttu-id="8d744-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8d744-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8d744-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d744-137">description</span></span>|<span data-ttu-id="8d744-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d744-138">String</span></span>|<span data-ttu-id="8d744-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8d744-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8d744-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8d744-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8d744-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d744-141">lastModifiedDateTime</span></span>|<span data-ttu-id="8d744-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d744-142">DateTimeOffset</span></span>|<span data-ttu-id="8d744-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8d744-143">DateTime the object was last modified.</span></span> <span data-ttu-id="8d744-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8d744-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8d744-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8d744-145">displayName</span></span>|<span data-ttu-id="8d744-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d744-146">String</span></span>|<span data-ttu-id="8d744-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8d744-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8d744-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8d744-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8d744-149">Version</span><span class="sxs-lookup"><span data-stu-id="8d744-149">version</span></span>|<span data-ttu-id="8d744-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8d744-150">Int32</span></span>|<span data-ttu-id="8d744-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8d744-151">Version of the device configuration.</span></span> <span data-ttu-id="8d744-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8d744-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8d744-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8d744-153">passwordRequired</span></span>|<span data-ttu-id="8d744-154">boolesch</span><span class="sxs-lookup"><span data-stu-id="8d744-154">Boolean</span></span>|<span data-ttu-id="8d744-155">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="8d744-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="8d744-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8d744-156">passwordBlockSimple</span></span>|<span data-ttu-id="8d744-157">boolesch</span><span class="sxs-lookup"><span data-stu-id="8d744-157">Boolean</span></span>|<span data-ttu-id="8d744-158">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="8d744-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="8d744-159">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="8d744-159">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="8d744-160">boolesch</span><span class="sxs-lookup"><span data-stu-id="8d744-160">Boolean</span></span>|<span data-ttu-id="8d744-161">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="8d744-161">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="8d744-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8d744-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8d744-163">Int32</span><span class="sxs-lookup"><span data-stu-id="8d744-163">Int32</span></span>|<span data-ttu-id="8d744-164">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="8d744-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="8d744-165">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8d744-165">passwordExpirationDays</span></span>|<span data-ttu-id="8d744-166">Int32</span><span class="sxs-lookup"><span data-stu-id="8d744-166">Int32</span></span>|<span data-ttu-id="8d744-167">Zeitraum in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="8d744-167">The password expiration in days.</span></span>|
|<span data-ttu-id="8d744-168">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8d744-168">passwordMinimumLength</span></span>|<span data-ttu-id="8d744-169">Int32</span><span class="sxs-lookup"><span data-stu-id="8d744-169">Int32</span></span>|<span data-ttu-id="8d744-170">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="8d744-170">The minimum password length.</span></span>|
|<span data-ttu-id="8d744-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8d744-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8d744-172">Int32</span><span class="sxs-lookup"><span data-stu-id="8d744-172">Int32</span></span>|<span data-ttu-id="8d744-173">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="8d744-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8d744-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8d744-174">passwordRequiredType</span></span>|[<span data-ttu-id="8d744-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8d744-175">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="8d744-p108">Der erforderliche Kennworttyp. Mögliche Werte: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="8d744-p108">The required password type. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8d744-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8d744-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8d744-179">Int32</span><span class="sxs-lookup"><span data-stu-id="8d744-179">Int32</span></span>|<span data-ttu-id="8d744-180">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="8d744-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="8d744-181">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="8d744-181">requireHealthyDeviceReport</span></span>|<span data-ttu-id="8d744-182">boolesch</span><span class="sxs-lookup"><span data-stu-id="8d744-182">Boolean</span></span>|<span data-ttu-id="8d744-183">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="8d744-183">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="8d744-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8d744-184">osMinimumVersion</span></span>|<span data-ttu-id="8d744-185">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d744-185">String</span></span>|<span data-ttu-id="8d744-186">Mindestversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="8d744-186">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="8d744-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8d744-187">osMaximumVersion</span></span>|<span data-ttu-id="8d744-188">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d744-188">String</span></span>|<span data-ttu-id="8d744-189">Maximalversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="8d744-189">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="8d744-190">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8d744-190">mobileOsMinimumVersion</span></span>|<span data-ttu-id="8d744-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d744-191">String</span></span>|<span data-ttu-id="8d744-192">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="8d744-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="8d744-193">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8d744-193">mobileOsMaximumVersion</span></span>|<span data-ttu-id="8d744-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8d744-194">String</span></span>|<span data-ttu-id="8d744-195">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="8d744-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="8d744-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="8d744-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="8d744-197">boolesch</span><span class="sxs-lookup"><span data-stu-id="8d744-197">Boolean</span></span>|<span data-ttu-id="8d744-198">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="8d744-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="8d744-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="8d744-199">bitLockerEnabled</span></span>|<span data-ttu-id="8d744-200">boolesch</span><span class="sxs-lookup"><span data-stu-id="8d744-200">Boolean</span></span>|<span data-ttu-id="8d744-201">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="8d744-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="8d744-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="8d744-202">secureBootEnabled</span></span>|<span data-ttu-id="8d744-203">boolesch</span><span class="sxs-lookup"><span data-stu-id="8d744-203">Boolean</span></span>|<span data-ttu-id="8d744-204">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="8d744-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="8d744-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="8d744-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="8d744-206">boolesch</span><span class="sxs-lookup"><span data-stu-id="8d744-206">Boolean</span></span>|<span data-ttu-id="8d744-207">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="8d744-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="8d744-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="8d744-208">storageRequireEncryption</span></span>|<span data-ttu-id="8d744-209">boolesch</span><span class="sxs-lookup"><span data-stu-id="8d744-209">Boolean</span></span>|<span data-ttu-id="8d744-210">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="8d744-210">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="8d744-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d744-211">Response</span></span>
<span data-ttu-id="8d744-212">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d744-212">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d744-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8d744-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d744-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8d744-214">Request</span></span>
<span data-ttu-id="8d744-215">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8d744-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1018

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="8d744-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="8d744-216">Response</span></span>
<span data-ttu-id="8d744-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8d744-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








