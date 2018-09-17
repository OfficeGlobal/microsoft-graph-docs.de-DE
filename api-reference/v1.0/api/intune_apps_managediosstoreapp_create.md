# <a name="create-managediosstoreapp"></a><span data-ttu-id="1286f-101">managedIOSStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="1286f-101">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="1286f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1286f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1286f-103">Erstellen eines neuen [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1286f-103">Create a new [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1286f-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1286f-104">Prerequisites</span></span>
<span data-ttu-id="1286f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1286f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1286f-107">Permission type</span></span>|<span data-ttu-id="1286f-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1286f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1286f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1286f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1286f-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1286f-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1286f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1286f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1286f-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1286f-112">Not supported.</span></span>|
|<span data-ttu-id="1286f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1286f-113">Application</span></span>|<span data-ttu-id="1286f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1286f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1286f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1286f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1286f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1286f-116">Request headers</span></span>
|<span data-ttu-id="1286f-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1286f-117">Header</span></span>|<span data-ttu-id="1286f-118">Wert</span><span class="sxs-lookup"><span data-stu-id="1286f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1286f-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1286f-119">Authorization</span></span>|<span data-ttu-id="1286f-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1286f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1286f-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="1286f-121">Accept</span></span>|<span data-ttu-id="1286f-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="1286f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1286f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1286f-123">Request body</span></span>
<span data-ttu-id="1286f-124">Geben Sie im Anforderungstext eine JSON-Darstellung des managedIOSStoreApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1286f-124">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="1286f-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedIOSStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1286f-125">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="1286f-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1286f-126">Property</span></span>|<span data-ttu-id="1286f-127">Typ</span><span class="sxs-lookup"><span data-stu-id="1286f-127">Type</span></span>|<span data-ttu-id="1286f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1286f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1286f-129">id</span><span class="sxs-lookup"><span data-stu-id="1286f-129">id</span></span>|<span data-ttu-id="1286f-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1286f-130">String</span></span>|<span data-ttu-id="1286f-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1286f-131">Key of the entity.</span></span> <span data-ttu-id="1286f-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1286f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1286f-133">displayName</span></span>|<span data-ttu-id="1286f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1286f-134">String</span></span>|<span data-ttu-id="1286f-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="1286f-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1286f-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1286f-137">description</span><span class="sxs-lookup"><span data-stu-id="1286f-137">description</span></span>|<span data-ttu-id="1286f-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1286f-138">String</span></span>|<span data-ttu-id="1286f-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="1286f-139">The description of the app.</span></span> <span data-ttu-id="1286f-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1286f-141">publisher</span><span class="sxs-lookup"><span data-stu-id="1286f-141">publisher</span></span>|<span data-ttu-id="1286f-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1286f-142">String</span></span>|<span data-ttu-id="1286f-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="1286f-143">The publisher of the app.</span></span> <span data-ttu-id="1286f-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1286f-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1286f-145">largeIcon</span></span>|[<span data-ttu-id="1286f-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1286f-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="1286f-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1286f-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1286f-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1286f-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1286f-149">createdDateTime</span></span>|<span data-ttu-id="1286f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1286f-150">DateTimeOffset</span></span>|<span data-ttu-id="1286f-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="1286f-151">The date and time the app was created.</span></span> <span data-ttu-id="1286f-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1286f-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1286f-153">lastModifiedDateTime</span></span>|<span data-ttu-id="1286f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1286f-154">DateTimeOffset</span></span>|<span data-ttu-id="1286f-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="1286f-155">The date and time the app was last modified.</span></span> <span data-ttu-id="1286f-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1286f-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1286f-157">isFeatured</span></span>|<span data-ttu-id="1286f-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1286f-158">Boolean</span></span>|<span data-ttu-id="1286f-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1286f-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1286f-160">privacyInformationUrl</span></span>|<span data-ttu-id="1286f-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1286f-161">String</span></span>|<span data-ttu-id="1286f-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="1286f-162">The privacy statement Url.</span></span> <span data-ttu-id="1286f-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1286f-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1286f-164">informationUrl</span></span>|<span data-ttu-id="1286f-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1286f-165">String</span></span>|<span data-ttu-id="1286f-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="1286f-166">The more information Url.</span></span> <span data-ttu-id="1286f-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1286f-168">owner</span><span class="sxs-lookup"><span data-stu-id="1286f-168">owner</span></span>|<span data-ttu-id="1286f-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1286f-169">String</span></span>|<span data-ttu-id="1286f-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="1286f-170">The owner of the app.</span></span> <span data-ttu-id="1286f-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1286f-172">developer</span><span class="sxs-lookup"><span data-stu-id="1286f-172">developer</span></span>|<span data-ttu-id="1286f-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1286f-173">String</span></span>|<span data-ttu-id="1286f-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="1286f-174">The developer of the app.</span></span> <span data-ttu-id="1286f-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1286f-176">notes</span><span class="sxs-lookup"><span data-stu-id="1286f-176">notes</span></span>|<span data-ttu-id="1286f-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1286f-177">String</span></span>|<span data-ttu-id="1286f-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="1286f-178">Notes for the app.</span></span> <span data-ttu-id="1286f-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1286f-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1286f-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="1286f-180">publishingState</span></span>|[<span data-ttu-id="1286f-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1286f-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="1286f-p114">Der Veröffentlichungsstand der App. Die App kann nur dann zugewiesen werden, wenn die App veröffentlicht wird. Vererbt von [mobileApp](../resources/intune_apps_mobileapp.md). Die möglichen Werte sind: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1286f-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1286f-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="1286f-186">appAvailability</span></span>|[<span data-ttu-id="1286f-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="1286f-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="1286f-p115">Verfügbarkeit der Anwendung. Geerbt von [ManagedApp](../resources/intune_apps_managedapp.md). Mögliche Werte sind: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="1286f-p115">The Application's availability. Inherited from [managedApp](../resources/intune_apps_managedapp.md). The possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="1286f-191">Version</span><span class="sxs-lookup"><span data-stu-id="1286f-191">version</span></span>|<span data-ttu-id="1286f-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1286f-192">String</span></span>|<span data-ttu-id="1286f-193">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="1286f-193">The Application's version.</span></span> <span data-ttu-id="1286f-194">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="1286f-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="1286f-195">bundled</span><span class="sxs-lookup"><span data-stu-id="1286f-195">bundleId</span></span>|<span data-ttu-id="1286f-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1286f-196">String</span></span>|<span data-ttu-id="1286f-197">Die Bundle-ID einer App.</span><span class="sxs-lookup"><span data-stu-id="1286f-197">The app's Bundle ID.</span></span>|
|<span data-ttu-id="1286f-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1286f-198">appStoreUrl</span></span>|<span data-ttu-id="1286f-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1286f-199">String</span></span>|<span data-ttu-id="1286f-200">Die URL des Apple-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="1286f-200">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="1286f-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="1286f-201">applicableDeviceType</span></span>|[<span data-ttu-id="1286f-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1286f-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="1286f-203">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="1286f-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="1286f-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1286f-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1286f-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1286f-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="1286f-206">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="1286f-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="1286f-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="1286f-207">Response</span></span>
<span data-ttu-id="1286f-208">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1286f-208">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1286f-209">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1286f-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="1286f-210">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1286f-210">Request</span></span>
<span data-ttu-id="1286f-211">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1286f-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1286f-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="1286f-212">Response</span></span>
<span data-ttu-id="1286f-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1286f-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








