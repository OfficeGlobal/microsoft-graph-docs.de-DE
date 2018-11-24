# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="c5e94-101">managedAndroidStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c5e94-101">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="c5e94-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c5e94-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5e94-103">Aktualisieren der Eigenschaften eines [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c5e94-103">Update the properties of a [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5e94-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c5e94-104">Prerequisites</span></span>
<span data-ttu-id="c5e94-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c5e94-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c5e94-107">Permission type</span></span>|<span data-ttu-id="c5e94-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c5e94-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5e94-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c5e94-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c5e94-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5e94-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c5e94-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c5e94-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5e94-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5e94-112">Not supported.</span></span>|
|<span data-ttu-id="c5e94-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c5e94-113">Application</span></span>|<span data-ttu-id="c5e94-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5e94-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5e94-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5e94-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="c5e94-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5e94-116">Request headers</span></span>
|<span data-ttu-id="c5e94-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c5e94-117">Header</span></span>|<span data-ttu-id="c5e94-118">Wert</span><span class="sxs-lookup"><span data-stu-id="c5e94-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5e94-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5e94-119">Authorization</span></span>|<span data-ttu-id="c5e94-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c5e94-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5e94-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c5e94-121">Accept</span></span>|<span data-ttu-id="c5e94-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c5e94-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5e94-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c5e94-123">Request body</span></span>
<span data-ttu-id="c5e94-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c5e94-124">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="c5e94-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c5e94-125">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="c5e94-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5e94-126">Property</span></span>|<span data-ttu-id="c5e94-127">Typ</span><span class="sxs-lookup"><span data-stu-id="c5e94-127">Type</span></span>|<span data-ttu-id="c5e94-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5e94-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5e94-129">id</span><span class="sxs-lookup"><span data-stu-id="c5e94-129">id</span></span>|<span data-ttu-id="c5e94-130">String</span><span class="sxs-lookup"><span data-stu-id="c5e94-130">String</span></span>|<span data-ttu-id="c5e94-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="c5e94-131">Key of the entity.</span></span> <span data-ttu-id="c5e94-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c5e94-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c5e94-133">displayName</span></span>|<span data-ttu-id="c5e94-134">String</span><span class="sxs-lookup"><span data-stu-id="c5e94-134">String</span></span>|<span data-ttu-id="c5e94-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="c5e94-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c5e94-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c5e94-137">description</span><span class="sxs-lookup"><span data-stu-id="c5e94-137">description</span></span>|<span data-ttu-id="c5e94-138">String</span><span class="sxs-lookup"><span data-stu-id="c5e94-138">String</span></span>|<span data-ttu-id="c5e94-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="c5e94-139">The description of the app.</span></span> <span data-ttu-id="c5e94-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c5e94-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="c5e94-141">publisher</span></span>|<span data-ttu-id="c5e94-142">String</span><span class="sxs-lookup"><span data-stu-id="c5e94-142">String</span></span>|<span data-ttu-id="c5e94-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="c5e94-143">The publisher of the app.</span></span> <span data-ttu-id="c5e94-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c5e94-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c5e94-145">largeIcon</span></span>|[<span data-ttu-id="c5e94-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c5e94-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="c5e94-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c5e94-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c5e94-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c5e94-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5e94-149">createdDateTime</span></span>|<span data-ttu-id="c5e94-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5e94-150">DateTimeOffset</span></span>|<span data-ttu-id="c5e94-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="c5e94-151">The date and time the app was created.</span></span> <span data-ttu-id="c5e94-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c5e94-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5e94-153">lastModifiedDateTime</span></span>|<span data-ttu-id="c5e94-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5e94-154">DateTimeOffset</span></span>|<span data-ttu-id="c5e94-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="c5e94-155">The date and time the app was last modified.</span></span> <span data-ttu-id="c5e94-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c5e94-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c5e94-157">isFeatured</span></span>|<span data-ttu-id="c5e94-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5e94-158">Boolean</span></span>|<span data-ttu-id="c5e94-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c5e94-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c5e94-160">privacyInformationUrl</span></span>|<span data-ttu-id="c5e94-161">String</span><span class="sxs-lookup"><span data-stu-id="c5e94-161">String</span></span>|<span data-ttu-id="c5e94-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="c5e94-162">The privacy statement Url.</span></span> <span data-ttu-id="c5e94-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c5e94-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c5e94-164">informationUrl</span></span>|<span data-ttu-id="c5e94-165">String</span><span class="sxs-lookup"><span data-stu-id="c5e94-165">String</span></span>|<span data-ttu-id="c5e94-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="c5e94-166">The more information Url.</span></span> <span data-ttu-id="c5e94-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c5e94-168">owner</span><span class="sxs-lookup"><span data-stu-id="c5e94-168">owner</span></span>|<span data-ttu-id="c5e94-169">String</span><span class="sxs-lookup"><span data-stu-id="c5e94-169">String</span></span>|<span data-ttu-id="c5e94-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="c5e94-170">The owner of the app.</span></span> <span data-ttu-id="c5e94-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c5e94-172">developer</span><span class="sxs-lookup"><span data-stu-id="c5e94-172">developer</span></span>|<span data-ttu-id="c5e94-173">String</span><span class="sxs-lookup"><span data-stu-id="c5e94-173">String</span></span>|<span data-ttu-id="c5e94-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="c5e94-174">The developer of the app.</span></span> <span data-ttu-id="c5e94-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c5e94-176">notes</span><span class="sxs-lookup"><span data-stu-id="c5e94-176">notes</span></span>|<span data-ttu-id="c5e94-177">String</span><span class="sxs-lookup"><span data-stu-id="c5e94-177">String</span></span>|<span data-ttu-id="c5e94-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="c5e94-178">Notes for the app.</span></span> <span data-ttu-id="c5e94-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c5e94-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="c5e94-180">publishingState</span></span>|[<span data-ttu-id="c5e94-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c5e94-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="c5e94-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="c5e94-182">The publishing state for the app.</span></span> <span data-ttu-id="c5e94-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="c5e94-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c5e94-184">Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="c5e94-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="c5e94-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c5e94-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="c5e94-186">appAvailability</span></span>|[<span data-ttu-id="c5e94-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="c5e94-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="c5e94-188">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="c5e94-188">The Application's availability.</span></span> <span data-ttu-id="c5e94-189">Geerbt von [ManagedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5e94-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md).</span></span> <span data-ttu-id="c5e94-190">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="c5e94-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="c5e94-191">version</span><span class="sxs-lookup"><span data-stu-id="c5e94-191">version</span></span>|<span data-ttu-id="c5e94-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5e94-192">String</span></span>|<span data-ttu-id="c5e94-193">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="c5e94-193">The Application's version.</span></span> <span data-ttu-id="c5e94-194">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c5e94-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="c5e94-195">packageId</span><span class="sxs-lookup"><span data-stu-id="c5e94-195">packageId</span></span>|<span data-ttu-id="c5e94-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5e94-196">String</span></span>|<span data-ttu-id="c5e94-197">Die Paket-ID der App.</span><span class="sxs-lookup"><span data-stu-id="c5e94-197">The app's package ID.</span></span>|
|<span data-ttu-id="c5e94-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c5e94-198">appStoreUrl</span></span>|<span data-ttu-id="c5e94-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5e94-199">String</span></span>|<span data-ttu-id="c5e94-200">Die URL des Android-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="c5e94-200">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="c5e94-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c5e94-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c5e94-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c5e94-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="c5e94-203">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="c5e94-203">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="c5e94-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5e94-204">Response</span></span>
<span data-ttu-id="c5e94-205">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5e94-205">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5e94-206">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5e94-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5e94-207">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5e94-207">Request</span></span>
<span data-ttu-id="c5e94-208">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5e94-208">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1016

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

### <a name="response"></a><span data-ttu-id="c5e94-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5e94-209">Response</span></span>
<span data-ttu-id="c5e94-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5e94-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



