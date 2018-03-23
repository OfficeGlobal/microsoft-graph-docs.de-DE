# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="31e1e-101">windowsPhone81CompliancePolicy erstellen</span><span class="sxs-lookup"><span data-stu-id="31e1e-101">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="31e1e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="31e1e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31e1e-103">Erstellen eines neuen [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="31e1e-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31e1e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="31e1e-104">Prerequisites</span></span>
<span data-ttu-id="31e1e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="31e1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="31e1e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="31e1e-107">Permission type</span></span>|<span data-ttu-id="31e1e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="31e1e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31e1e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="31e1e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="31e1e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31e1e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31e1e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="31e1e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31e1e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31e1e-112">Not supported.</span></span>|
|<span data-ttu-id="31e1e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="31e1e-113">Application</span></span>|<span data-ttu-id="31e1e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31e1e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31e1e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="31e1e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="31e1e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="31e1e-116">Request headers</span></span>
|<span data-ttu-id="31e1e-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="31e1e-117">Header</span></span>|<span data-ttu-id="31e1e-118">Wert</span><span class="sxs-lookup"><span data-stu-id="31e1e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31e1e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="31e1e-119">Authorization</span></span>|<span data-ttu-id="31e1e-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="31e1e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="31e1e-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="31e1e-121">Accept</span></span>|<span data-ttu-id="31e1e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="31e1e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31e1e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="31e1e-123">Request body</span></span>
<span data-ttu-id="31e1e-124">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsPhone81CompliancePolicy-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="31e1e-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="31e1e-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsPhone81CompliancePolicy erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="31e1e-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="31e1e-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="31e1e-126">Property</span></span>|<span data-ttu-id="31e1e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="31e1e-127">Type</span></span>|<span data-ttu-id="31e1e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31e1e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31e1e-129">id</span><span class="sxs-lookup"><span data-stu-id="31e1e-129">id</span></span>|<span data-ttu-id="31e1e-130">String</span><span class="sxs-lookup"><span data-stu-id="31e1e-130">String</span></span>|<span data-ttu-id="31e1e-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="31e1e-131">Key of the setting.</span></span> <span data-ttu-id="31e1e-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="31e1e-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="31e1e-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31e1e-133">createdDateTime</span></span>|<span data-ttu-id="31e1e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31e1e-134">DateTimeOffset</span></span>|<span data-ttu-id="31e1e-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="31e1e-135">DateTime the object was created.</span></span> <span data-ttu-id="31e1e-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="31e1e-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="31e1e-137">description</span><span class="sxs-lookup"><span data-stu-id="31e1e-137">description</span></span>|<span data-ttu-id="31e1e-138">String</span><span class="sxs-lookup"><span data-stu-id="31e1e-138">String</span></span>|<span data-ttu-id="31e1e-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="31e1e-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="31e1e-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="31e1e-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="31e1e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31e1e-141">lastModifiedDateTime</span></span>|<span data-ttu-id="31e1e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31e1e-142">DateTimeOffset</span></span>|<span data-ttu-id="31e1e-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="31e1e-143">Indicates the date the object was last modified.</span></span> <span data-ttu-id="31e1e-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="31e1e-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="31e1e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="31e1e-145">displayName</span></span>|<span data-ttu-id="31e1e-146">String</span><span class="sxs-lookup"><span data-stu-id="31e1e-146">String</span></span>|<span data-ttu-id="31e1e-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="31e1e-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="31e1e-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="31e1e-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="31e1e-149">Version</span><span class="sxs-lookup"><span data-stu-id="31e1e-149">version</span></span>|<span data-ttu-id="31e1e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="31e1e-150">Int32</span></span>|<span data-ttu-id="31e1e-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="31e1e-151">Version of the device configuration.</span></span> <span data-ttu-id="31e1e-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="31e1e-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="31e1e-153">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="31e1e-153">passwordBlockSimple</span></span>|<span data-ttu-id="31e1e-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="31e1e-154">Boolean</span></span>|<span data-ttu-id="31e1e-155">Gibt an, ob die Kalendersynchronisierung blockiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="31e1e-155">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="31e1e-156">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="31e1e-156">passwordExpirationDays</span></span>|<span data-ttu-id="31e1e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="31e1e-157">Int32</span></span>|<span data-ttu-id="31e1e-158">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="31e1e-158">Number of days before the password expires.</span></span>|
|<span data-ttu-id="31e1e-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="31e1e-159">passwordMinimumLength</span></span>|<span data-ttu-id="31e1e-160">Int32</span><span class="sxs-lookup"><span data-stu-id="31e1e-160">Int32</span></span>|<span data-ttu-id="31e1e-161">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="31e1e-161">Minimum length of passwords.</span></span>|
|<span data-ttu-id="31e1e-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="31e1e-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="31e1e-163">Int32</span><span class="sxs-lookup"><span data-stu-id="31e1e-163">Int32</span></span>|<span data-ttu-id="31e1e-164">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="31e1e-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="31e1e-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="31e1e-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="31e1e-166">Int32</span><span class="sxs-lookup"><span data-stu-id="31e1e-166">Int32</span></span>|<span data-ttu-id="31e1e-167">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="31e1e-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="31e1e-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="31e1e-168">passwordRequiredType</span></span>|<span data-ttu-id="31e1e-169">String</span><span class="sxs-lookup"><span data-stu-id="31e1e-169">String</span></span>|<span data-ttu-id="31e1e-170">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="31e1e-170">The required password type.</span></span> <span data-ttu-id="31e1e-171">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="31e1e-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="31e1e-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="31e1e-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="31e1e-173">Int32</span><span class="sxs-lookup"><span data-stu-id="31e1e-173">Int32</span></span>|<span data-ttu-id="31e1e-174">Anzahl der zuletzt verwendeten Kennwörter, die nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="31e1e-174">Number of previous passwords to block.</span></span> <span data-ttu-id="31e1e-175">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="31e1e-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="31e1e-176">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="31e1e-176">passwordRequired</span></span>|<span data-ttu-id="31e1e-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="31e1e-177">Boolean</span></span>|<span data-ttu-id="31e1e-178">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="31e1e-178">Whether or not to require a password.</span></span>|
|<span data-ttu-id="31e1e-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="31e1e-179">osMinimumVersion</span></span>|<span data-ttu-id="31e1e-180">String</span><span class="sxs-lookup"><span data-stu-id="31e1e-180">String</span></span>|<span data-ttu-id="31e1e-181">Mindestversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="31e1e-181">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="31e1e-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="31e1e-182">osMaximumVersion</span></span>|<span data-ttu-id="31e1e-183">String</span><span class="sxs-lookup"><span data-stu-id="31e1e-183">String</span></span>|<span data-ttu-id="31e1e-184">Maximalversion von Windows Phone</span><span class="sxs-lookup"><span data-stu-id="31e1e-184">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="31e1e-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="31e1e-185">storageRequireEncryption</span></span>|<span data-ttu-id="31e1e-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="31e1e-186">Boolean</span></span>|<span data-ttu-id="31e1e-187">Verschlüsselung auf Windows Phone-Geräten erforderlich</span><span class="sxs-lookup"><span data-stu-id="31e1e-187">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="31e1e-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="31e1e-188">Response</span></span>
<span data-ttu-id="31e1e-189">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="31e1e-189">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31e1e-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="31e1e-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="31e1e-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31e1e-191">Request</span></span>
<span data-ttu-id="31e1e-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="31e1e-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 671

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="31e1e-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="31e1e-193">Response</span></span>
<span data-ttu-id="31e1e-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31e1e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 779

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```



