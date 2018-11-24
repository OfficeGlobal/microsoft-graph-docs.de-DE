# <a name="create-iosstoreapp"></a><span data-ttu-id="eef97-101">iosStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="eef97-101">Create iosStoreApp</span></span>

> <span data-ttu-id="eef97-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eef97-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eef97-103">Erstellen eines neuen [IosStoreApp](../resources/intune_apps_iosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="eef97-103">Create a new [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eef97-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eef97-104">Prerequisites</span></span>
<span data-ttu-id="eef97-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eef97-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eef97-107">Permission type</span></span>|<span data-ttu-id="eef97-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eef97-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eef97-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eef97-109">Delegated (work or school account)</span></span>|<span data-ttu-id="eef97-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eef97-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eef97-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eef97-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eef97-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eef97-112">Not supported.</span></span>|
|<span data-ttu-id="eef97-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eef97-113">Application</span></span>|<span data-ttu-id="eef97-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eef97-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eef97-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eef97-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="eef97-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eef97-116">Request headers</span></span>
|<span data-ttu-id="eef97-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eef97-117">Header</span></span>|<span data-ttu-id="eef97-118">Wert</span><span class="sxs-lookup"><span data-stu-id="eef97-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eef97-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="eef97-119">Authorization</span></span>|<span data-ttu-id="eef97-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eef97-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eef97-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eef97-121">Accept</span></span>|<span data-ttu-id="eef97-122">application/json</span><span class="sxs-lookup"><span data-stu-id="eef97-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eef97-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eef97-123">Request body</span></span>
<span data-ttu-id="eef97-124">Geben Sie im Anforderungstext eine JSON-Darstellung des iosStoreApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="eef97-124">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="eef97-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="eef97-125">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="eef97-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eef97-126">Property</span></span>|<span data-ttu-id="eef97-127">Typ</span><span class="sxs-lookup"><span data-stu-id="eef97-127">Type</span></span>|<span data-ttu-id="eef97-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eef97-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eef97-129">id</span><span class="sxs-lookup"><span data-stu-id="eef97-129">id</span></span>|<span data-ttu-id="eef97-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eef97-130">String</span></span>|<span data-ttu-id="eef97-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="eef97-131">Key of the entity.</span></span> <span data-ttu-id="eef97-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eef97-133">displayName</span><span class="sxs-lookup"><span data-stu-id="eef97-133">displayName</span></span>|<span data-ttu-id="eef97-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eef97-134">String</span></span>|<span data-ttu-id="eef97-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="eef97-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="eef97-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eef97-137">description</span><span class="sxs-lookup"><span data-stu-id="eef97-137">description</span></span>|<span data-ttu-id="eef97-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eef97-138">String</span></span>|<span data-ttu-id="eef97-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="eef97-139">The description of the app.</span></span> <span data-ttu-id="eef97-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eef97-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="eef97-141">publisher</span></span>|<span data-ttu-id="eef97-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eef97-142">String</span></span>|<span data-ttu-id="eef97-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="eef97-143">The publisher of the app.</span></span> <span data-ttu-id="eef97-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eef97-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="eef97-145">largeIcon</span></span>|[<span data-ttu-id="eef97-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eef97-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="eef97-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="eef97-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="eef97-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eef97-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eef97-149">createdDateTime</span></span>|<span data-ttu-id="eef97-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eef97-150">DateTimeOffset</span></span>|<span data-ttu-id="eef97-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="eef97-151">The date and time the app was created.</span></span> <span data-ttu-id="eef97-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eef97-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eef97-153">lastModifiedDateTime</span></span>|<span data-ttu-id="eef97-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eef97-154">DateTimeOffset</span></span>|<span data-ttu-id="eef97-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="eef97-155">The date and time the app was last modified.</span></span> <span data-ttu-id="eef97-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eef97-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="eef97-157">isFeatured</span></span>|<span data-ttu-id="eef97-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eef97-158">Boolean</span></span>|<span data-ttu-id="eef97-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eef97-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="eef97-160">privacyInformationUrl</span></span>|<span data-ttu-id="eef97-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eef97-161">String</span></span>|<span data-ttu-id="eef97-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="eef97-162">The privacy statement Url.</span></span> <span data-ttu-id="eef97-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eef97-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="eef97-164">informationUrl</span></span>|<span data-ttu-id="eef97-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eef97-165">String</span></span>|<span data-ttu-id="eef97-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="eef97-166">The more information Url.</span></span> <span data-ttu-id="eef97-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eef97-168">owner</span><span class="sxs-lookup"><span data-stu-id="eef97-168">owner</span></span>|<span data-ttu-id="eef97-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eef97-169">String</span></span>|<span data-ttu-id="eef97-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="eef97-170">The owner of the app.</span></span> <span data-ttu-id="eef97-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eef97-172">developer</span><span class="sxs-lookup"><span data-stu-id="eef97-172">developer</span></span>|<span data-ttu-id="eef97-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eef97-173">String</span></span>|<span data-ttu-id="eef97-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="eef97-174">The developer of the app.</span></span> <span data-ttu-id="eef97-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eef97-176">notes</span><span class="sxs-lookup"><span data-stu-id="eef97-176">notes</span></span>|<span data-ttu-id="eef97-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eef97-177">String</span></span>|<span data-ttu-id="eef97-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="eef97-178">Notes for the app.</span></span> <span data-ttu-id="eef97-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="eef97-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="eef97-180">publishingState</span></span>|[<span data-ttu-id="eef97-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="eef97-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="eef97-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="eef97-182">The publishing state for the app.</span></span> <span data-ttu-id="eef97-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="eef97-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="eef97-184">Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eef97-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="eef97-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="eef97-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="eef97-186">bundleId</span><span class="sxs-lookup"><span data-stu-id="eef97-186">bundleId</span></span>|<span data-ttu-id="eef97-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eef97-187">String</span></span>|<span data-ttu-id="eef97-188">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="eef97-188">The Identity Name.</span></span>|
|<span data-ttu-id="eef97-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="eef97-189">appStoreUrl</span></span>|<span data-ttu-id="eef97-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eef97-190">String</span></span>|<span data-ttu-id="eef97-191">URL des Apple-App-Stores</span><span class="sxs-lookup"><span data-stu-id="eef97-191">The Apple App Store URL</span></span>|
|<span data-ttu-id="eef97-192">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="eef97-192">applicableDeviceType</span></span>|[<span data-ttu-id="eef97-193">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="eef97-193">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="eef97-194">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="eef97-194">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="eef97-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="eef97-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="eef97-196">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="eef97-196">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="eef97-197">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="eef97-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="eef97-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="eef97-198">Response</span></span>
<span data-ttu-id="eef97-199">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosStoreApp](../resources/intune_apps_iosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eef97-199">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eef97-200">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eef97-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="eef97-201">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eef97-201">Request</span></span>
<span data-ttu-id="eef97-202">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eef97-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1006

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
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
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="eef97-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="eef97-203">Response</span></span>
<span data-ttu-id="eef97-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eef97-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1178

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
    "v11_0": true,
    "v12_0": true
  }
}
```



