# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="90471-101">managedAndroidStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="90471-101">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="90471-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="90471-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90471-103">Aktualisieren der Eigenschaften eines [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="90471-103">Update the properties of a [calendar](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="90471-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="90471-104">Prerequisites</span></span>
<span data-ttu-id="90471-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="90471-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="90471-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="90471-107">Permission type</span></span>|<span data-ttu-id="90471-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="90471-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90471-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="90471-109">Delegated (work or school account)</span></span>|<span data-ttu-id="90471-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90471-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="90471-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="90471-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90471-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90471-112">Not supported.</span></span>|
|<span data-ttu-id="90471-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="90471-113">Application</span></span>|<span data-ttu-id="90471-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90471-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90471-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="90471-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="90471-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="90471-116">Request headers</span></span>
|<span data-ttu-id="90471-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="90471-117">Header</span></span>|<span data-ttu-id="90471-118">Wert</span><span class="sxs-lookup"><span data-stu-id="90471-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90471-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="90471-119">Authorization</span></span>|<span data-ttu-id="90471-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="90471-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="90471-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="90471-121">Accept</span></span>|<span data-ttu-id="90471-122">application/json</span><span class="sxs-lookup"><span data-stu-id="90471-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90471-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="90471-123">Request body</span></span>
<span data-ttu-id="90471-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="90471-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="90471-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="90471-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="90471-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="90471-126">Property</span></span>|<span data-ttu-id="90471-127">Typ</span><span class="sxs-lookup"><span data-stu-id="90471-127">Type</span></span>|<span data-ttu-id="90471-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90471-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90471-129">id</span><span class="sxs-lookup"><span data-stu-id="90471-129">id</span></span>|<span data-ttu-id="90471-130">String</span><span class="sxs-lookup"><span data-stu-id="90471-130">String</span></span>|<span data-ttu-id="90471-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="90471-131">Key of the setting.</span></span> <span data-ttu-id="90471-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90471-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="90471-133">displayName</span><span class="sxs-lookup"><span data-stu-id="90471-133">displayName</span></span>|<span data-ttu-id="90471-134">String</span><span class="sxs-lookup"><span data-stu-id="90471-134">String</span></span>|<span data-ttu-id="90471-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="90471-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="90471-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90471-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="90471-137">description</span><span class="sxs-lookup"><span data-stu-id="90471-137">description</span></span>|<span data-ttu-id="90471-138">String</span><span class="sxs-lookup"><span data-stu-id="90471-138">String</span></span>|<span data-ttu-id="90471-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="90471-139">The description of the app.</span></span> <span data-ttu-id="90471-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90471-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="90471-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="90471-141">Publisher</span></span>|<span data-ttu-id="90471-142">String</span><span class="sxs-lookup"><span data-stu-id="90471-142">String</span></span>|<span data-ttu-id="90471-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="90471-143">The name of the app.</span></span> <span data-ttu-id="90471-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90471-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="90471-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="90471-145">largeIcon</span></span>|[<span data-ttu-id="90471-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="90471-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="90471-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="90471-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="90471-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90471-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="90471-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90471-149">createdDateTime</span></span>|<span data-ttu-id="90471-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90471-150">DateTimeOffset</span></span>|<span data-ttu-id="90471-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="90471-151">The date and time the group was created.</span></span> <span data-ttu-id="90471-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90471-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="90471-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90471-153">lastModifiedDateTime</span></span>|<span data-ttu-id="90471-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90471-154">DateTimeOffset</span></span>|<span data-ttu-id="90471-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="90471-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="90471-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90471-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="90471-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="90471-157">isFeatured</span></span>|<span data-ttu-id="90471-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="90471-158">Boolean</span></span>|<span data-ttu-id="90471-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90471-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="90471-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="90471-160">privacyInformationUrl</span></span>|<span data-ttu-id="90471-161">String</span><span class="sxs-lookup"><span data-stu-id="90471-161">String</span></span>|<span data-ttu-id="90471-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="90471-162">The privacy statement Url.</span></span> <span data-ttu-id="90471-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90471-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="90471-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="90471-164">informationUrl</span></span>|<span data-ttu-id="90471-165">String</span><span class="sxs-lookup"><span data-stu-id="90471-165">String</span></span>|<span data-ttu-id="90471-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="90471-166">The more information Url.</span></span> <span data-ttu-id="90471-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90471-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="90471-168">owner</span><span class="sxs-lookup"><span data-stu-id="90471-168">owner</span></span>|<span data-ttu-id="90471-169">String</span><span class="sxs-lookup"><span data-stu-id="90471-169">String</span></span>|<span data-ttu-id="90471-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="90471-170">The owner of the app.</span></span> <span data-ttu-id="90471-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90471-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="90471-172">developer</span><span class="sxs-lookup"><span data-stu-id="90471-172">developer</span></span>|<span data-ttu-id="90471-173">String</span><span class="sxs-lookup"><span data-stu-id="90471-173">String</span></span>|<span data-ttu-id="90471-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="90471-174">The name of the app.</span></span> <span data-ttu-id="90471-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90471-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="90471-176">notes</span><span class="sxs-lookup"><span data-stu-id="90471-176">notes</span></span>|<span data-ttu-id="90471-177">String</span><span class="sxs-lookup"><span data-stu-id="90471-177">String</span></span>|<span data-ttu-id="90471-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="90471-178">Notes for the app.</span></span> <span data-ttu-id="90471-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90471-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="90471-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="90471-180">publishingState</span></span>|<span data-ttu-id="90471-181">String</span><span class="sxs-lookup"><span data-stu-id="90471-181">String</span></span>|<span data-ttu-id="90471-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="90471-182">The publishing state for the app.</span></span> <span data-ttu-id="90471-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="90471-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="90471-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="90471-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="90471-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="90471-185">appAvailability</span></span>|<span data-ttu-id="90471-186">String</span><span class="sxs-lookup"><span data-stu-id="90471-186">String</span></span>|<span data-ttu-id="90471-187">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="90471-187">The Application's availability.</span></span> <span data-ttu-id="90471-188">Geerbt von [managedApp](../resources/intune_apps_managedapp.md). Mögliche Werte sind: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="90471-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="90471-189">Version</span><span class="sxs-lookup"><span data-stu-id="90471-189">version</span></span>|<span data-ttu-id="90471-190">String</span><span class="sxs-lookup"><span data-stu-id="90471-190">String</span></span>|<span data-ttu-id="90471-191">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="90471-191">The Application's version.</span></span> <span data-ttu-id="90471-192">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="90471-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="90471-193">packageId</span><span class="sxs-lookup"><span data-stu-id="90471-193">packageId</span></span>|<span data-ttu-id="90471-194">String</span><span class="sxs-lookup"><span data-stu-id="90471-194">String</span></span>|<span data-ttu-id="90471-195">Die Paket-ID der App.</span><span class="sxs-lookup"><span data-stu-id="90471-195">The app's package ID.</span></span>|
|<span data-ttu-id="90471-196">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="90471-196">appStoreUrl</span></span>|<span data-ttu-id="90471-197">String</span><span class="sxs-lookup"><span data-stu-id="90471-197">String</span></span>|<span data-ttu-id="90471-198">Die URL des Android-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="90471-198">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="90471-199">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="90471-199">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="90471-200">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="90471-200">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="90471-201">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="90471-201">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="90471-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="90471-202">Response</span></span>
<span data-ttu-id="90471-203">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="90471-203">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90471-204">Beispiel</span><span class="sxs-lookup"><span data-stu-id="90471-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="90471-205">Anforderung</span><span class="sxs-lookup"><span data-stu-id="90471-205">Request</span></span>
<span data-ttu-id="90471-206">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="90471-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1019

{
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

### <a name="response"></a><span data-ttu-id="90471-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="90471-207">Response</span></span>
<span data-ttu-id="90471-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="90471-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



