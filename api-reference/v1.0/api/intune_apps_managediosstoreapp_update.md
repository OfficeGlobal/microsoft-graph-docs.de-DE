# <a name="update-managediosstoreapp"></a><span data-ttu-id="6ca66-101">managedIOSStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6ca66-101">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="6ca66-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6ca66-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ca66-103">Aktualisieren der Eigenschaften eines [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6ca66-103">Update the properties of a [calendar](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ca66-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6ca66-104">Prerequisites</span></span>
<span data-ttu-id="6ca66-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6ca66-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6ca66-107">Permission type</span></span>|<span data-ttu-id="6ca66-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6ca66-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ca66-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6ca66-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6ca66-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ca66-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6ca66-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6ca66-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ca66-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6ca66-112">Not supported.</span></span>|
|<span data-ttu-id="6ca66-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6ca66-113">Application</span></span>|<span data-ttu-id="6ca66-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6ca66-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ca66-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ca66-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="6ca66-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6ca66-116">Request headers</span></span>
|<span data-ttu-id="6ca66-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6ca66-117">Header</span></span>|<span data-ttu-id="6ca66-118">Wert</span><span class="sxs-lookup"><span data-stu-id="6ca66-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ca66-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ca66-119">Authorization</span></span>|<span data-ttu-id="6ca66-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6ca66-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6ca66-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6ca66-121">Accept</span></span>|<span data-ttu-id="6ca66-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6ca66-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ca66-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6ca66-123">Request body</span></span>
<span data-ttu-id="6ca66-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="6ca66-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_managediosstoreapp.md) object.</span></span>

<span data-ttu-id="6ca66-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6ca66-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="6ca66-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ca66-126">Property</span></span>|<span data-ttu-id="6ca66-127">Typ</span><span class="sxs-lookup"><span data-stu-id="6ca66-127">Type</span></span>|<span data-ttu-id="6ca66-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ca66-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ca66-129">id</span><span class="sxs-lookup"><span data-stu-id="6ca66-129">id</span></span>|<span data-ttu-id="6ca66-130">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-130">String</span></span>|<span data-ttu-id="6ca66-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="6ca66-131">Key of the setting.</span></span> <span data-ttu-id="6ca66-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6ca66-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6ca66-133">displayName</span></span>|<span data-ttu-id="6ca66-134">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-134">String</span></span>|<span data-ttu-id="6ca66-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="6ca66-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6ca66-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6ca66-137">description</span><span class="sxs-lookup"><span data-stu-id="6ca66-137">description</span></span>|<span data-ttu-id="6ca66-138">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-138">String</span></span>|<span data-ttu-id="6ca66-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="6ca66-139">The description of the app.</span></span> <span data-ttu-id="6ca66-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6ca66-141">publisher</span><span class="sxs-lookup"><span data-stu-id="6ca66-141">Publisher</span></span>|<span data-ttu-id="6ca66-142">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-142">String</span></span>|<span data-ttu-id="6ca66-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="6ca66-143">The name of the app.</span></span> <span data-ttu-id="6ca66-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6ca66-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6ca66-145">largeIcon</span></span>|[<span data-ttu-id="6ca66-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6ca66-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="6ca66-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="6ca66-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6ca66-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6ca66-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ca66-149">createdDateTime</span></span>|<span data-ttu-id="6ca66-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ca66-150">DateTimeOffset</span></span>|<span data-ttu-id="6ca66-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="6ca66-151">The date and time the group was created.</span></span> <span data-ttu-id="6ca66-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6ca66-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ca66-153">lastModifiedDateTime</span></span>|<span data-ttu-id="6ca66-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ca66-154">DateTimeOffset</span></span>|<span data-ttu-id="6ca66-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="6ca66-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="6ca66-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6ca66-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6ca66-157">isFeatured</span></span>|<span data-ttu-id="6ca66-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ca66-158">Boolean</span></span>|<span data-ttu-id="6ca66-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6ca66-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6ca66-160">privacyInformationUrl</span></span>|<span data-ttu-id="6ca66-161">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-161">String</span></span>|<span data-ttu-id="6ca66-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="6ca66-162">The privacy statement Url.</span></span> <span data-ttu-id="6ca66-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6ca66-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6ca66-164">informationUrl</span></span>|<span data-ttu-id="6ca66-165">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-165">String</span></span>|<span data-ttu-id="6ca66-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="6ca66-166">The more information Url.</span></span> <span data-ttu-id="6ca66-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6ca66-168">owner</span><span class="sxs-lookup"><span data-stu-id="6ca66-168">owner</span></span>|<span data-ttu-id="6ca66-169">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-169">String</span></span>|<span data-ttu-id="6ca66-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="6ca66-170">The owner of the app.</span></span> <span data-ttu-id="6ca66-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6ca66-172">developer</span><span class="sxs-lookup"><span data-stu-id="6ca66-172">developer</span></span>|<span data-ttu-id="6ca66-173">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-173">String</span></span>|<span data-ttu-id="6ca66-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="6ca66-174">The name of the app.</span></span> <span data-ttu-id="6ca66-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6ca66-176">notes</span><span class="sxs-lookup"><span data-stu-id="6ca66-176">notes</span></span>|<span data-ttu-id="6ca66-177">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-177">String</span></span>|<span data-ttu-id="6ca66-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="6ca66-178">Notes for the app.</span></span> <span data-ttu-id="6ca66-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6ca66-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6ca66-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="6ca66-180">publishingState</span></span>|<span data-ttu-id="6ca66-181">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-181">String</span></span>|<span data-ttu-id="6ca66-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="6ca66-182">The publishing state for the app.</span></span> <span data-ttu-id="6ca66-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="6ca66-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6ca66-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="6ca66-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6ca66-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="6ca66-185">appAvailability</span></span>|<span data-ttu-id="6ca66-186">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-186">String</span></span>|<span data-ttu-id="6ca66-187">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="6ca66-187">The Application's availability.</span></span> <span data-ttu-id="6ca66-188">Geerbt von [managedApp](../resources/intune_apps_managedapp.md). Mögliche Werte sind: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="6ca66-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="6ca66-189">Version</span><span class="sxs-lookup"><span data-stu-id="6ca66-189">version</span></span>|<span data-ttu-id="6ca66-190">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-190">String</span></span>|<span data-ttu-id="6ca66-191">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="6ca66-191">The Application's version.</span></span> <span data-ttu-id="6ca66-192">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="6ca66-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="6ca66-193">bundleId</span><span class="sxs-lookup"><span data-stu-id="6ca66-193">bundleId</span></span>|<span data-ttu-id="6ca66-194">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-194">String</span></span>|<span data-ttu-id="6ca66-195">Die Bundle-ID einer App.</span><span class="sxs-lookup"><span data-stu-id="6ca66-195">The app's Bundle ID.</span></span>|
|<span data-ttu-id="6ca66-196">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6ca66-196">appStoreUrl</span></span>|<span data-ttu-id="6ca66-197">String</span><span class="sxs-lookup"><span data-stu-id="6ca66-197">String</span></span>|<span data-ttu-id="6ca66-198">Die URL des Apple-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="6ca66-198">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="6ca66-199">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="6ca66-199">applicableDeviceType</span></span>|[<span data-ttu-id="6ca66-200">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="6ca66-200">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="6ca66-201">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="6ca66-201">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="6ca66-202">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6ca66-202">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6ca66-203">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6ca66-203">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="6ca66-204">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="6ca66-204">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="6ca66-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ca66-205">Response</span></span>
<span data-ttu-id="6ca66-206">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6ca66-206">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ca66-207">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6ca66-207">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ca66-208">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ca66-208">Request</span></span>
<span data-ttu-id="6ca66-209">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6ca66-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1071

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

### <a name="response"></a><span data-ttu-id="6ca66-210">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ca66-210">Response</span></span>
<span data-ttu-id="6ca66-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6ca66-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



