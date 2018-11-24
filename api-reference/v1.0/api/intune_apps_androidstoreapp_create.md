# <a name="create-androidstoreapp"></a><span data-ttu-id="5bd6c-101">Erstellen von „androidStoreApp“</span><span class="sxs-lookup"><span data-stu-id="5bd6c-101">Create androidStoreApp</span></span>

> <span data-ttu-id="5bd6c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5bd6c-103">Diese Methode erstellt ein neues Objekt des Typs [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-103">Create a new [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5bd6c-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5bd6c-104">Prerequisites</span></span>
<span data-ttu-id="5bd6c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5bd6c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5bd6c-107">Permission type</span></span>|<span data-ttu-id="5bd6c-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5bd6c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bd6c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5bd6c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5bd6c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bd6c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5bd6c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5bd6c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bd6c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5bd6c-112">Not supported.</span></span>|
|<span data-ttu-id="5bd6c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5bd6c-113">Application</span></span>|<span data-ttu-id="5bd6c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5bd6c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bd6c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5bd6c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5bd6c-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5bd6c-116">Request headers</span></span>
|<span data-ttu-id="5bd6c-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5bd6c-117">Header</span></span>|<span data-ttu-id="5bd6c-118">Wert</span><span class="sxs-lookup"><span data-stu-id="5bd6c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bd6c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bd6c-119">Authorization</span></span>|<span data-ttu-id="5bd6c-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5bd6c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bd6c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5bd6c-121">Accept</span></span>|<span data-ttu-id="5bd6c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5bd6c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bd6c-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5bd6c-123">Request body</span></span>
<span data-ttu-id="5bd6c-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidStoreApp“ an.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-124">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="5bd6c-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidStoreApp“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-125">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="5bd6c-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5bd6c-126">Property</span></span>|<span data-ttu-id="5bd6c-127">Typ</span><span class="sxs-lookup"><span data-stu-id="5bd6c-127">Type</span></span>|<span data-ttu-id="5bd6c-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5bd6c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bd6c-129">id</span><span class="sxs-lookup"><span data-stu-id="5bd6c-129">id</span></span>|<span data-ttu-id="5bd6c-130">String</span><span class="sxs-lookup"><span data-stu-id="5bd6c-130">String</span></span>|<span data-ttu-id="5bd6c-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-131">Key of the entity.</span></span> <span data-ttu-id="5bd6c-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5bd6c-133">displayName</span></span>|<span data-ttu-id="5bd6c-134">String</span><span class="sxs-lookup"><span data-stu-id="5bd6c-134">String</span></span>|<span data-ttu-id="5bd6c-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5bd6c-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6c-137">description</span><span class="sxs-lookup"><span data-stu-id="5bd6c-137">description</span></span>|<span data-ttu-id="5bd6c-138">String</span><span class="sxs-lookup"><span data-stu-id="5bd6c-138">String</span></span>|<span data-ttu-id="5bd6c-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-139">The description of the app.</span></span> <span data-ttu-id="5bd6c-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6c-141">publisher</span><span class="sxs-lookup"><span data-stu-id="5bd6c-141">publisher</span></span>|<span data-ttu-id="5bd6c-142">String</span><span class="sxs-lookup"><span data-stu-id="5bd6c-142">String</span></span>|<span data-ttu-id="5bd6c-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-143">The publisher of the app.</span></span> <span data-ttu-id="5bd6c-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6c-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5bd6c-145">largeIcon</span></span>|[<span data-ttu-id="5bd6c-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5bd6c-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="5bd6c-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5bd6c-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6c-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd6c-149">createdDateTime</span></span>|<span data-ttu-id="5bd6c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd6c-150">DateTimeOffset</span></span>|<span data-ttu-id="5bd6c-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-151">The date and time the app was created.</span></span> <span data-ttu-id="5bd6c-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6c-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd6c-153">lastModifiedDateTime</span></span>|<span data-ttu-id="5bd6c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd6c-154">DateTimeOffset</span></span>|<span data-ttu-id="5bd6c-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-155">The date and time the app was last modified.</span></span> <span data-ttu-id="5bd6c-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6c-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5bd6c-157">isFeatured</span></span>|<span data-ttu-id="5bd6c-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bd6c-158">Boolean</span></span>|<span data-ttu-id="5bd6c-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6c-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5bd6c-160">privacyInformationUrl</span></span>|<span data-ttu-id="5bd6c-161">String</span><span class="sxs-lookup"><span data-stu-id="5bd6c-161">String</span></span>|<span data-ttu-id="5bd6c-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-162">The privacy statement Url.</span></span> <span data-ttu-id="5bd6c-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6c-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5bd6c-164">informationUrl</span></span>|<span data-ttu-id="5bd6c-165">String</span><span class="sxs-lookup"><span data-stu-id="5bd6c-165">String</span></span>|<span data-ttu-id="5bd6c-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-166">The more information Url.</span></span> <span data-ttu-id="5bd6c-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6c-168">owner</span><span class="sxs-lookup"><span data-stu-id="5bd6c-168">owner</span></span>|<span data-ttu-id="5bd6c-169">String</span><span class="sxs-lookup"><span data-stu-id="5bd6c-169">String</span></span>|<span data-ttu-id="5bd6c-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-170">The owner of the app.</span></span> <span data-ttu-id="5bd6c-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6c-172">developer</span><span class="sxs-lookup"><span data-stu-id="5bd6c-172">developer</span></span>|<span data-ttu-id="5bd6c-173">String</span><span class="sxs-lookup"><span data-stu-id="5bd6c-173">String</span></span>|<span data-ttu-id="5bd6c-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-174">The developer of the app.</span></span> <span data-ttu-id="5bd6c-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6c-176">notes</span><span class="sxs-lookup"><span data-stu-id="5bd6c-176">notes</span></span>|<span data-ttu-id="5bd6c-177">String</span><span class="sxs-lookup"><span data-stu-id="5bd6c-177">String</span></span>|<span data-ttu-id="5bd6c-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-178">Notes for the app.</span></span> <span data-ttu-id="5bd6c-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5bd6c-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="5bd6c-180">publishingState</span></span>|[<span data-ttu-id="5bd6c-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5bd6c-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="5bd6c-182">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-182">The publishing state for the app.</span></span> <span data-ttu-id="5bd6c-183">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5bd6c-184">Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bd6c-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="5bd6c-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5bd6c-186">packageId</span><span class="sxs-lookup"><span data-stu-id="5bd6c-186">packageId</span></span>|<span data-ttu-id="5bd6c-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5bd6c-187">String</span></span>|<span data-ttu-id="5bd6c-188">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="5bd6c-188">The package identifier.</span></span>|
|<span data-ttu-id="5bd6c-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5bd6c-189">appStoreUrl</span></span>|<span data-ttu-id="5bd6c-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5bd6c-190">String</span></span>|<span data-ttu-id="5bd6c-191">URL zum App-Store von Android</span><span class="sxs-lookup"><span data-stu-id="5bd6c-191">The Android app store URL.</span></span>|
|<span data-ttu-id="5bd6c-192">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5bd6c-192">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5bd6c-193">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5bd6c-193">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="5bd6c-194">Wert, der angibt, welche Betriebssystemversion mindestens erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="5bd6c-194">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="5bd6c-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="5bd6c-195">Response</span></span>
<span data-ttu-id="5bd6c-196">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidStoreApp](../resources/intune_apps_androidstoreapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-196">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bd6c-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5bd6c-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="5bd6c-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5bd6c-198">Request</span></span>
<span data-ttu-id="5bd6c-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="5bd6c-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="5bd6c-200">Response</span></span>
<span data-ttu-id="5bd6c-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5bd6c-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



