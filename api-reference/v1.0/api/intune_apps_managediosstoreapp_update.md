# <a name="update-managediosstoreapp"></a><span data-ttu-id="beaa0-101">managedIOSStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="beaa0-101">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="beaa0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="beaa0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="beaa0-103">Aktualisieren der Eigenschaften eines [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="beaa0-103">Update the properties of a [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="beaa0-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="beaa0-104">Prerequisites</span></span>
<span data-ttu-id="beaa0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="beaa0-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="beaa0-107">Permission type</span></span>|<span data-ttu-id="beaa0-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="beaa0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="beaa0-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="beaa0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="beaa0-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beaa0-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="beaa0-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="beaa0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="beaa0-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beaa0-112">Not supported.</span></span>|
|<span data-ttu-id="beaa0-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="beaa0-113">Application</span></span>|<span data-ttu-id="beaa0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beaa0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="beaa0-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="beaa0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="beaa0-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="beaa0-116">Request headers</span></span>
|<span data-ttu-id="beaa0-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="beaa0-117">Header</span></span>|<span data-ttu-id="beaa0-118">Wert</span><span class="sxs-lookup"><span data-stu-id="beaa0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="beaa0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="beaa0-119">Authorization</span></span>|<span data-ttu-id="beaa0-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="beaa0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="beaa0-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="beaa0-121">Accept</span></span>|<span data-ttu-id="beaa0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="beaa0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="beaa0-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="beaa0-123">Request body</span></span>
<span data-ttu-id="beaa0-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="beaa0-124">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>

<span data-ttu-id="beaa0-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="beaa0-125">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span></span>

|<span data-ttu-id="beaa0-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="beaa0-126">Property</span></span>|<span data-ttu-id="beaa0-127">Typ</span><span class="sxs-lookup"><span data-stu-id="beaa0-127">Type</span></span>|<span data-ttu-id="beaa0-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="beaa0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beaa0-129">id</span><span class="sxs-lookup"><span data-stu-id="beaa0-129">id</span></span>|<span data-ttu-id="beaa0-130">String</span><span class="sxs-lookup"><span data-stu-id="beaa0-130">String</span></span>|<span data-ttu-id="beaa0-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="beaa0-131">Key of the entity.</span></span> <span data-ttu-id="beaa0-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="beaa0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="beaa0-133">displayName</span></span>|<span data-ttu-id="beaa0-134">String</span><span class="sxs-lookup"><span data-stu-id="beaa0-134">String</span></span>|<span data-ttu-id="beaa0-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="beaa0-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="beaa0-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="beaa0-137">description</span><span class="sxs-lookup"><span data-stu-id="beaa0-137">description</span></span>|<span data-ttu-id="beaa0-138">String</span><span class="sxs-lookup"><span data-stu-id="beaa0-138">String</span></span>|<span data-ttu-id="beaa0-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="beaa0-139">The description of the app.</span></span> <span data-ttu-id="beaa0-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="beaa0-141">publisher</span><span class="sxs-lookup"><span data-stu-id="beaa0-141">publisher</span></span>|<span data-ttu-id="beaa0-142">String</span><span class="sxs-lookup"><span data-stu-id="beaa0-142">String</span></span>|<span data-ttu-id="beaa0-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="beaa0-143">The publisher of the app.</span></span> <span data-ttu-id="beaa0-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="beaa0-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="beaa0-145">largeIcon</span></span>|[<span data-ttu-id="beaa0-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="beaa0-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="beaa0-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="beaa0-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="beaa0-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="beaa0-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="beaa0-149">createdDateTime</span></span>|<span data-ttu-id="beaa0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="beaa0-150">DateTimeOffset</span></span>|<span data-ttu-id="beaa0-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="beaa0-151">The date and time the app was created.</span></span> <span data-ttu-id="beaa0-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="beaa0-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="beaa0-153">lastModifiedDateTime</span></span>|<span data-ttu-id="beaa0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="beaa0-154">DateTimeOffset</span></span>|<span data-ttu-id="beaa0-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="beaa0-155">The date and time the app was last modified.</span></span> <span data-ttu-id="beaa0-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="beaa0-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="beaa0-157">isFeatured</span></span>|<span data-ttu-id="beaa0-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="beaa0-158">Boolean</span></span>|<span data-ttu-id="beaa0-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="beaa0-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="beaa0-160">privacyInformationUrl</span></span>|<span data-ttu-id="beaa0-161">String</span><span class="sxs-lookup"><span data-stu-id="beaa0-161">String</span></span>|<span data-ttu-id="beaa0-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="beaa0-162">The privacy statement Url.</span></span> <span data-ttu-id="beaa0-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="beaa0-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="beaa0-164">informationUrl</span></span>|<span data-ttu-id="beaa0-165">String</span><span class="sxs-lookup"><span data-stu-id="beaa0-165">String</span></span>|<span data-ttu-id="beaa0-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="beaa0-166">The more information Url.</span></span> <span data-ttu-id="beaa0-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="beaa0-168">owner</span><span class="sxs-lookup"><span data-stu-id="beaa0-168">owner</span></span>|<span data-ttu-id="beaa0-169">String</span><span class="sxs-lookup"><span data-stu-id="beaa0-169">String</span></span>|<span data-ttu-id="beaa0-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="beaa0-170">The owner of the app.</span></span> <span data-ttu-id="beaa0-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="beaa0-172">developer</span><span class="sxs-lookup"><span data-stu-id="beaa0-172">developer</span></span>|<span data-ttu-id="beaa0-173">String</span><span class="sxs-lookup"><span data-stu-id="beaa0-173">String</span></span>|<span data-ttu-id="beaa0-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="beaa0-174">The developer of the app.</span></span> <span data-ttu-id="beaa0-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="beaa0-176">notes</span><span class="sxs-lookup"><span data-stu-id="beaa0-176">notes</span></span>|<span data-ttu-id="beaa0-177">String</span><span class="sxs-lookup"><span data-stu-id="beaa0-177">String</span></span>|<span data-ttu-id="beaa0-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="beaa0-178">Notes for the app.</span></span> <span data-ttu-id="beaa0-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="beaa0-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="beaa0-180">publishingState</span></span>|[<span data-ttu-id="beaa0-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="beaa0-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="beaa0-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="beaa0-182">The publishing state for the app.</span></span> <span data-ttu-id="beaa0-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="beaa0-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="beaa0-184">Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="beaa0-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="beaa0-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="beaa0-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="beaa0-186">appAvailability</span></span>|[<span data-ttu-id="beaa0-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="beaa0-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="beaa0-188">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="beaa0-188">The Application's availability.</span></span> <span data-ttu-id="beaa0-189">Geerbt von [ManagedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="beaa0-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md).</span></span> <span data-ttu-id="beaa0-190">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="beaa0-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="beaa0-191">version</span><span class="sxs-lookup"><span data-stu-id="beaa0-191">version</span></span>|<span data-ttu-id="beaa0-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="beaa0-192">String</span></span>|<span data-ttu-id="beaa0-193">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="beaa0-193">The Application's version.</span></span> <span data-ttu-id="beaa0-194">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="beaa0-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="beaa0-195">bundleId</span><span class="sxs-lookup"><span data-stu-id="beaa0-195">bundleId</span></span>|<span data-ttu-id="beaa0-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="beaa0-196">String</span></span>|<span data-ttu-id="beaa0-197">Die Bundle-ID einer App.</span><span class="sxs-lookup"><span data-stu-id="beaa0-197">The app's Bundle ID.</span></span>|
|<span data-ttu-id="beaa0-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="beaa0-198">appStoreUrl</span></span>|<span data-ttu-id="beaa0-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="beaa0-199">String</span></span>|<span data-ttu-id="beaa0-200">Die URL des Apple-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="beaa0-200">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="beaa0-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="beaa0-201">applicableDeviceType</span></span>|[<span data-ttu-id="beaa0-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="beaa0-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="beaa0-203">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="beaa0-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="beaa0-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="beaa0-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="beaa0-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="beaa0-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="beaa0-206">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="beaa0-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="beaa0-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="beaa0-207">Response</span></span>
<span data-ttu-id="beaa0-208">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="beaa0-208">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beaa0-209">Beispiel</span><span class="sxs-lookup"><span data-stu-id="beaa0-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="beaa0-210">Anforderung</span><span class="sxs-lookup"><span data-stu-id="beaa0-210">Request</span></span>
<span data-ttu-id="beaa0-211">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="beaa0-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1084

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
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="beaa0-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="beaa0-212">Response</span></span>
<span data-ttu-id="beaa0-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="beaa0-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1256

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
    "v11_0": true,
    "v12_0": true
  }
}
```



