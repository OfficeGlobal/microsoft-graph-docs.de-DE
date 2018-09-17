# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="7f18c-101">windows10MobileCompliancePolicy aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7f18c-101">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="7f18c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7f18c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f18c-103">Aktualisiert die Eigenschaften von Objekten des Typs [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7f18c-103">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f18c-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7f18c-104">Prerequisites</span></span>
<span data-ttu-id="7f18c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7f18c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7f18c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f18c-107">Permission type</span></span>|<span data-ttu-id="7f18c-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f18c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f18c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f18c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7f18c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f18c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f18c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f18c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f18c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f18c-112">Not supported.</span></span>|
|<span data-ttu-id="7f18c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f18c-113">Application</span></span>|<span data-ttu-id="7f18c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f18c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f18c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f18c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="7f18c-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7f18c-116">Request headers</span></span>
|<span data-ttu-id="7f18c-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7f18c-117">Header</span></span>|<span data-ttu-id="7f18c-118">Wert</span><span class="sxs-lookup"><span data-stu-id="7f18c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f18c-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7f18c-119">Authorization</span></span>|<span data-ttu-id="7f18c-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7f18c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f18c-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="7f18c-121">Accept</span></span>|<span data-ttu-id="7f18c-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="7f18c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f18c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7f18c-123">Request body</span></span>
<span data-ttu-id="7f18c-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7f18c-124">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="7f18c-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="7f18c-125">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="7f18c-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7f18c-126">Property</span></span>|<span data-ttu-id="7f18c-127">Typ</span><span class="sxs-lookup"><span data-stu-id="7f18c-127">Type</span></span>|<span data-ttu-id="7f18c-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f18c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f18c-129">id</span><span class="sxs-lookup"><span data-stu-id="7f18c-129">id</span></span>|<span data-ttu-id="7f18c-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f18c-130">String</span></span>|<span data-ttu-id="7f18c-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7f18c-131">Key of the entity.</span></span> <span data-ttu-id="7f18c-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7f18c-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7f18c-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f18c-133">createdDateTime</span></span>|<span data-ttu-id="7f18c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f18c-134">DateTimeOffset</span></span>|<span data-ttu-id="7f18c-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7f18c-135">DateTime the object was created.</span></span> <span data-ttu-id="7f18c-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7f18c-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7f18c-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f18c-137">description</span></span>|<span data-ttu-id="7f18c-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f18c-138">String</span></span>|<span data-ttu-id="7f18c-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7f18c-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7f18c-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7f18c-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7f18c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f18c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="7f18c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f18c-142">DateTimeOffset</span></span>|<span data-ttu-id="7f18c-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7f18c-143">DateTime the object was last modified.</span></span> <span data-ttu-id="7f18c-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7f18c-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7f18c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7f18c-145">displayName</span></span>|<span data-ttu-id="7f18c-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f18c-146">String</span></span>|<span data-ttu-id="7f18c-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7f18c-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7f18c-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7f18c-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7f18c-149">Version</span><span class="sxs-lookup"><span data-stu-id="7f18c-149">version</span></span>|<span data-ttu-id="7f18c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7f18c-150">Int32</span></span>|<span data-ttu-id="7f18c-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="7f18c-151">Version of the device configuration.</span></span> <span data-ttu-id="7f18c-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7f18c-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7f18c-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7f18c-153">passwordRequired</span></span>|<span data-ttu-id="7f18c-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7f18c-154">Boolean</span></span>|<span data-ttu-id="7f18c-155">Legt fest, dass zum Entsperren des Windows Phone-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="7f18c-155">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="7f18c-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7f18c-156">passwordBlockSimple</span></span>|<span data-ttu-id="7f18c-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7f18c-157">Boolean</span></span>|<span data-ttu-id="7f18c-158">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="7f18c-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="7f18c-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7f18c-159">passwordMinimumLength</span></span>|<span data-ttu-id="7f18c-160">Int32</span><span class="sxs-lookup"><span data-stu-id="7f18c-160">Int32</span></span>|<span data-ttu-id="7f18c-161">Mindestlänge des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="7f18c-161">Minimum password length.</span></span> <span data-ttu-id="7f18c-162">Gültige Werte: 4 bis 16.</span><span class="sxs-lookup"><span data-stu-id="7f18c-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="7f18c-163">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7f18c-163">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="7f18c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7f18c-164">Int32</span></span>|<span data-ttu-id="7f18c-165">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="7f18c-165">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="7f18c-166">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7f18c-166">passwordRequiredType</span></span>|[<span data-ttu-id="7f18c-167">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7f18c-167">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="7f18c-p109">Der erforderliche Kennworttyp. Mögliche Werte: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="7f18c-p109">The required password type. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7f18c-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7f18c-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7f18c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="7f18c-171">Int32</span></span>|<span data-ttu-id="7f18c-172">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="7f18c-172">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="7f18c-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7f18c-173">passwordExpirationDays</span></span>|<span data-ttu-id="7f18c-174">Int32</span><span class="sxs-lookup"><span data-stu-id="7f18c-174">Int32</span></span>|<span data-ttu-id="7f18c-175">Zeit in Tagen bis zum Ablaufen des Kennworts.</span><span class="sxs-lookup"><span data-stu-id="7f18c-175">Number of days before password expiration.</span></span> <span data-ttu-id="7f18c-176">Gültige Werte: 1 bis 255.</span><span class="sxs-lookup"><span data-stu-id="7f18c-176">Valid values 1 to 255</span></span>|
|<span data-ttu-id="7f18c-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7f18c-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7f18c-178">Int32</span><span class="sxs-lookup"><span data-stu-id="7f18c-178">Int32</span></span>|<span data-ttu-id="7f18c-179">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="7f18c-179">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7f18c-180">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="7f18c-180">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="7f18c-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7f18c-181">Boolean</span></span>|<span data-ttu-id="7f18c-182">Legt fest, dass zum Entsperren eines im Leerlauf laufenden Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="7f18c-182">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="7f18c-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7f18c-183">osMinimumVersion</span></span>|<span data-ttu-id="7f18c-184">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f18c-184">String</span></span>|<span data-ttu-id="7f18c-185">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="7f18c-185">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="7f18c-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7f18c-186">osMaximumVersion</span></span>|<span data-ttu-id="7f18c-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7f18c-187">String</span></span>|<span data-ttu-id="7f18c-188">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="7f18c-188">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="7f18c-189">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="7f18c-189">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="7f18c-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7f18c-190">Boolean</span></span>|<span data-ttu-id="7f18c-191">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Der Treiber für Antischadsoftware-Frühstart ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="7f18c-191">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="7f18c-192">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="7f18c-192">bitLockerEnabled</span></span>|<span data-ttu-id="7f18c-193">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7f18c-193">Boolean</span></span>|<span data-ttu-id="7f18c-194">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: BitLocker ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="7f18c-194">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="7f18c-195">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="7f18c-195">secureBootEnabled</span></span>|<span data-ttu-id="7f18c-196">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7f18c-196">Boolean</span></span>|<span data-ttu-id="7f18c-197">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss: Die Option „Sicherer Start“ ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="7f18c-197">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="7f18c-198">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="7f18c-198">codeIntegrityEnabled</span></span>|<span data-ttu-id="7f18c-199">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7f18c-199">Boolean</span></span>|<span data-ttu-id="7f18c-200">Legt fest, dass die Integrität von Geräten durch den Windows-Integritätsnachweis für Geräte bestätigt werden muss.</span><span class="sxs-lookup"><span data-stu-id="7f18c-200">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="7f18c-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7f18c-201">storageRequireEncryption</span></span>|<span data-ttu-id="7f18c-202">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7f18c-202">Boolean</span></span>|<span data-ttu-id="7f18c-203">Legt fest, dass auf Windows-Geräten Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="7f18c-203">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="7f18c-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f18c-204">Response</span></span>
<span data-ttu-id="7f18c-205">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7f18c-205">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f18c-206">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f18c-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f18c-207">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f18c-207">Request</span></span>
<span data-ttu-id="7f18c-208">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7f18c-208">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 786

{
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

### <a name="response"></a><span data-ttu-id="7f18c-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f18c-209">Response</span></span>
<span data-ttu-id="7f18c-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f18c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








