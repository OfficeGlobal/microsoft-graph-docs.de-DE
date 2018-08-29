# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="8052c-101">windows10CompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8052c-101">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="8052c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8052c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8052c-103">Aktualisiert die Eigenschaften von Objekten des Typs [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8052c-103">Update the properties of a [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8052c-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8052c-104">Prerequisites</span></span>
<span data-ttu-id="8052c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8052c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8052c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8052c-107">Permission type</span></span>|<span data-ttu-id="8052c-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8052c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8052c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8052c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8052c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8052c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8052c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8052c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8052c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8052c-112">Not supported.</span></span>|
|<span data-ttu-id="8052c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8052c-113">Application</span></span>|<span data-ttu-id="8052c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8052c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8052c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8052c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="8052c-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8052c-116">Request headers</span></span>
|<span data-ttu-id="8052c-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8052c-117">Header</span></span>|<span data-ttu-id="8052c-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8052c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8052c-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8052c-119">Authorization</span></span>|<span data-ttu-id="8052c-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8052c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8052c-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="8052c-121">Accept</span></span>|<span data-ttu-id="8052c-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="8052c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8052c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8052c-123">Request body</span></span>
<span data-ttu-id="8052c-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8052c-124">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="8052c-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8052c-125">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="8052c-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8052c-126">Property</span></span>|<span data-ttu-id="8052c-127">Typ</span><span class="sxs-lookup"><span data-stu-id="8052c-127">Type</span></span>|<span data-ttu-id="8052c-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8052c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8052c-129">ID</span><span class="sxs-lookup"><span data-stu-id="8052c-129">id</span></span>|<span data-ttu-id="8052c-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8052c-130">String</span></span>|<span data-ttu-id="8052c-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8052c-131">Key of the entity.</span></span> <span data-ttu-id="8052c-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8052c-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8052c-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8052c-133">createdDateTime</span></span>|<span data-ttu-id="8052c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8052c-134">DateTimeOffset</span></span>|<span data-ttu-id="8052c-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8052c-135">DateTime the object was created.</span></span> <span data-ttu-id="8052c-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8052c-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8052c-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8052c-137">description</span></span>|<span data-ttu-id="8052c-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8052c-138">String</span></span>|<span data-ttu-id="8052c-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8052c-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8052c-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8052c-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8052c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8052c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="8052c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8052c-142">DateTimeOffset</span></span>|<span data-ttu-id="8052c-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8052c-143">DateTime the object was last modified.</span></span> <span data-ttu-id="8052c-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8052c-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8052c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8052c-145">displayName</span></span>|<span data-ttu-id="8052c-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8052c-146">String</span></span>|<span data-ttu-id="8052c-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8052c-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8052c-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8052c-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8052c-149">Version</span><span class="sxs-lookup"><span data-stu-id="8052c-149">version</span></span>|<span data-ttu-id="8052c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8052c-150">Int32</span></span>|<span data-ttu-id="8052c-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="8052c-151">Version of the device configuration.</span></span> <span data-ttu-id="8052c-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8052c-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8052c-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8052c-153">passwordRequired</span></span>|<span data-ttu-id="8052c-154">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8052c-154">Boolean</span></span>|<span data-ttu-id="8052c-155">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="8052c-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="8052c-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8052c-156">passwordBlockSimple</span></span>|<span data-ttu-id="8052c-157">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8052c-157">Boolean</span></span>|<span data-ttu-id="8052c-158">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="8052c-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="8052c-159">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="8052c-159">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="8052c-160">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8052c-160">Boolean</span></span>|<span data-ttu-id="8052c-161">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="8052c-161">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="8052c-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8052c-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8052c-163">Int32</span><span class="sxs-lookup"><span data-stu-id="8052c-163">Int32</span></span>|<span data-ttu-id="8052c-164">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="8052c-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="8052c-165">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8052c-165">passwordExpirationDays</span></span>|<span data-ttu-id="8052c-166">Int32</span><span class="sxs-lookup"><span data-stu-id="8052c-166">Int32</span></span>|<span data-ttu-id="8052c-167">Zeitraum in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="8052c-167">The password expiration in days.</span></span>|
|<span data-ttu-id="8052c-168">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8052c-168">passwordMinimumLength</span></span>|<span data-ttu-id="8052c-169">Int32</span><span class="sxs-lookup"><span data-stu-id="8052c-169">Int32</span></span>|<span data-ttu-id="8052c-170">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="8052c-170">The minimum password length.</span></span>|
|<span data-ttu-id="8052c-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8052c-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8052c-172">Int32</span><span class="sxs-lookup"><span data-stu-id="8052c-172">Int32</span></span>|<span data-ttu-id="8052c-173">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="8052c-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8052c-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8052c-174">passwordRequiredType</span></span>|[<span data-ttu-id="8052c-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8052c-175">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="8052c-176">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="8052c-176">The required password type.</span></span> <span data-ttu-id="8052c-177">Mögliche Werte sind `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="8052c-177">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="8052c-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8052c-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8052c-179">Int32</span><span class="sxs-lookup"><span data-stu-id="8052c-179">Int32</span></span>|<span data-ttu-id="8052c-180">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="8052c-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="8052c-181">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="8052c-181">requireHealthyDeviceReport</span></span>|<span data-ttu-id="8052c-182">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8052c-182">Boolean</span></span>|<span data-ttu-id="8052c-183">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="8052c-183">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="8052c-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8052c-184">osMinimumVersion</span></span>|<span data-ttu-id="8052c-185">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8052c-185">String</span></span>|<span data-ttu-id="8052c-186">Mindestversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="8052c-186">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="8052c-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8052c-187">osMaximumVersion</span></span>|<span data-ttu-id="8052c-188">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8052c-188">String</span></span>|<span data-ttu-id="8052c-189">Maximalversion von Windows 10</span><span class="sxs-lookup"><span data-stu-id="8052c-189">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="8052c-190">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8052c-190">mobileOsMinimumVersion</span></span>|<span data-ttu-id="8052c-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8052c-191">String</span></span>|<span data-ttu-id="8052c-192">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="8052c-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="8052c-193">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8052c-193">mobileOsMaximumVersion</span></span>|<span data-ttu-id="8052c-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8052c-194">String</span></span>|<span data-ttu-id="8052c-195">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="8052c-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="8052c-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="8052c-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="8052c-197">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8052c-197">Boolean</span></span>|<span data-ttu-id="8052c-198">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="8052c-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="8052c-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="8052c-199">bitLockerEnabled</span></span>|<span data-ttu-id="8052c-200">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8052c-200">Boolean</span></span>|<span data-ttu-id="8052c-201">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="8052c-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="8052c-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="8052c-202">secureBootEnabled</span></span>|<span data-ttu-id="8052c-203">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8052c-203">Boolean</span></span>|<span data-ttu-id="8052c-204">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="8052c-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="8052c-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="8052c-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="8052c-206">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8052c-206">Boolean</span></span>|<span data-ttu-id="8052c-207">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="8052c-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="8052c-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="8052c-208">storageRequireEncryption</span></span>|<span data-ttu-id="8052c-209">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8052c-209">Boolean</span></span>|<span data-ttu-id="8052c-210">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="8052c-210">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="8052c-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="8052c-211">Response</span></span>
<span data-ttu-id="8052c-212">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8052c-212">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8052c-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8052c-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="8052c-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8052c-214">Request</span></span>
<span data-ttu-id="8052c-215">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8052c-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8052c-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="8052c-216">Response</span></span>
<span data-ttu-id="8052c-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8052c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



