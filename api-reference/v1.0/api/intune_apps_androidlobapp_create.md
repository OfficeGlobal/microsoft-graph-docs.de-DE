# <a name="create-androidlobapp"></a><span data-ttu-id="76db4-101">AndroidLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="76db4-101">Create androidLobApp</span></span>

> <span data-ttu-id="76db4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="76db4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76db4-103">Erstellen eines neuen [androidLobApp](../resources/intune_apps_androidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="76db4-103">Create a new [androidLobApp](../resources/intune_apps_androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="76db4-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="76db4-104">Prerequisites</span></span>
<span data-ttu-id="76db4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="76db4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="76db4-107">Permission type</span></span>|<span data-ttu-id="76db4-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="76db4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76db4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="76db4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="76db4-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76db4-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="76db4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="76db4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76db4-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76db4-112">Not supported.</span></span>|
|<span data-ttu-id="76db4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="76db4-113">Application</span></span>|<span data-ttu-id="76db4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76db4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76db4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="76db4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="76db4-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="76db4-116">Request headers</span></span>
|<span data-ttu-id="76db4-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="76db4-117">Header</span></span>|<span data-ttu-id="76db4-118">Wert</span><span class="sxs-lookup"><span data-stu-id="76db4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76db4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="76db4-119">Authorization</span></span>|<span data-ttu-id="76db4-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="76db4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76db4-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="76db4-121">Accept</span></span>|<span data-ttu-id="76db4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="76db4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76db4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="76db4-123">Request body</span></span>
<span data-ttu-id="76db4-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs androidLobApp an.</span><span class="sxs-lookup"><span data-stu-id="76db4-124">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="76db4-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs androidLobApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="76db4-125">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="76db4-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="76db4-126">Property</span></span>|<span data-ttu-id="76db4-127">Typ</span><span class="sxs-lookup"><span data-stu-id="76db4-127">Type</span></span>|<span data-ttu-id="76db4-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76db4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76db4-129">id</span><span class="sxs-lookup"><span data-stu-id="76db4-129">id</span></span>|<span data-ttu-id="76db4-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-130">String</span></span>|<span data-ttu-id="76db4-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="76db4-131">Key of the entity.</span></span> <span data-ttu-id="76db4-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="76db4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="76db4-133">displayName</span></span>|<span data-ttu-id="76db4-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-134">String</span></span>|<span data-ttu-id="76db4-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="76db4-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="76db4-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="76db4-137">description</span><span class="sxs-lookup"><span data-stu-id="76db4-137">description</span></span>|<span data-ttu-id="76db4-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-138">String</span></span>|<span data-ttu-id="76db4-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="76db4-139">The description of the app.</span></span> <span data-ttu-id="76db4-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="76db4-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="76db4-141">publisher</span></span>|<span data-ttu-id="76db4-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-142">String</span></span>|<span data-ttu-id="76db4-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="76db4-143">The publisher of the app.</span></span> <span data-ttu-id="76db4-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="76db4-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="76db4-145">largeIcon</span></span>|[<span data-ttu-id="76db4-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="76db4-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="76db4-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="76db4-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="76db4-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="76db4-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76db4-149">createdDateTime</span></span>|<span data-ttu-id="76db4-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76db4-150">DateTimeOffset</span></span>|<span data-ttu-id="76db4-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="76db4-151">The date and time the app was created.</span></span> <span data-ttu-id="76db4-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="76db4-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76db4-153">lastModifiedDateTime</span></span>|<span data-ttu-id="76db4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76db4-154">DateTimeOffset</span></span>|<span data-ttu-id="76db4-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="76db4-155">The date and time the app was last modified.</span></span> <span data-ttu-id="76db4-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="76db4-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="76db4-157">isFeatured</span></span>|<span data-ttu-id="76db4-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="76db4-158">Boolean</span></span>|<span data-ttu-id="76db4-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="76db4-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="76db4-160">privacyInformationUrl</span></span>|<span data-ttu-id="76db4-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-161">String</span></span>|<span data-ttu-id="76db4-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="76db4-162">The privacy statement Url.</span></span> <span data-ttu-id="76db4-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="76db4-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="76db4-164">informationUrl</span></span>|<span data-ttu-id="76db4-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-165">String</span></span>|<span data-ttu-id="76db4-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="76db4-166">The more information Url.</span></span> <span data-ttu-id="76db4-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="76db4-168">owner</span><span class="sxs-lookup"><span data-stu-id="76db4-168">owner</span></span>|<span data-ttu-id="76db4-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-169">String</span></span>|<span data-ttu-id="76db4-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="76db4-170">The owner of the app.</span></span> <span data-ttu-id="76db4-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="76db4-172">developer</span><span class="sxs-lookup"><span data-stu-id="76db4-172">developer</span></span>|<span data-ttu-id="76db4-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-173">String</span></span>|<span data-ttu-id="76db4-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="76db4-174">The developer of the app.</span></span> <span data-ttu-id="76db4-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="76db4-176">notes</span><span class="sxs-lookup"><span data-stu-id="76db4-176">notes</span></span>|<span data-ttu-id="76db4-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-177">String</span></span>|<span data-ttu-id="76db4-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="76db4-178">Notes for the app.</span></span> <span data-ttu-id="76db4-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="76db4-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="76db4-180">publishingState</span></span>|[<span data-ttu-id="76db4-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="76db4-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="76db4-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="76db4-182">The publishing state for the app.</span></span> <span data-ttu-id="76db4-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="76db4-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="76db4-184">Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="76db4-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="76db4-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="76db4-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="76db4-186">committedContentVersion</span></span>|<span data-ttu-id="76db4-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-187">String</span></span>|<span data-ttu-id="76db4-188">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="76db4-188">The internal committed content version.</span></span> <span data-ttu-id="76db4-189">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="76db4-190">fileName</span><span class="sxs-lookup"><span data-stu-id="76db4-190">fileName</span></span>|<span data-ttu-id="76db4-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-191">String</span></span>|<span data-ttu-id="76db4-192">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="76db4-192">The name of the main Lob application file.</span></span> <span data-ttu-id="76db4-193">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="76db4-194">size</span><span class="sxs-lookup"><span data-stu-id="76db4-194">size</span></span>|<span data-ttu-id="76db4-195">Int64</span><span class="sxs-lookup"><span data-stu-id="76db4-195">Int64</span></span>|<span data-ttu-id="76db4-196">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="76db4-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="76db4-197">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db4-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="76db4-198">packageId</span><span class="sxs-lookup"><span data-stu-id="76db4-198">packageId</span></span>|<span data-ttu-id="76db4-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-199">String</span></span>|<span data-ttu-id="76db4-200">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="76db4-200">The package identifier.</span></span>|
|<span data-ttu-id="76db4-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="76db4-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="76db4-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="76db4-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="76db4-203">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="76db4-203">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="76db4-204">versionName</span><span class="sxs-lookup"><span data-stu-id="76db4-204">versionName</span></span>|<span data-ttu-id="76db4-205">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-205">String</span></span>|<span data-ttu-id="76db4-206">Der Versionsname der branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="76db4-206">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="76db4-207">versionCode</span><span class="sxs-lookup"><span data-stu-id="76db4-207">versionCode</span></span>|<span data-ttu-id="76db4-208">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db4-208">String</span></span>|<span data-ttu-id="76db4-209">Der Versionscode der branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="76db4-209">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="76db4-210">Antwort</span><span class="sxs-lookup"><span data-stu-id="76db4-210">Response</span></span>
<span data-ttu-id="76db4-211">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [androidLobApp](../resources/intune_apps_androidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76db4-211">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune_apps_androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76db4-212">Beispiel</span><span class="sxs-lookup"><span data-stu-id="76db4-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="76db4-213">Anforderung</span><span class="sxs-lookup"><span data-stu-id="76db4-213">Request</span></span>
<span data-ttu-id="76db4-214">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="76db4-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1075

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="76db4-215">Antwort</span><span class="sxs-lookup"><span data-stu-id="76db4-215">Response</span></span>
<span data-ttu-id="76db4-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76db4-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



