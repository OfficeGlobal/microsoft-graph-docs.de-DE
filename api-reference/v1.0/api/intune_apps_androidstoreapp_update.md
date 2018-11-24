# <a name="update-androidstoreapp"></a><span data-ttu-id="0ce58-101">androidStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0ce58-101">Update androidStoreApp</span></span>

> <span data-ttu-id="0ce58-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0ce58-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ce58-103">Aktualisieren der Eigenschaften eines [androidStoreApp](../resources/intune_apps_androidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0ce58-103">Update the properties of a [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ce58-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0ce58-104">Prerequisites</span></span>
<span data-ttu-id="0ce58-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0ce58-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0ce58-107">Permission type</span></span>|<span data-ttu-id="0ce58-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0ce58-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ce58-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0ce58-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0ce58-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ce58-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0ce58-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0ce58-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ce58-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ce58-112">Not supported.</span></span>|
|<span data-ttu-id="0ce58-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0ce58-113">Application</span></span>|<span data-ttu-id="0ce58-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ce58-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ce58-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ce58-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="0ce58-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0ce58-116">Request headers</span></span>
|<span data-ttu-id="0ce58-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0ce58-117">Header</span></span>|<span data-ttu-id="0ce58-118">Wert</span><span class="sxs-lookup"><span data-stu-id="0ce58-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ce58-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ce58-119">Authorization</span></span>|<span data-ttu-id="0ce58-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0ce58-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ce58-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0ce58-121">Accept</span></span>|<span data-ttu-id="0ce58-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0ce58-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ce58-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0ce58-123">Request body</span></span>
<span data-ttu-id="0ce58-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidStoreApp](../resources/intune_apps_androidstoreapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="0ce58-124">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>

<span data-ttu-id="0ce58-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidStoreApp](../resources/intune_apps_androidstoreapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="0ce58-125">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span></span>

|<span data-ttu-id="0ce58-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0ce58-126">Property</span></span>|<span data-ttu-id="0ce58-127">Typ</span><span class="sxs-lookup"><span data-stu-id="0ce58-127">Type</span></span>|<span data-ttu-id="0ce58-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ce58-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ce58-129">id</span><span class="sxs-lookup"><span data-stu-id="0ce58-129">id</span></span>|<span data-ttu-id="0ce58-130">String</span><span class="sxs-lookup"><span data-stu-id="0ce58-130">String</span></span>|<span data-ttu-id="0ce58-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="0ce58-131">Key of the entity.</span></span> <span data-ttu-id="0ce58-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0ce58-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0ce58-133">displayName</span></span>|<span data-ttu-id="0ce58-134">String</span><span class="sxs-lookup"><span data-stu-id="0ce58-134">String</span></span>|<span data-ttu-id="0ce58-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="0ce58-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0ce58-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0ce58-137">description</span><span class="sxs-lookup"><span data-stu-id="0ce58-137">description</span></span>|<span data-ttu-id="0ce58-138">String</span><span class="sxs-lookup"><span data-stu-id="0ce58-138">String</span></span>|<span data-ttu-id="0ce58-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="0ce58-139">The description of the app.</span></span> <span data-ttu-id="0ce58-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0ce58-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="0ce58-141">publisher</span></span>|<span data-ttu-id="0ce58-142">String</span><span class="sxs-lookup"><span data-stu-id="0ce58-142">String</span></span>|<span data-ttu-id="0ce58-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="0ce58-143">The publisher of the app.</span></span> <span data-ttu-id="0ce58-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0ce58-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0ce58-145">largeIcon</span></span>|[<span data-ttu-id="0ce58-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0ce58-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="0ce58-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="0ce58-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0ce58-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0ce58-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ce58-149">createdDateTime</span></span>|<span data-ttu-id="0ce58-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ce58-150">DateTimeOffset</span></span>|<span data-ttu-id="0ce58-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="0ce58-151">The date and time the app was created.</span></span> <span data-ttu-id="0ce58-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0ce58-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ce58-153">lastModifiedDateTime</span></span>|<span data-ttu-id="0ce58-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ce58-154">DateTimeOffset</span></span>|<span data-ttu-id="0ce58-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="0ce58-155">The date and time the app was last modified.</span></span> <span data-ttu-id="0ce58-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0ce58-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0ce58-157">isFeatured</span></span>|<span data-ttu-id="0ce58-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ce58-158">Boolean</span></span>|<span data-ttu-id="0ce58-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0ce58-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0ce58-160">privacyInformationUrl</span></span>|<span data-ttu-id="0ce58-161">String</span><span class="sxs-lookup"><span data-stu-id="0ce58-161">String</span></span>|<span data-ttu-id="0ce58-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="0ce58-162">The privacy statement Url.</span></span> <span data-ttu-id="0ce58-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0ce58-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0ce58-164">informationUrl</span></span>|<span data-ttu-id="0ce58-165">String</span><span class="sxs-lookup"><span data-stu-id="0ce58-165">String</span></span>|<span data-ttu-id="0ce58-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="0ce58-166">The more information Url.</span></span> <span data-ttu-id="0ce58-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0ce58-168">owner</span><span class="sxs-lookup"><span data-stu-id="0ce58-168">owner</span></span>|<span data-ttu-id="0ce58-169">String</span><span class="sxs-lookup"><span data-stu-id="0ce58-169">String</span></span>|<span data-ttu-id="0ce58-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="0ce58-170">The owner of the app.</span></span> <span data-ttu-id="0ce58-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0ce58-172">developer</span><span class="sxs-lookup"><span data-stu-id="0ce58-172">developer</span></span>|<span data-ttu-id="0ce58-173">String</span><span class="sxs-lookup"><span data-stu-id="0ce58-173">String</span></span>|<span data-ttu-id="0ce58-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="0ce58-174">The developer of the app.</span></span> <span data-ttu-id="0ce58-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0ce58-176">notes</span><span class="sxs-lookup"><span data-stu-id="0ce58-176">notes</span></span>|<span data-ttu-id="0ce58-177">String</span><span class="sxs-lookup"><span data-stu-id="0ce58-177">String</span></span>|<span data-ttu-id="0ce58-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="0ce58-178">Notes for the app.</span></span> <span data-ttu-id="0ce58-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0ce58-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="0ce58-180">publishingState</span></span>|[<span data-ttu-id="0ce58-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0ce58-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="0ce58-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="0ce58-182">The publishing state for the app.</span></span> <span data-ttu-id="0ce58-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="0ce58-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0ce58-184">Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0ce58-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="0ce58-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="0ce58-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0ce58-186">packageId</span><span class="sxs-lookup"><span data-stu-id="0ce58-186">packageId</span></span>|<span data-ttu-id="0ce58-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ce58-187">String</span></span>|<span data-ttu-id="0ce58-188">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="0ce58-188">The package identifier.</span></span>|
|<span data-ttu-id="0ce58-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0ce58-189">appStoreUrl</span></span>|<span data-ttu-id="0ce58-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0ce58-190">String</span></span>|<span data-ttu-id="0ce58-191">URL zum App-Store von Android</span><span class="sxs-lookup"><span data-stu-id="0ce58-191">The Android app store URL.</span></span>|
|<span data-ttu-id="0ce58-192">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0ce58-192">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0ce58-193">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0ce58-193">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="0ce58-194">Wert, der angibt, welche Betriebssystemversion mindestens erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="0ce58-194">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="0ce58-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ce58-195">Response</span></span>
<span data-ttu-id="0ce58-196">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidStoreApp](../resources/intune_apps_androidstoreapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0ce58-196">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ce58-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0ce58-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ce58-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ce58-198">Request</span></span>
<span data-ttu-id="0ce58-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0ce58-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 938

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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

### <a name="response"></a><span data-ttu-id="0ce58-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ce58-200">Response</span></span>
<span data-ttu-id="0ce58-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ce58-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1110

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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



