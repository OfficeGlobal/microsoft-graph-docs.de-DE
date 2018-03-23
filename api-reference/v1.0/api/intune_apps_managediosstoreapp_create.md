# <a name="create-managediosstoreapp"></a><span data-ttu-id="73218-101">managedIOSStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="73218-101">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="73218-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="73218-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73218-103">Erstellen eines neuen [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="73218-103">Create a new [plannerBucket](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73218-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="73218-104">Prerequisites</span></span>
<span data-ttu-id="73218-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="73218-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="73218-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73218-107">Permission type</span></span>|<span data-ttu-id="73218-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73218-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73218-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73218-109">Delegated (work or school account)</span></span>|<span data-ttu-id="73218-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73218-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73218-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73218-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73218-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73218-112">Not supported.</span></span>|
|<span data-ttu-id="73218-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73218-113">Application</span></span>|<span data-ttu-id="73218-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73218-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73218-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73218-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="73218-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73218-116">Request headers</span></span>
|<span data-ttu-id="73218-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="73218-117">Header</span></span>|<span data-ttu-id="73218-118">Wert</span><span class="sxs-lookup"><span data-stu-id="73218-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73218-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="73218-119">Authorization</span></span>|<span data-ttu-id="73218-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="73218-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="73218-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="73218-121">Accept</span></span>|<span data-ttu-id="73218-122">application/json</span><span class="sxs-lookup"><span data-stu-id="73218-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73218-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73218-123">Request body</span></span>
<span data-ttu-id="73218-124">Geben Sie im Anforderungstext eine JSON-Darstellung des managedIOSStoreApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="73218-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="73218-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedIOSStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="73218-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="73218-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73218-126">Property</span></span>|<span data-ttu-id="73218-127">Typ</span><span class="sxs-lookup"><span data-stu-id="73218-127">Type</span></span>|<span data-ttu-id="73218-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73218-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73218-129">id</span><span class="sxs-lookup"><span data-stu-id="73218-129">id</span></span>|<span data-ttu-id="73218-130">String</span><span class="sxs-lookup"><span data-stu-id="73218-130">String</span></span>|<span data-ttu-id="73218-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="73218-131">Key of the setting.</span></span> <span data-ttu-id="73218-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73218-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73218-133">displayName</span><span class="sxs-lookup"><span data-stu-id="73218-133">displayName</span></span>|<span data-ttu-id="73218-134">String</span><span class="sxs-lookup"><span data-stu-id="73218-134">String</span></span>|<span data-ttu-id="73218-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="73218-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="73218-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73218-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73218-137">description</span><span class="sxs-lookup"><span data-stu-id="73218-137">description</span></span>|<span data-ttu-id="73218-138">String</span><span class="sxs-lookup"><span data-stu-id="73218-138">String</span></span>|<span data-ttu-id="73218-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="73218-139">The description of the app.</span></span> <span data-ttu-id="73218-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73218-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73218-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="73218-141">Publisher</span></span>|<span data-ttu-id="73218-142">String</span><span class="sxs-lookup"><span data-stu-id="73218-142">String</span></span>|<span data-ttu-id="73218-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="73218-143">The name of the app.</span></span> <span data-ttu-id="73218-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73218-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73218-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="73218-145">largeIcon</span></span>|[<span data-ttu-id="73218-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="73218-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="73218-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="73218-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="73218-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73218-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73218-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73218-149">createdDateTime</span></span>|<span data-ttu-id="73218-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73218-150">DateTimeOffset</span></span>|<span data-ttu-id="73218-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="73218-151">The date and time the group was created.</span></span> <span data-ttu-id="73218-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73218-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73218-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73218-153">lastModifiedDateTime</span></span>|<span data-ttu-id="73218-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73218-154">DateTimeOffset</span></span>|<span data-ttu-id="73218-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="73218-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="73218-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73218-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73218-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="73218-157">isFeatured</span></span>|<span data-ttu-id="73218-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="73218-158">Boolean</span></span>|<span data-ttu-id="73218-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73218-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73218-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="73218-160">privacyInformationUrl</span></span>|<span data-ttu-id="73218-161">String</span><span class="sxs-lookup"><span data-stu-id="73218-161">String</span></span>|<span data-ttu-id="73218-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="73218-162">The privacy statement Url.</span></span> <span data-ttu-id="73218-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73218-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73218-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="73218-164">informationUrl</span></span>|<span data-ttu-id="73218-165">String</span><span class="sxs-lookup"><span data-stu-id="73218-165">String</span></span>|<span data-ttu-id="73218-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="73218-166">The more information Url.</span></span> <span data-ttu-id="73218-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73218-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73218-168">owner</span><span class="sxs-lookup"><span data-stu-id="73218-168">owner</span></span>|<span data-ttu-id="73218-169">String</span><span class="sxs-lookup"><span data-stu-id="73218-169">String</span></span>|<span data-ttu-id="73218-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="73218-170">The owner of the app.</span></span> <span data-ttu-id="73218-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73218-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73218-172">developer</span><span class="sxs-lookup"><span data-stu-id="73218-172">developer</span></span>|<span data-ttu-id="73218-173">String</span><span class="sxs-lookup"><span data-stu-id="73218-173">String</span></span>|<span data-ttu-id="73218-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="73218-174">The name of the app.</span></span> <span data-ttu-id="73218-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73218-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73218-176">notes</span><span class="sxs-lookup"><span data-stu-id="73218-176">notes</span></span>|<span data-ttu-id="73218-177">String</span><span class="sxs-lookup"><span data-stu-id="73218-177">String</span></span>|<span data-ttu-id="73218-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="73218-178">Notes for the app.</span></span> <span data-ttu-id="73218-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73218-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73218-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="73218-180">publishingState</span></span>|<span data-ttu-id="73218-181">String</span><span class="sxs-lookup"><span data-stu-id="73218-181">String</span></span>|<span data-ttu-id="73218-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="73218-182">The publishing state for the app.</span></span> <span data-ttu-id="73218-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="73218-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="73218-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="73218-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="73218-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="73218-185">appAvailability</span></span>|<span data-ttu-id="73218-186">String</span><span class="sxs-lookup"><span data-stu-id="73218-186">String</span></span>|<span data-ttu-id="73218-187">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="73218-187">The Application's availability.</span></span> <span data-ttu-id="73218-188">Geerbt von [managedApp](../resources/intune_apps_managedapp.md). Mögliche Werte sind: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="73218-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="73218-189">Version</span><span class="sxs-lookup"><span data-stu-id="73218-189">version</span></span>|<span data-ttu-id="73218-190">String</span><span class="sxs-lookup"><span data-stu-id="73218-190">String</span></span>|<span data-ttu-id="73218-191">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="73218-191">The Application's version.</span></span> <span data-ttu-id="73218-192">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="73218-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="73218-193">bundleId</span><span class="sxs-lookup"><span data-stu-id="73218-193">bundleId</span></span>|<span data-ttu-id="73218-194">String</span><span class="sxs-lookup"><span data-stu-id="73218-194">String</span></span>|<span data-ttu-id="73218-195">Die Bundle-ID einer App.</span><span class="sxs-lookup"><span data-stu-id="73218-195">The app's Bundle ID.</span></span>|
|<span data-ttu-id="73218-196">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="73218-196">appStoreUrl</span></span>|<span data-ttu-id="73218-197">String</span><span class="sxs-lookup"><span data-stu-id="73218-197">String</span></span>|<span data-ttu-id="73218-198">Die URL des Apple-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="73218-198">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="73218-199">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="73218-199">applicableDeviceType</span></span>|[<span data-ttu-id="73218-200">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="73218-200">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="73218-201">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="73218-201">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="73218-202">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="73218-202">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="73218-203">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="73218-203">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="73218-204">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="73218-204">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="73218-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="73218-205">Response</span></span>
<span data-ttu-id="73218-206">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73218-206">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73218-207">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73218-207">Example</span></span>
### <a name="request"></a><span data-ttu-id="73218-208">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73218-208">Request</span></span>
<span data-ttu-id="73218-209">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73218-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1128

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="73218-210">Antwort</span><span class="sxs-lookup"><span data-stu-id="73218-210">Response</span></span>
<span data-ttu-id="73218-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73218-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1236

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```



