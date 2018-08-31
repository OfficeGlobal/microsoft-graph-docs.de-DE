# <a name="create-managediosstoreapp"></a><span data-ttu-id="9827a-101">managedIOSStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="9827a-101">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="9827a-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9827a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9827a-103">Erstellen eines neuen [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9827a-103">Create a new [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9827a-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9827a-104">Prerequisites</span></span>
<span data-ttu-id="9827a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9827a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9827a-107">Permission type</span></span>|<span data-ttu-id="9827a-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9827a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9827a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9827a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9827a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9827a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9827a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9827a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9827a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9827a-112">Not supported.</span></span>|
|<span data-ttu-id="9827a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9827a-113">Application</span></span>|<span data-ttu-id="9827a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9827a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9827a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9827a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9827a-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9827a-116">Request headers</span></span>
|<span data-ttu-id="9827a-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9827a-117">Header</span></span>|<span data-ttu-id="9827a-118">Wert</span><span class="sxs-lookup"><span data-stu-id="9827a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9827a-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9827a-119">Authorization</span></span>|<span data-ttu-id="9827a-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9827a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9827a-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="9827a-121">Accept</span></span>|<span data-ttu-id="9827a-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="9827a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9827a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9827a-123">Request body</span></span>
<span data-ttu-id="9827a-124">Geben Sie im Anforderungstext eine JSON-Darstellung des managedIOSStoreApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="9827a-124">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="9827a-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedIOSStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9827a-125">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="9827a-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9827a-126">Property</span></span>|<span data-ttu-id="9827a-127">Typ</span><span class="sxs-lookup"><span data-stu-id="9827a-127">Type</span></span>|<span data-ttu-id="9827a-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9827a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9827a-129">id</span><span class="sxs-lookup"><span data-stu-id="9827a-129">id</span></span>|<span data-ttu-id="9827a-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9827a-130">String</span></span>|<span data-ttu-id="9827a-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9827a-131">Key of the entity.</span></span> <span data-ttu-id="9827a-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9827a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9827a-133">displayName</span></span>|<span data-ttu-id="9827a-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9827a-134">String</span></span>|<span data-ttu-id="9827a-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="9827a-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9827a-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9827a-137">description</span><span class="sxs-lookup"><span data-stu-id="9827a-137">description</span></span>|<span data-ttu-id="9827a-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9827a-138">String</span></span>|<span data-ttu-id="9827a-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="9827a-139">The description of the app.</span></span> <span data-ttu-id="9827a-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9827a-141">publisher</span><span class="sxs-lookup"><span data-stu-id="9827a-141">publisher</span></span>|<span data-ttu-id="9827a-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9827a-142">String</span></span>|<span data-ttu-id="9827a-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="9827a-143">The publisher of the app.</span></span> <span data-ttu-id="9827a-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9827a-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9827a-145">largeIcon</span></span>|[<span data-ttu-id="9827a-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9827a-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="9827a-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="9827a-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9827a-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9827a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9827a-149">createdDateTime</span></span>|<span data-ttu-id="9827a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9827a-150">DateTimeOffset</span></span>|<span data-ttu-id="9827a-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="9827a-151">The date and time the app was created.</span></span> <span data-ttu-id="9827a-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9827a-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9827a-153">lastModifiedDateTime</span></span>|<span data-ttu-id="9827a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9827a-154">DateTimeOffset</span></span>|<span data-ttu-id="9827a-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="9827a-155">The date and time the app was last modified.</span></span> <span data-ttu-id="9827a-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9827a-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9827a-157">isFeatured</span></span>|<span data-ttu-id="9827a-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="9827a-158">Boolean</span></span>|<span data-ttu-id="9827a-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9827a-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9827a-160">privacyInformationUrl</span></span>|<span data-ttu-id="9827a-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9827a-161">String</span></span>|<span data-ttu-id="9827a-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="9827a-162">The privacy statement Url.</span></span> <span data-ttu-id="9827a-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9827a-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9827a-164">informationUrl</span></span>|<span data-ttu-id="9827a-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9827a-165">String</span></span>|<span data-ttu-id="9827a-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="9827a-166">The more information Url.</span></span> <span data-ttu-id="9827a-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9827a-168">owner</span><span class="sxs-lookup"><span data-stu-id="9827a-168">owner</span></span>|<span data-ttu-id="9827a-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9827a-169">String</span></span>|<span data-ttu-id="9827a-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="9827a-170">The owner of the app.</span></span> <span data-ttu-id="9827a-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9827a-172">developer</span><span class="sxs-lookup"><span data-stu-id="9827a-172">developer</span></span>|<span data-ttu-id="9827a-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9827a-173">String</span></span>|<span data-ttu-id="9827a-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="9827a-174">The developer of the app.</span></span> <span data-ttu-id="9827a-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9827a-176">notes</span><span class="sxs-lookup"><span data-stu-id="9827a-176">notes</span></span>|<span data-ttu-id="9827a-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9827a-177">String</span></span>|<span data-ttu-id="9827a-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="9827a-178">Notes for the app.</span></span> <span data-ttu-id="9827a-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9827a-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="9827a-180">publishingState</span></span>|[<span data-ttu-id="9827a-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9827a-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="9827a-182">Der Veröffentlichungsstatus der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="9827a-182">The publishing state for the app.</span></span> <span data-ttu-id="9827a-183">Eine Anwendung kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="9827a-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9827a-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="9827a-185">Mögliche Werte sind `notPublished`, `processing`,`published`.</span><span class="sxs-lookup"><span data-stu-id="9827a-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="9827a-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="9827a-186">appAvailability</span></span>|[<span data-ttu-id="9827a-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="9827a-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="9827a-188">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="9827a-188">The Application's availability.</span></span> <span data-ttu-id="9827a-189">Geerbt von [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9827a-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span> <span data-ttu-id="9827a-190">Mögliche Werte sind: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="9827a-190">The possible values are:</span></span>|
|<span data-ttu-id="9827a-191">version</span><span class="sxs-lookup"><span data-stu-id="9827a-191">version</span></span>|<span data-ttu-id="9827a-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9827a-192">String</span></span>|<span data-ttu-id="9827a-193">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="9827a-193">The Application's version.</span></span> <span data-ttu-id="9827a-194">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="9827a-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="9827a-195">bundled</span><span class="sxs-lookup"><span data-stu-id="9827a-195">bundleId</span></span>|<span data-ttu-id="9827a-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9827a-196">String</span></span>|<span data-ttu-id="9827a-197">Die Bundle-ID einer App.</span><span class="sxs-lookup"><span data-stu-id="9827a-197">The app's Bundle ID.</span></span>|
|<span data-ttu-id="9827a-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9827a-198">appStoreUrl</span></span>|<span data-ttu-id="9827a-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9827a-199">String</span></span>|<span data-ttu-id="9827a-200">Die URL des Apple-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="9827a-200">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="9827a-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="9827a-201">applicableDeviceType</span></span>|[<span data-ttu-id="9827a-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9827a-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="9827a-203">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="9827a-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="9827a-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9827a-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9827a-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9827a-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="9827a-206">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="9827a-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="9827a-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="9827a-207">Response</span></span>
<span data-ttu-id="9827a-208">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9827a-208">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9827a-209">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9827a-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="9827a-210">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9827a-210">Request</span></span>
<span data-ttu-id="9827a-211">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9827a-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9827a-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="9827a-212">Response</span></span>
<span data-ttu-id="9827a-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9827a-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



