# <a name="update-androidlobapp"></a><span data-ttu-id="73604-101">AndroidLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="73604-101">Update androidLobApp</span></span>

> <span data-ttu-id="73604-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="73604-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73604-103">Aktualisieren der Eigenschaften eines [androidLobApp](../resources/intune_apps_androidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="73604-103">Update the properties of a [calendar](../resources/intune_apps_androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73604-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="73604-104">Prerequisites</span></span>
<span data-ttu-id="73604-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="73604-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="73604-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73604-107">Permission type</span></span>|<span data-ttu-id="73604-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73604-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73604-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73604-109">Delegated (work or school account)</span></span>|<span data-ttu-id="73604-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73604-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73604-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73604-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73604-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73604-112">Not supported.</span></span>|
|<span data-ttu-id="73604-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73604-113">Application</span></span>|<span data-ttu-id="73604-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73604-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73604-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73604-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="73604-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73604-116">Request headers</span></span>
|<span data-ttu-id="73604-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="73604-117">Header</span></span>|<span data-ttu-id="73604-118">Wert</span><span class="sxs-lookup"><span data-stu-id="73604-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73604-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="73604-119">Authorization</span></span>|<span data-ttu-id="73604-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="73604-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="73604-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="73604-121">Accept</span></span>|<span data-ttu-id="73604-122">application/json</span><span class="sxs-lookup"><span data-stu-id="73604-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73604-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73604-123">Request body</span></span>
<span data-ttu-id="73604-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidLobApp](../resources/intune_apps_androidlobapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="73604-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_androidlobapp.md) object.</span></span>

<span data-ttu-id="73604-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidLobApp](../resources/intune_apps_androidlobapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="73604-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="73604-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73604-126">Property</span></span>|<span data-ttu-id="73604-127">Typ</span><span class="sxs-lookup"><span data-stu-id="73604-127">Type</span></span>|<span data-ttu-id="73604-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73604-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73604-129">id</span><span class="sxs-lookup"><span data-stu-id="73604-129">id</span></span>|<span data-ttu-id="73604-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-130">String</span></span>|<span data-ttu-id="73604-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="73604-131">Key of the setting.</span></span> <span data-ttu-id="73604-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73604-133">displayName</span><span class="sxs-lookup"><span data-stu-id="73604-133">displayName</span></span>|<span data-ttu-id="73604-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-134">String</span></span>|<span data-ttu-id="73604-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="73604-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="73604-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73604-137">description</span><span class="sxs-lookup"><span data-stu-id="73604-137">description</span></span>|<span data-ttu-id="73604-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-138">String</span></span>|<span data-ttu-id="73604-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="73604-139">The description of the app.</span></span> <span data-ttu-id="73604-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73604-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="73604-141">Publisher</span></span>|<span data-ttu-id="73604-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-142">String</span></span>|<span data-ttu-id="73604-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="73604-143">The name of the app.</span></span> <span data-ttu-id="73604-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73604-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="73604-145">largeIcon</span></span>|[<span data-ttu-id="73604-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="73604-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="73604-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="73604-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="73604-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73604-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73604-149">createdDateTime</span></span>|<span data-ttu-id="73604-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73604-150">DateTimeOffset</span></span>|<span data-ttu-id="73604-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="73604-151">The date and time the group was created.</span></span> <span data-ttu-id="73604-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73604-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73604-153">lastModifiedDateTime</span></span>|<span data-ttu-id="73604-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73604-154">DateTimeOffset</span></span>|<span data-ttu-id="73604-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="73604-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="73604-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73604-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="73604-157">isFeatured</span></span>|<span data-ttu-id="73604-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="73604-158">Boolean</span></span>|<span data-ttu-id="73604-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73604-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="73604-160">privacyInformationUrl</span></span>|<span data-ttu-id="73604-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-161">String</span></span>|<span data-ttu-id="73604-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="73604-162">The privacy statement Url.</span></span> <span data-ttu-id="73604-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73604-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="73604-164">informationUrl</span></span>|<span data-ttu-id="73604-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-165">String</span></span>|<span data-ttu-id="73604-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="73604-166">The more information Url.</span></span> <span data-ttu-id="73604-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73604-168">owner</span><span class="sxs-lookup"><span data-stu-id="73604-168">owner</span></span>|<span data-ttu-id="73604-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-169">String</span></span>|<span data-ttu-id="73604-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="73604-170">The owner of the app.</span></span> <span data-ttu-id="73604-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73604-172">developer</span><span class="sxs-lookup"><span data-stu-id="73604-172">developer</span></span>|<span data-ttu-id="73604-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-173">String</span></span>|<span data-ttu-id="73604-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="73604-174">The name of the app.</span></span> <span data-ttu-id="73604-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73604-176">notes</span><span class="sxs-lookup"><span data-stu-id="73604-176">notes</span></span>|<span data-ttu-id="73604-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-177">String</span></span>|<span data-ttu-id="73604-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="73604-178">Notes for the app.</span></span> <span data-ttu-id="73604-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73604-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="73604-180">publishingState</span></span>|<span data-ttu-id="73604-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-181">String</span></span>|<span data-ttu-id="73604-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="73604-182">The publishing state for the app.</span></span> <span data-ttu-id="73604-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="73604-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="73604-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="73604-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="73604-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="73604-185">committedContentVersion</span></span>|<span data-ttu-id="73604-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-186">String</span></span>|<span data-ttu-id="73604-187">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="73604-187">The internal committed content version.</span></span> <span data-ttu-id="73604-188">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="73604-189">fileName</span><span class="sxs-lookup"><span data-stu-id="73604-189">fileName</span></span>|<span data-ttu-id="73604-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-190">String</span></span>|<span data-ttu-id="73604-191">Der Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="73604-191">The name of the main Lob application file.</span></span> <span data-ttu-id="73604-192">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="73604-193">size</span><span class="sxs-lookup"><span data-stu-id="73604-193">size</span></span>|<span data-ttu-id="73604-194">Int64</span><span class="sxs-lookup"><span data-stu-id="73604-194">Int64</span></span>|<span data-ttu-id="73604-195">Die Gesamtgröße, einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="73604-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="73604-196">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="73604-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="73604-197">packageId</span><span class="sxs-lookup"><span data-stu-id="73604-197">packageId</span></span>|<span data-ttu-id="73604-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-198">String</span></span>|<span data-ttu-id="73604-199">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="73604-199">The package identifier.</span></span>|
|<span data-ttu-id="73604-200">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="73604-200">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="73604-201">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="73604-201">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="73604-202">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="73604-202">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="73604-203">versionName</span><span class="sxs-lookup"><span data-stu-id="73604-203">versionName</span></span>|<span data-ttu-id="73604-204">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-204">String</span></span>|<span data-ttu-id="73604-205">Der Versionsname der branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="73604-205">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="73604-206">versionCode</span><span class="sxs-lookup"><span data-stu-id="73604-206">versionCode</span></span>|<span data-ttu-id="73604-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73604-207">String</span></span>|<span data-ttu-id="73604-208">Der Versionscode der branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="73604-208">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="73604-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="73604-209">Response</span></span>
<span data-ttu-id="73604-210">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [androidLobApp](../resources/intune_apps_androidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73604-210">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73604-211">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73604-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="73604-212">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73604-212">Request</span></span>
<span data-ttu-id="73604-213">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73604-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1087

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

### <a name="response"></a><span data-ttu-id="73604-214">Antwort</span><span class="sxs-lookup"><span data-stu-id="73604-214">Response</span></span>
<span data-ttu-id="73604-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73604-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



