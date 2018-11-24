# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="b500b-101">windows81CompliancePolicy aktualsieren</span><span class="sxs-lookup"><span data-stu-id="b500b-101">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="b500b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b500b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b500b-103">Aktualisiert die Eigenschaften von Objekten des Typs [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b500b-103">Update the properties of a [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b500b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b500b-104">Prerequisites</span></span>
<span data-ttu-id="b500b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b500b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b500b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b500b-107">Permission type</span></span>|<span data-ttu-id="b500b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b500b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b500b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b500b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b500b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b500b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b500b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b500b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b500b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b500b-112">Not supported.</span></span>|
|<span data-ttu-id="b500b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b500b-113">Application</span></span>|<span data-ttu-id="b500b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b500b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b500b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b500b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b500b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b500b-116">Request headers</span></span>
|<span data-ttu-id="b500b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b500b-117">Header</span></span>|<span data-ttu-id="b500b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="b500b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b500b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b500b-119">Authorization</span></span>|<span data-ttu-id="b500b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b500b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b500b-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b500b-121">Accept</span></span>|<span data-ttu-id="b500b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b500b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b500b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b500b-123">Request body</span></span>
<span data-ttu-id="b500b-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b500b-124">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="b500b-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b500b-125">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="b500b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b500b-126">Property</span></span>|<span data-ttu-id="b500b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="b500b-127">Type</span></span>|<span data-ttu-id="b500b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b500b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b500b-129">id</span><span class="sxs-lookup"><span data-stu-id="b500b-129">id</span></span>|<span data-ttu-id="b500b-130">String</span><span class="sxs-lookup"><span data-stu-id="b500b-130">String</span></span>|<span data-ttu-id="b500b-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="b500b-131">Key of the entity.</span></span> <span data-ttu-id="b500b-132">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b500b-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b500b-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b500b-133">createdDateTime</span></span>|<span data-ttu-id="b500b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b500b-134">DateTimeOffset</span></span>|<span data-ttu-id="b500b-135">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b500b-135">DateTime the object was created.</span></span> <span data-ttu-id="b500b-136">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b500b-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b500b-137">description</span><span class="sxs-lookup"><span data-stu-id="b500b-137">description</span></span>|<span data-ttu-id="b500b-138">String</span><span class="sxs-lookup"><span data-stu-id="b500b-138">String</span></span>|<span data-ttu-id="b500b-139">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b500b-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b500b-140">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b500b-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b500b-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b500b-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b500b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b500b-142">DateTimeOffset</span></span>|<span data-ttu-id="b500b-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b500b-143">DateTime the object was last modified.</span></span> <span data-ttu-id="b500b-144">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b500b-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b500b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b500b-145">displayName</span></span>|<span data-ttu-id="b500b-146">String</span><span class="sxs-lookup"><span data-stu-id="b500b-146">String</span></span>|<span data-ttu-id="b500b-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b500b-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b500b-148">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b500b-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b500b-149">Version</span><span class="sxs-lookup"><span data-stu-id="b500b-149">version</span></span>|<span data-ttu-id="b500b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b500b-150">Int32</span></span>|<span data-ttu-id="b500b-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b500b-151">Version of the device configuration.</span></span> <span data-ttu-id="b500b-152">Geerbt von [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b500b-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b500b-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b500b-153">passwordRequired</span></span>|<span data-ttu-id="b500b-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="b500b-154">Boolean</span></span>|<span data-ttu-id="b500b-155">Legt fest, dass zum Entsperren des Windows-Geräts ein Kennwort erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="b500b-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="b500b-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b500b-156">passwordBlockSimple</span></span>|<span data-ttu-id="b500b-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="b500b-157">Boolean</span></span>|<span data-ttu-id="b500b-158">Gibt an, ob einfache Kennwörter erlaubt sind.</span><span class="sxs-lookup"><span data-stu-id="b500b-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="b500b-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b500b-159">passwordExpirationDays</span></span>|<span data-ttu-id="b500b-160">Int32</span><span class="sxs-lookup"><span data-stu-id="b500b-160">Int32</span></span>|<span data-ttu-id="b500b-161">Zeit bis zum Ablaufen des Kennworts in Tagen</span><span class="sxs-lookup"><span data-stu-id="b500b-161">Password expiration in days.</span></span>|
|<span data-ttu-id="b500b-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b500b-162">passwordMinimumLength</span></span>|<span data-ttu-id="b500b-163">Int32</span><span class="sxs-lookup"><span data-stu-id="b500b-163">Int32</span></span>|<span data-ttu-id="b500b-164">Mindestlänge des Kennworts</span><span class="sxs-lookup"><span data-stu-id="b500b-164">The minimum password length.</span></span>|
|<span data-ttu-id="b500b-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b500b-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b500b-166">Int32</span><span class="sxs-lookup"><span data-stu-id="b500b-166">Int32</span></span>|<span data-ttu-id="b500b-167">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="b500b-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b500b-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b500b-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b500b-169">Int32</span><span class="sxs-lookup"><span data-stu-id="b500b-169">Int32</span></span>|<span data-ttu-id="b500b-170">Anzahl der Zeichensätze, die im Kennwort enthalten sein müssen</span><span class="sxs-lookup"><span data-stu-id="b500b-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b500b-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b500b-171">passwordRequiredType</span></span>|[<span data-ttu-id="b500b-172">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b500b-172">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="b500b-173">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="b500b-173">The required password type.</span></span> <span data-ttu-id="b500b-174">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b500b-174">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b500b-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b500b-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b500b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b500b-176">Int32</span></span>|<span data-ttu-id="b500b-177">Grenze für die Wiederverwendung von Kennwörtern. Der festgelegte Wert gibt an, von wie vielen der zuletzt genutzten Kennwörter sich das Kennwort unterscheiden muss.</span><span class="sxs-lookup"><span data-stu-id="b500b-177">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="b500b-178">Gültige Werte: 0 bis 24.</span><span class="sxs-lookup"><span data-stu-id="b500b-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b500b-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b500b-179">osMinimumVersion</span></span>|<span data-ttu-id="b500b-180">String</span><span class="sxs-lookup"><span data-stu-id="b500b-180">String</span></span>|<span data-ttu-id="b500b-181">Mindestversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="b500b-181">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="b500b-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b500b-182">osMaximumVersion</span></span>|<span data-ttu-id="b500b-183">String</span><span class="sxs-lookup"><span data-stu-id="b500b-183">String</span></span>|<span data-ttu-id="b500b-184">Maximalversion von Windows 8.1</span><span class="sxs-lookup"><span data-stu-id="b500b-184">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="b500b-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b500b-185">storageRequireEncryption</span></span>|<span data-ttu-id="b500b-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="b500b-186">Boolean</span></span>|<span data-ttu-id="b500b-187">Gibt an, ob für ein Windows 8.1-Gerät Verschlüsselung gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="b500b-187">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="b500b-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="b500b-188">Response</span></span>
<span data-ttu-id="b500b-189">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte  [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b500b-189">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b500b-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b500b-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="b500b-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b500b-191">Request</span></span>
<span data-ttu-id="b500b-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b500b-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="b500b-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="b500b-193">Response</span></span>
<span data-ttu-id="b500b-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b500b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



