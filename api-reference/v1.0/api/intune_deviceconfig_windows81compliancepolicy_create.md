# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="e4e77-101">Erstellen von „windows81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="e4e77-101">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="e4e77-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e4e77-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4e77-103">Diese Methode erstellt ein neues Objekt des Typs [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4e77-103">Create a new [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4e77-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e4e77-104">Prerequisites</span></span>
<span data-ttu-id="e4e77-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4e77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e4e77-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4e77-107">Permission type</span></span>|<span data-ttu-id="e4e77-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4e77-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4e77-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4e77-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e4e77-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4e77-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4e77-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4e77-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4e77-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4e77-112">Not supported.</span></span>|
|<span data-ttu-id="e4e77-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4e77-113">Application</span></span>|<span data-ttu-id="e4e77-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4e77-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4e77-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4e77-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e4e77-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4e77-116">Request headers</span></span>
|<span data-ttu-id="e4e77-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e4e77-117">Header</span></span>|<span data-ttu-id="e4e77-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e4e77-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4e77-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e4e77-119">Authorization</span></span>|<span data-ttu-id="e4e77-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e4e77-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4e77-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="e4e77-121">Accept</span></span>|<span data-ttu-id="e4e77-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="e4e77-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4e77-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4e77-123">Request body</span></span>
<span data-ttu-id="e4e77-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windows81CompliancePolicy“ an.</span><span class="sxs-lookup"><span data-stu-id="e4e77-124">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="e4e77-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windows81CompliancePolicy“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="e4e77-125">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="e4e77-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e4e77-126">Property</span></span>|<span data-ttu-id="e4e77-127">Typ</span><span class="sxs-lookup"><span data-stu-id="e4e77-127">Type</span></span>|<span data-ttu-id="e4e77-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4e77-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4e77-129">id</span><span class="sxs-lookup"><span data-stu-id="e4e77-129">id</span></span>|<span data-ttu-id="e4e77-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4e77-130">String</span></span>|<span data-ttu-id="e4e77-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e4e77-131">Key of the entity.</span></span> <span data-ttu-id="e4e77-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4e77-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4e77-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4e77-133">createdDateTime</span></span>|<span data-ttu-id="e4e77-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4e77-134">DateTimeOffset</span></span>|<span data-ttu-id="e4e77-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4e77-135">DateTime the object was created.</span></span> <span data-ttu-id="e4e77-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4e77-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4e77-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4e77-137">description</span></span>|<span data-ttu-id="e4e77-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4e77-138">String</span></span>|<span data-ttu-id="e4e77-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e4e77-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e4e77-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4e77-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4e77-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4e77-141">lastModifiedDateTime</span></span>|<span data-ttu-id="e4e77-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4e77-142">DateTimeOffset</span></span>|<span data-ttu-id="e4e77-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4e77-143">DateTime the object was last modified.</span></span> <span data-ttu-id="e4e77-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4e77-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4e77-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e4e77-145">displayName</span></span>|<span data-ttu-id="e4e77-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4e77-146">String</span></span>|<span data-ttu-id="e4e77-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e4e77-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e4e77-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4e77-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4e77-149">Version</span><span class="sxs-lookup"><span data-stu-id="e4e77-149">version</span></span>|<span data-ttu-id="e4e77-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e4e77-150">Int32</span></span>|<span data-ttu-id="e4e77-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="e4e77-151">Version of the device configuration.</span></span> <span data-ttu-id="e4e77-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e4e77-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e4e77-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e4e77-153">passwordRequired</span></span>|<span data-ttu-id="e4e77-154">boolesch</span><span class="sxs-lookup"><span data-stu-id="e4e77-154">Boolean</span></span>|<span data-ttu-id="e4e77-155">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="e4e77-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="e4e77-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e4e77-156">passwordBlockSimple</span></span>|<span data-ttu-id="e4e77-157">boolesch</span><span class="sxs-lookup"><span data-stu-id="e4e77-157">Boolean</span></span>|<span data-ttu-id="e4e77-158">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="e4e77-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="e4e77-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e4e77-159">passwordExpirationDays</span></span>|<span data-ttu-id="e4e77-160">Int32</span><span class="sxs-lookup"><span data-stu-id="e4e77-160">Int32</span></span>|<span data-ttu-id="e4e77-161">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="e4e77-161">Password expiration in days.</span></span>|
|<span data-ttu-id="e4e77-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e4e77-162">passwordMinimumLength</span></span>|<span data-ttu-id="e4e77-163">Int32</span><span class="sxs-lookup"><span data-stu-id="e4e77-163">Int32</span></span>|<span data-ttu-id="e4e77-164">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="e4e77-164">The minimum password length.</span></span>|
|<span data-ttu-id="e4e77-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e4e77-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e4e77-166">Int32</span><span class="sxs-lookup"><span data-stu-id="e4e77-166">Int32</span></span>|<span data-ttu-id="e4e77-167">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="e4e77-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e4e77-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e4e77-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e4e77-169">Int32</span><span class="sxs-lookup"><span data-stu-id="e4e77-169">Int32</span></span>|<span data-ttu-id="e4e77-170">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="e4e77-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e4e77-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e4e77-171">passwordRequiredType</span></span>|[<span data-ttu-id="e4e77-172">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e4e77-172">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="e4e77-p108">Der erforderliche Kennworttyp. Mögliche Werte: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e4e77-p108">The required password type. The possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e4e77-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e4e77-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e4e77-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e4e77-176">Int32</span></span>|<span data-ttu-id="e4e77-177">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="e4e77-177">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="e4e77-178">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="e4e77-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e4e77-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e4e77-179">osMinimumVersion</span></span>|<span data-ttu-id="e4e77-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4e77-180">String</span></span>|<span data-ttu-id="e4e77-181">Mindestversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="e4e77-181">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="e4e77-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e4e77-182">osMaximumVersion</span></span>|<span data-ttu-id="e4e77-183">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4e77-183">String</span></span>|<span data-ttu-id="e4e77-184">Maximalversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="e4e77-184">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="e4e77-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e4e77-185">storageRequireEncryption</span></span>|<span data-ttu-id="e4e77-186">boolesch</span><span class="sxs-lookup"><span data-stu-id="e4e77-186">Boolean</span></span>|<span data-ttu-id="e4e77-187">Gibt an, ob für ein Windows 8.1-Gerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="e4e77-187">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="e4e77-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4e77-188">Response</span></span>
<span data-ttu-id="e4e77-189">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e4e77-189">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4e77-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4e77-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4e77-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4e77-191">Request</span></span>
<span data-ttu-id="e4e77-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4e77-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 666

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="e4e77-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4e77-193">Response</span></span>
<span data-ttu-id="e4e77-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4e77-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 774

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
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
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```








