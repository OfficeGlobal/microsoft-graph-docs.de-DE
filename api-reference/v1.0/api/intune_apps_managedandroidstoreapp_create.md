# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="fa28e-101">managedAndroidStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="fa28e-101">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="fa28e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fa28e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa28e-103">Erstellen eines neuen [ManagedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa28e-103">Create a new [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa28e-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa28e-104">Prerequisites</span></span>
<span data-ttu-id="fa28e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fa28e-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa28e-107">Permission type</span></span>|<span data-ttu-id="fa28e-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa28e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa28e-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa28e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fa28e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa28e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fa28e-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa28e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa28e-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa28e-112">Not supported.</span></span>|
|<span data-ttu-id="fa28e-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa28e-113">Application</span></span>|<span data-ttu-id="fa28e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa28e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa28e-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa28e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fa28e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa28e-116">Request headers</span></span>
|<span data-ttu-id="fa28e-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fa28e-117">Header</span></span>|<span data-ttu-id="fa28e-118">Wert</span><span class="sxs-lookup"><span data-stu-id="fa28e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa28e-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fa28e-119">Authorization</span></span>|<span data-ttu-id="fa28e-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa28e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa28e-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="fa28e-121">Accept</span></span>|<span data-ttu-id="fa28e-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="fa28e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa28e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa28e-123">Request body</span></span>
<span data-ttu-id="fa28e-124">Geben Sie im Anforderungstext eine JSON-Darstellung des managedAndroidStoreApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="fa28e-124">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="fa28e-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedAndroidStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fa28e-125">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="fa28e-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa28e-126">Property</span></span>|<span data-ttu-id="fa28e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="fa28e-127">Type</span></span>|<span data-ttu-id="fa28e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa28e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa28e-129">ID</span><span class="sxs-lookup"><span data-stu-id="fa28e-129">id</span></span>|<span data-ttu-id="fa28e-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa28e-130">String</span></span>|<span data-ttu-id="fa28e-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fa28e-131">Key of the entity.</span></span> <span data-ttu-id="fa28e-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fa28e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="fa28e-133">displayName</span></span>|<span data-ttu-id="fa28e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa28e-134">String</span></span>|<span data-ttu-id="fa28e-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="fa28e-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fa28e-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fa28e-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa28e-137">description</span></span>|<span data-ttu-id="fa28e-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa28e-138">String</span></span>|<span data-ttu-id="fa28e-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="fa28e-139">The description of the app.</span></span> <span data-ttu-id="fa28e-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fa28e-141">Verleger</span><span class="sxs-lookup"><span data-stu-id="fa28e-141">publisher</span></span>|<span data-ttu-id="fa28e-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa28e-142">String</span></span>|<span data-ttu-id="fa28e-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="fa28e-143">The publisher of the app.</span></span> <span data-ttu-id="fa28e-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fa28e-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fa28e-145">largeIcon</span></span>|[<span data-ttu-id="fa28e-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fa28e-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="fa28e-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="fa28e-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fa28e-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fa28e-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa28e-149">createdDateTime</span></span>|<span data-ttu-id="fa28e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa28e-150">DateTimeOffset</span></span>|<span data-ttu-id="fa28e-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="fa28e-151">The date and time the app was created.</span></span> <span data-ttu-id="fa28e-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fa28e-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa28e-153">lastModifiedDateTime</span></span>|<span data-ttu-id="fa28e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa28e-154">DateTimeOffset</span></span>|<span data-ttu-id="fa28e-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="fa28e-155">The date and time the app was last modified.</span></span> <span data-ttu-id="fa28e-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fa28e-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fa28e-157">isFeatured</span></span>|<span data-ttu-id="fa28e-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="fa28e-158">Boolean</span></span>|<span data-ttu-id="fa28e-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fa28e-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fa28e-160">privacyInformationUrl</span></span>|<span data-ttu-id="fa28e-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa28e-161">String</span></span>|<span data-ttu-id="fa28e-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="fa28e-162">The privacy statement Url.</span></span> <span data-ttu-id="fa28e-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fa28e-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fa28e-164">informationUrl</span></span>|<span data-ttu-id="fa28e-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa28e-165">String</span></span>|<span data-ttu-id="fa28e-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="fa28e-166">The more information Url.</span></span> <span data-ttu-id="fa28e-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fa28e-168">owner</span><span class="sxs-lookup"><span data-stu-id="fa28e-168">owner</span></span>|<span data-ttu-id="fa28e-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa28e-169">String</span></span>|<span data-ttu-id="fa28e-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="fa28e-170">The owner of the app.</span></span> <span data-ttu-id="fa28e-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fa28e-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="fa28e-172">developer</span></span>|<span data-ttu-id="fa28e-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa28e-173">String</span></span>|<span data-ttu-id="fa28e-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="fa28e-174">The developer of the app.</span></span> <span data-ttu-id="fa28e-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fa28e-176">Hinweise</span><span class="sxs-lookup"><span data-stu-id="fa28e-176">notes</span></span>|<span data-ttu-id="fa28e-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa28e-177">String</span></span>|<span data-ttu-id="fa28e-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="fa28e-178">Notes for the app.</span></span> <span data-ttu-id="fa28e-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="fa28e-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="fa28e-180">publishingState</span></span>|[<span data-ttu-id="fa28e-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fa28e-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="fa28e-182">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="fa28e-182">The publishing state for the app.</span></span> <span data-ttu-id="fa28e-183">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="fa28e-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fa28e-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="fa28e-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="fa28e-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fa28e-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="fa28e-186">appAvailability</span></span>|[<span data-ttu-id="fa28e-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="fa28e-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="fa28e-188">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="fa28e-188">The Application's availability.</span></span> <span data-ttu-id="fa28e-189">Geerbt von [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa28e-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span> <span data-ttu-id="fa28e-190">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="fa28e-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="fa28e-191">version</span><span class="sxs-lookup"><span data-stu-id="fa28e-191">version</span></span>|<span data-ttu-id="fa28e-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa28e-192">String</span></span>|<span data-ttu-id="fa28e-193">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="fa28e-193">The Application's version.</span></span> <span data-ttu-id="fa28e-194">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="fa28e-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="fa28e-195">packageId</span><span class="sxs-lookup"><span data-stu-id="fa28e-195">packageId</span></span>|<span data-ttu-id="fa28e-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa28e-196">String</span></span>|<span data-ttu-id="fa28e-197">Die Paket-ID der App.</span><span class="sxs-lookup"><span data-stu-id="fa28e-197">The app's package ID.</span></span>|
|<span data-ttu-id="fa28e-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="fa28e-198">appStoreUrl</span></span>|<span data-ttu-id="fa28e-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa28e-199">String</span></span>|<span data-ttu-id="fa28e-200">Die URL des Android-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="fa28e-200">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="fa28e-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fa28e-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fa28e-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fa28e-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="fa28e-203">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="fa28e-203">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="fa28e-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa28e-204">Response</span></span>
<span data-ttu-id="fa28e-205">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa28e-205">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa28e-206">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa28e-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa28e-207">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa28e-207">Request</span></span>
<span data-ttu-id="fa28e-208">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa28e-208">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fa28e-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa28e-209">Response</span></span>
<span data-ttu-id="fa28e-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa28e-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








