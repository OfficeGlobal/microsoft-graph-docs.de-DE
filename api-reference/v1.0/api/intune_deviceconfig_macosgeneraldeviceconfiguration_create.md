# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="3cac0-101">Erstellen von „macOSGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="3cac0-101">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="3cac0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3cac0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cac0-103">Diese Methode erstellt ein neues Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cac0-103">Create a new [plannerBucket](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3cac0-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3cac0-104">Prerequisites</span></span>
<span data-ttu-id="3cac0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3cac0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3cac0-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3cac0-107">Permission type</span></span>|<span data-ttu-id="3cac0-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3cac0-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cac0-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3cac0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3cac0-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cac0-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3cac0-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3cac0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cac0-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3cac0-112">Not supported.</span></span>|
|<span data-ttu-id="3cac0-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3cac0-113">Application</span></span>|<span data-ttu-id="3cac0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3cac0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cac0-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3cac0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3cac0-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3cac0-116">Request headers</span></span>
|<span data-ttu-id="3cac0-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3cac0-117">Header</span></span>|<span data-ttu-id="3cac0-118">Wert</span><span class="sxs-lookup"><span data-stu-id="3cac0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cac0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cac0-119">Authorization</span></span>|<span data-ttu-id="3cac0-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3cac0-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3cac0-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3cac0-121">Accept</span></span>|<span data-ttu-id="3cac0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3cac0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cac0-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3cac0-123">Request body</span></span>
<span data-ttu-id="3cac0-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „macOSGeneralDeviceConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="3cac0-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="3cac0-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSGeneralDeviceConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="3cac0-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="3cac0-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3cac0-126">Property</span></span>|<span data-ttu-id="3cac0-127">Typ</span><span class="sxs-lookup"><span data-stu-id="3cac0-127">Type</span></span>|<span data-ttu-id="3cac0-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3cac0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cac0-129">id</span><span class="sxs-lookup"><span data-stu-id="3cac0-129">id</span></span>|<span data-ttu-id="3cac0-130">String</span><span class="sxs-lookup"><span data-stu-id="3cac0-130">String</span></span>|<span data-ttu-id="3cac0-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="3cac0-131">Key of the setting.</span></span> <span data-ttu-id="3cac0-132">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cac0-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cac0-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cac0-133">lastModifiedDateTime</span></span>|<span data-ttu-id="3cac0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cac0-134">DateTimeOffset</span></span>|<span data-ttu-id="3cac0-135">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3cac0-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="3cac0-136">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cac0-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cac0-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3cac0-137">createdDateTime</span></span>|<span data-ttu-id="3cac0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cac0-138">DateTimeOffset</span></span>|<span data-ttu-id="3cac0-139">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3cac0-139">DateTime the object was created.</span></span> <span data-ttu-id="3cac0-140">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cac0-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cac0-141">description</span><span class="sxs-lookup"><span data-stu-id="3cac0-141">description</span></span>|<span data-ttu-id="3cac0-142">String</span><span class="sxs-lookup"><span data-stu-id="3cac0-142">String</span></span>|<span data-ttu-id="3cac0-143">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3cac0-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3cac0-144">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cac0-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cac0-145">displayName</span><span class="sxs-lookup"><span data-stu-id="3cac0-145">displayName</span></span>|<span data-ttu-id="3cac0-146">String</span><span class="sxs-lookup"><span data-stu-id="3cac0-146">String</span></span>|<span data-ttu-id="3cac0-147">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3cac0-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3cac0-148">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cac0-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cac0-149">version</span><span class="sxs-lookup"><span data-stu-id="3cac0-149">version</span></span>|<span data-ttu-id="3cac0-150">Int32</span><span class="sxs-lookup"><span data-stu-id="3cac0-150">Int32</span></span>|<span data-ttu-id="3cac0-151">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="3cac0-151">Version of the device configuration.</span></span> <span data-ttu-id="3cac0-152">Geerbt von [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cac0-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cac0-153">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="3cac0-153">compliantAppsList</span></span>|<span data-ttu-id="3cac0-154">Collection von Objekten des Typs [appListItem](../resources/intune_deviceconfig_applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3cac0-154">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="3cac0-155">Liste aller Apps, für die die Konformitätsrichtlinie gilt (Zulassungsliste oder Sperrliste, gesteuert über „compliantAppListType“).</span><span class="sxs-lookup"><span data-stu-id="3cac0-155">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="3cac0-156">Diese Collection darf maximal 10.000 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="3cac0-156">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="3cac0-157">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="3cac0-157">compliantAppListType</span></span>|<span data-ttu-id="3cac0-158">String</span><span class="sxs-lookup"><span data-stu-id="3cac0-158">String</span></span>|<span data-ttu-id="3cac0-159">Typ der in „compliantAppsList“ definierten Liste.</span><span class="sxs-lookup"><span data-stu-id="3cac0-159">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="3cac0-160">Mögliche Werte sind: `none`, `appsInListCompliant` und `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="3cac0-160">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="3cac0-161">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="3cac0-161">emailInDomainSuffixes</span></span>|<span data-ttu-id="3cac0-162">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="3cac0-162">String collection</span></span>|<span data-ttu-id="3cac0-163">E-Mail-Adressen, deren Suffix keiner dieser Zeichenfolgen entspricht, gelten als domänenextern.</span><span class="sxs-lookup"><span data-stu-id="3cac0-163">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="3cac0-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3cac0-164">passwordBlockSimple</span></span>|<span data-ttu-id="3cac0-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cac0-165">Boolean</span></span>|<span data-ttu-id="3cac0-166">Unterbindet die Verwendung einfacher Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="3cac0-166">Block simple passwords.</span></span>|
|<span data-ttu-id="3cac0-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3cac0-167">passwordExpirationDays</span></span>|<span data-ttu-id="3cac0-168">Int32</span><span class="sxs-lookup"><span data-stu-id="3cac0-168">Int32</span></span>|<span data-ttu-id="3cac0-169">Zeit in Tagen bis zum Ablaufen des Kennworts</span><span class="sxs-lookup"><span data-stu-id="3cac0-169">Number of days before the password expires.</span></span>|
|<span data-ttu-id="3cac0-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3cac0-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="3cac0-171">Int32</span><span class="sxs-lookup"><span data-stu-id="3cac0-171">Int32</span></span>|<span data-ttu-id="3cac0-172">Anzahl von Zeichensätzen, die ein Kennwort enthalten muss.</span><span class="sxs-lookup"><span data-stu-id="3cac0-172">Number of character sets a password must contain.</span></span> <span data-ttu-id="3cac0-173">Gültige Werte: 0 bis 4.</span><span class="sxs-lookup"><span data-stu-id="3cac0-173">Valid values 0 to 4</span></span>|
|<span data-ttu-id="3cac0-174">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3cac0-174">passwordMinimumLength</span></span>|<span data-ttu-id="3cac0-175">Int32</span><span class="sxs-lookup"><span data-stu-id="3cac0-175">Int32</span></span>|<span data-ttu-id="3cac0-176">Mindestlänge von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="3cac0-176">Minimum length of passwords.</span></span>|
|<span data-ttu-id="3cac0-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3cac0-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3cac0-178">Int32</span><span class="sxs-lookup"><span data-stu-id="3cac0-178">Int32</span></span>|<span data-ttu-id="3cac0-179">Zeitraum von Inaktivität in Minuten, nach dem die Eingabe eines Kennworts gefordert wird</span><span class="sxs-lookup"><span data-stu-id="3cac0-179">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="3cac0-180">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="3cac0-180">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="3cac0-181">Int32</span><span class="sxs-lookup"><span data-stu-id="3cac0-181">Int32</span></span>|<span data-ttu-id="3cac0-182">Zeitraum von Inaktivität in Minuten, nach dem es zu einem Bildschirmtimeout kommt</span><span class="sxs-lookup"><span data-stu-id="3cac0-182">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="3cac0-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3cac0-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3cac0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="3cac0-184">Int32</span></span>|<span data-ttu-id="3cac0-185">Legt fest, wie viele der zuletzt verwendeten Kennwörter nicht erneut verwendet werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="3cac0-185">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="3cac0-186">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3cac0-186">passwordRequiredType</span></span>|<span data-ttu-id="3cac0-187">String</span><span class="sxs-lookup"><span data-stu-id="3cac0-187">String</span></span>|<span data-ttu-id="3cac0-188">Geforderter Kennworttyp.</span><span class="sxs-lookup"><span data-stu-id="3cac0-188">Type of password that is required.</span></span> <span data-ttu-id="3cac0-189">Mögliche Werte sind: `deviceDefault`, `alphanumeric` und `numeric`.</span><span class="sxs-lookup"><span data-stu-id="3cac0-189">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3cac0-190">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3cac0-190">passwordRequired</span></span>|<span data-ttu-id="3cac0-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cac0-191">Boolean</span></span>|<span data-ttu-id="3cac0-192">Legt fest, ob ein Kennwort gefordert wird.</span><span class="sxs-lookup"><span data-stu-id="3cac0-192">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="3cac0-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="3cac0-193">Response</span></span>
<span data-ttu-id="3cac0-194">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3cac0-194">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cac0-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3cac0-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="3cac0-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3cac0-196">Request</span></span>
<span data-ttu-id="3cac0-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3cac0-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 970

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```

### <a name="response"></a><span data-ttu-id="3cac0-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="3cac0-198">Response</span></span>
<span data-ttu-id="3cac0-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3cac0-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1078

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```



