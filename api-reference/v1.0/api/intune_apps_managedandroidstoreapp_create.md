# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="75960-101">managedAndroidStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="75960-101">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="75960-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="75960-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75960-103">Erstellen eines neuen [ManagedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="75960-103">Create a new [plannerBucket](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="75960-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="75960-104">Prerequisites</span></span>
<span data-ttu-id="75960-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="75960-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="75960-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="75960-107">Permission type</span></span>|<span data-ttu-id="75960-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="75960-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75960-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="75960-109">Delegated (work or school account)</span></span>|<span data-ttu-id="75960-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75960-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="75960-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="75960-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75960-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75960-112">Not supported.</span></span>|
|<span data-ttu-id="75960-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="75960-113">Application</span></span>|<span data-ttu-id="75960-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75960-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75960-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="75960-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="75960-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="75960-116">Request headers</span></span>
|<span data-ttu-id="75960-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="75960-117">Header</span></span>|<span data-ttu-id="75960-118">Wert</span><span class="sxs-lookup"><span data-stu-id="75960-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75960-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="75960-119">Authorization</span></span>|<span data-ttu-id="75960-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="75960-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="75960-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="75960-121">Accept</span></span>|<span data-ttu-id="75960-122">application/json</span><span class="sxs-lookup"><span data-stu-id="75960-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75960-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="75960-123">Request body</span></span>
<span data-ttu-id="75960-124">Geben Sie im Anforderungstext eine JSON-Darstellung des managedAndroidStoreApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="75960-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="75960-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedAndroidStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="75960-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="75960-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="75960-126">Property</span></span>|<span data-ttu-id="75960-127">Typ</span><span class="sxs-lookup"><span data-stu-id="75960-127">Type</span></span>|<span data-ttu-id="75960-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75960-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75960-129">id</span><span class="sxs-lookup"><span data-stu-id="75960-129">id</span></span>|<span data-ttu-id="75960-130">String</span><span class="sxs-lookup"><span data-stu-id="75960-130">String</span></span>|<span data-ttu-id="75960-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="75960-131">Key of the setting.</span></span> <span data-ttu-id="75960-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75960-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="75960-133">displayName</span><span class="sxs-lookup"><span data-stu-id="75960-133">displayName</span></span>|<span data-ttu-id="75960-134">String</span><span class="sxs-lookup"><span data-stu-id="75960-134">String</span></span>|<span data-ttu-id="75960-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="75960-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="75960-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75960-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="75960-137">description</span><span class="sxs-lookup"><span data-stu-id="75960-137">description</span></span>|<span data-ttu-id="75960-138">String</span><span class="sxs-lookup"><span data-stu-id="75960-138">String</span></span>|<span data-ttu-id="75960-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="75960-139">The description of the app.</span></span> <span data-ttu-id="75960-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75960-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="75960-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="75960-141">Publisher</span></span>|<span data-ttu-id="75960-142">String</span><span class="sxs-lookup"><span data-stu-id="75960-142">String</span></span>|<span data-ttu-id="75960-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="75960-143">The name of the app.</span></span> <span data-ttu-id="75960-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75960-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="75960-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="75960-145">largeIcon</span></span>|[<span data-ttu-id="75960-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="75960-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="75960-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="75960-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="75960-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75960-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="75960-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75960-149">createdDateTime</span></span>|<span data-ttu-id="75960-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75960-150">DateTimeOffset</span></span>|<span data-ttu-id="75960-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="75960-151">The date and time the group was created.</span></span> <span data-ttu-id="75960-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75960-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="75960-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75960-153">lastModifiedDateTime</span></span>|<span data-ttu-id="75960-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75960-154">DateTimeOffset</span></span>|<span data-ttu-id="75960-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="75960-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="75960-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75960-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="75960-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="75960-157">isFeatured</span></span>|<span data-ttu-id="75960-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="75960-158">Boolean</span></span>|<span data-ttu-id="75960-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75960-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="75960-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="75960-160">privacyInformationUrl</span></span>|<span data-ttu-id="75960-161">String</span><span class="sxs-lookup"><span data-stu-id="75960-161">String</span></span>|<span data-ttu-id="75960-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="75960-162">The privacy statement Url.</span></span> <span data-ttu-id="75960-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75960-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="75960-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="75960-164">informationUrl</span></span>|<span data-ttu-id="75960-165">String</span><span class="sxs-lookup"><span data-stu-id="75960-165">String</span></span>|<span data-ttu-id="75960-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="75960-166">The more information Url.</span></span> <span data-ttu-id="75960-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75960-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="75960-168">owner</span><span class="sxs-lookup"><span data-stu-id="75960-168">owner</span></span>|<span data-ttu-id="75960-169">String</span><span class="sxs-lookup"><span data-stu-id="75960-169">String</span></span>|<span data-ttu-id="75960-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="75960-170">The owner of the app.</span></span> <span data-ttu-id="75960-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75960-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="75960-172">developer</span><span class="sxs-lookup"><span data-stu-id="75960-172">developer</span></span>|<span data-ttu-id="75960-173">String</span><span class="sxs-lookup"><span data-stu-id="75960-173">String</span></span>|<span data-ttu-id="75960-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="75960-174">The name of the app.</span></span> <span data-ttu-id="75960-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75960-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="75960-176">notes</span><span class="sxs-lookup"><span data-stu-id="75960-176">notes</span></span>|<span data-ttu-id="75960-177">String</span><span class="sxs-lookup"><span data-stu-id="75960-177">String</span></span>|<span data-ttu-id="75960-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="75960-178">Notes for the app.</span></span> <span data-ttu-id="75960-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75960-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="75960-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="75960-180">publishingState</span></span>|<span data-ttu-id="75960-181">String</span><span class="sxs-lookup"><span data-stu-id="75960-181">String</span></span>|<span data-ttu-id="75960-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="75960-182">The publishing state for the app.</span></span> <span data-ttu-id="75960-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="75960-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="75960-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="75960-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="75960-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="75960-185">appAvailability</span></span>|<span data-ttu-id="75960-186">String</span><span class="sxs-lookup"><span data-stu-id="75960-186">String</span></span>|<span data-ttu-id="75960-187">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="75960-187">The Application's availability.</span></span> <span data-ttu-id="75960-188">Geerbt von [managedApp](../resources/intune_apps_managedapp.md). Mögliche Werte sind: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="75960-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="75960-189">Version</span><span class="sxs-lookup"><span data-stu-id="75960-189">version</span></span>|<span data-ttu-id="75960-190">String</span><span class="sxs-lookup"><span data-stu-id="75960-190">String</span></span>|<span data-ttu-id="75960-191">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="75960-191">The Application's version.</span></span> <span data-ttu-id="75960-192">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="75960-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="75960-193">packageId</span><span class="sxs-lookup"><span data-stu-id="75960-193">packageId</span></span>|<span data-ttu-id="75960-194">String</span><span class="sxs-lookup"><span data-stu-id="75960-194">String</span></span>|<span data-ttu-id="75960-195">Die Paket-ID der App.</span><span class="sxs-lookup"><span data-stu-id="75960-195">The app's package ID.</span></span>|
|<span data-ttu-id="75960-196">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="75960-196">appStoreUrl</span></span>|<span data-ttu-id="75960-197">String</span><span class="sxs-lookup"><span data-stu-id="75960-197">String</span></span>|<span data-ttu-id="75960-198">Die URL des Android-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="75960-198">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="75960-199">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="75960-199">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="75960-200">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="75960-200">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="75960-201">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="75960-201">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="75960-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="75960-202">Response</span></span>
<span data-ttu-id="75960-203">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75960-203">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75960-204">Beispiel</span><span class="sxs-lookup"><span data-stu-id="75960-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="75960-205">Anforderung</span><span class="sxs-lookup"><span data-stu-id="75960-205">Request</span></span>
<span data-ttu-id="75960-206">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="75960-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1080

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="75960-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="75960-207">Response</span></span>
<span data-ttu-id="75960-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75960-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1188

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```



