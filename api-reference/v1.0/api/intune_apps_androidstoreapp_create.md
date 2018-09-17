# <a name="create-androidstoreapp"></a><span data-ttu-id="95530-101">Erstellen von „androidStoreApp“</span><span class="sxs-lookup"><span data-stu-id="95530-101">Create androidStoreApp</span></span>

> <span data-ttu-id="95530-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="95530-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95530-103">Diese Methode erstellt ein neues Objekt des Typs [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-103">Create a new [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95530-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="95530-104">Prerequisites</span></span>
<span data-ttu-id="95530-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="95530-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="95530-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="95530-107">Permission type</span></span>|<span data-ttu-id="95530-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="95530-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95530-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="95530-109">Delegated (work or school account)</span></span>|<span data-ttu-id="95530-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95530-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95530-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="95530-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95530-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="95530-112">Not supported.</span></span>|
|<span data-ttu-id="95530-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="95530-113">Application</span></span>|<span data-ttu-id="95530-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="95530-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95530-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="95530-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="95530-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="95530-116">Request headers</span></span>
|<span data-ttu-id="95530-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="95530-117">Header</span></span>|<span data-ttu-id="95530-118">Wert</span><span class="sxs-lookup"><span data-stu-id="95530-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95530-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="95530-119">Authorization</span></span>|<span data-ttu-id="95530-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="95530-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95530-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="95530-121">Accept</span></span>|<span data-ttu-id="95530-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="95530-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95530-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="95530-123">Request body</span></span>
<span data-ttu-id="95530-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidStoreApp“ an.</span><span class="sxs-lookup"><span data-stu-id="95530-124">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="95530-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidStoreApp“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="95530-125">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="95530-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="95530-126">Property</span></span>|<span data-ttu-id="95530-127">Typ</span><span class="sxs-lookup"><span data-stu-id="95530-127">Type</span></span>|<span data-ttu-id="95530-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95530-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95530-129">ID</span><span class="sxs-lookup"><span data-stu-id="95530-129">id</span></span>|<span data-ttu-id="95530-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95530-130">String</span></span>|<span data-ttu-id="95530-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="95530-131">Key of the entity.</span></span> <span data-ttu-id="95530-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95530-133">displayName</span><span class="sxs-lookup"><span data-stu-id="95530-133">displayName</span></span>|<span data-ttu-id="95530-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95530-134">String</span></span>|<span data-ttu-id="95530-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="95530-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="95530-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95530-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95530-137">description</span></span>|<span data-ttu-id="95530-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95530-138">String</span></span>|<span data-ttu-id="95530-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="95530-139">The description of the app.</span></span> <span data-ttu-id="95530-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95530-141">Verleger</span><span class="sxs-lookup"><span data-stu-id="95530-141">publisher</span></span>|<span data-ttu-id="95530-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95530-142">String</span></span>|<span data-ttu-id="95530-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="95530-143">The publisher of the app.</span></span> <span data-ttu-id="95530-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95530-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="95530-145">largeIcon</span></span>|[<span data-ttu-id="95530-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="95530-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="95530-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="95530-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="95530-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95530-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95530-149">createdDateTime</span></span>|<span data-ttu-id="95530-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95530-150">DateTimeOffset</span></span>|<span data-ttu-id="95530-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="95530-151">The date and time the app was created.</span></span> <span data-ttu-id="95530-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95530-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95530-153">lastModifiedDateTime</span></span>|<span data-ttu-id="95530-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95530-154">DateTimeOffset</span></span>|<span data-ttu-id="95530-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="95530-155">The date and time the app was last modified.</span></span> <span data-ttu-id="95530-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95530-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="95530-157">isFeatured</span></span>|<span data-ttu-id="95530-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="95530-158">Boolean</span></span>|<span data-ttu-id="95530-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95530-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="95530-160">privacyInformationUrl</span></span>|<span data-ttu-id="95530-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95530-161">String</span></span>|<span data-ttu-id="95530-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="95530-162">The privacy statement Url.</span></span> <span data-ttu-id="95530-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95530-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="95530-164">informationUrl</span></span>|<span data-ttu-id="95530-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95530-165">String</span></span>|<span data-ttu-id="95530-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="95530-166">The more information Url.</span></span> <span data-ttu-id="95530-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95530-168">Besitzer</span><span class="sxs-lookup"><span data-stu-id="95530-168">owner</span></span>|<span data-ttu-id="95530-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95530-169">String</span></span>|<span data-ttu-id="95530-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="95530-170">The owner of the app.</span></span> <span data-ttu-id="95530-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95530-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="95530-172">developer</span></span>|<span data-ttu-id="95530-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95530-173">String</span></span>|<span data-ttu-id="95530-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="95530-174">The developer of the app.</span></span> <span data-ttu-id="95530-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95530-176">Notizen</span><span class="sxs-lookup"><span data-stu-id="95530-176">notes</span></span>|<span data-ttu-id="95530-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95530-177">String</span></span>|<span data-ttu-id="95530-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="95530-178">Notes for the app.</span></span> <span data-ttu-id="95530-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95530-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="95530-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="95530-180">publishingState</span></span>|[<span data-ttu-id="95530-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="95530-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="95530-p114">Der Veröffentlichungsstand der App. Die App kann nur dann zugewiesen werden, wenn die App veröffentlicht wird. Vererbt von [mobileApp](../resources/intune_apps_mobileapp.md). Die möglichen Werte sind: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="95530-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="95530-186">packageId</span><span class="sxs-lookup"><span data-stu-id="95530-186">packageId</span></span>|<span data-ttu-id="95530-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95530-187">String</span></span>|<span data-ttu-id="95530-188">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="95530-188">The package identifier.</span></span>|
|<span data-ttu-id="95530-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="95530-189">appStoreUrl</span></span>|<span data-ttu-id="95530-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95530-190">String</span></span>|<span data-ttu-id="95530-191">URL zum App-Store von Android</span><span class="sxs-lookup"><span data-stu-id="95530-191">The Android app store URL.</span></span>|
|<span data-ttu-id="95530-192">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="95530-192">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="95530-193">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="95530-193">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="95530-194">Wert, der angibt, welche Betriebssystemversion mindestens erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="95530-194">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="95530-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="95530-195">Response</span></span>
<span data-ttu-id="95530-196">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidStoreApp](../resources/intune_apps_androidstoreapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="95530-196">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95530-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="95530-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="95530-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="95530-198">Request</span></span>
<span data-ttu-id="95530-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="95530-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1002

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

### <a name="response"></a><span data-ttu-id="95530-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="95530-200">Response</span></span>
<span data-ttu-id="95530-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="95530-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








