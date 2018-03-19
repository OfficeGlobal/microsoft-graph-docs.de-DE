# <a name="create-windowsmobilemsi"></a><span data-ttu-id="304ca-101">Erstellen von „windowsMobileMSI“</span><span class="sxs-lookup"><span data-stu-id="304ca-101">Create windowsMobileMSI</span></span>

> <span data-ttu-id="304ca-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="304ca-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="304ca-103">Erstellen eines neuen [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="304ca-103">Create a new [plannerBucket](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="304ca-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="304ca-104">Prerequisites</span></span>
<span data-ttu-id="304ca-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="304ca-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="304ca-107">Permission type</span></span>|<span data-ttu-id="304ca-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="304ca-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="304ca-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="304ca-109">Delegated (work or school account)</span></span>|<span data-ttu-id="304ca-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304ca-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="304ca-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="304ca-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="304ca-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="304ca-112">Not supported.</span></span>|
|<span data-ttu-id="304ca-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="304ca-113">Application</span></span>|<span data-ttu-id="304ca-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="304ca-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="304ca-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="304ca-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="304ca-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="304ca-116">Request headers</span></span>
|<span data-ttu-id="304ca-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="304ca-117">Header</span></span>|<span data-ttu-id="304ca-118">Wert</span><span class="sxs-lookup"><span data-stu-id="304ca-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="304ca-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="304ca-119">Authorization</span></span>|<span data-ttu-id="304ca-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="304ca-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="304ca-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="304ca-121">Accept</span></span>|<span data-ttu-id="304ca-122">application/json</span><span class="sxs-lookup"><span data-stu-id="304ca-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="304ca-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="304ca-123">Request body</span></span>
<span data-ttu-id="304ca-124">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsMobileMSI-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="304ca-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="304ca-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsMobileMSI erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="304ca-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="304ca-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="304ca-126">Property</span></span>|<span data-ttu-id="304ca-127">Typ</span><span class="sxs-lookup"><span data-stu-id="304ca-127">Type</span></span>|<span data-ttu-id="304ca-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="304ca-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="304ca-129">id</span><span class="sxs-lookup"><span data-stu-id="304ca-129">id</span></span>|<span data-ttu-id="304ca-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-130">String</span></span>|<span data-ttu-id="304ca-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="304ca-131">Key of the setting.</span></span> <span data-ttu-id="304ca-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="304ca-133">displayName</span><span class="sxs-lookup"><span data-stu-id="304ca-133">displayName</span></span>|<span data-ttu-id="304ca-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-134">String</span></span>|<span data-ttu-id="304ca-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="304ca-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="304ca-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="304ca-137">description</span><span class="sxs-lookup"><span data-stu-id="304ca-137">description</span></span>|<span data-ttu-id="304ca-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-138">String</span></span>|<span data-ttu-id="304ca-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="304ca-139">The description of the app.</span></span> <span data-ttu-id="304ca-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="304ca-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="304ca-141">Publisher</span></span>|<span data-ttu-id="304ca-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-142">String</span></span>|<span data-ttu-id="304ca-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="304ca-143">The name of the app.</span></span> <span data-ttu-id="304ca-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="304ca-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="304ca-145">largeIcon</span></span>|[<span data-ttu-id="304ca-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="304ca-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="304ca-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="304ca-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="304ca-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="304ca-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="304ca-149">createdDateTime</span></span>|<span data-ttu-id="304ca-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="304ca-150">DateTimeOffset</span></span>|<span data-ttu-id="304ca-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="304ca-151">The date and time the group was created.</span></span> <span data-ttu-id="304ca-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="304ca-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="304ca-153">lastModifiedDateTime</span></span>|<span data-ttu-id="304ca-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="304ca-154">DateTimeOffset</span></span>|<span data-ttu-id="304ca-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="304ca-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="304ca-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="304ca-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="304ca-157">isFeatured</span></span>|<span data-ttu-id="304ca-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="304ca-158">Boolean</span></span>|<span data-ttu-id="304ca-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="304ca-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="304ca-160">privacyInformationUrl</span></span>|<span data-ttu-id="304ca-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-161">String</span></span>|<span data-ttu-id="304ca-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="304ca-162">The privacy statement Url.</span></span> <span data-ttu-id="304ca-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="304ca-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="304ca-164">informationUrl</span></span>|<span data-ttu-id="304ca-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-165">String</span></span>|<span data-ttu-id="304ca-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="304ca-166">The more information Url.</span></span> <span data-ttu-id="304ca-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="304ca-168">owner</span><span class="sxs-lookup"><span data-stu-id="304ca-168">owner</span></span>|<span data-ttu-id="304ca-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-169">String</span></span>|<span data-ttu-id="304ca-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="304ca-170">The owner of the app.</span></span> <span data-ttu-id="304ca-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="304ca-172">developer</span><span class="sxs-lookup"><span data-stu-id="304ca-172">developer</span></span>|<span data-ttu-id="304ca-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-173">String</span></span>|<span data-ttu-id="304ca-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="304ca-174">The name of the app.</span></span> <span data-ttu-id="304ca-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="304ca-176">notes</span><span class="sxs-lookup"><span data-stu-id="304ca-176">notes</span></span>|<span data-ttu-id="304ca-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-177">String</span></span>|<span data-ttu-id="304ca-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="304ca-178">Notes for the app.</span></span> <span data-ttu-id="304ca-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="304ca-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="304ca-180">publishingState</span></span>|<span data-ttu-id="304ca-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-181">String</span></span>|<span data-ttu-id="304ca-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="304ca-182">The publishing state for the app.</span></span> <span data-ttu-id="304ca-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="304ca-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="304ca-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="304ca-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="304ca-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="304ca-185">committedContentVersion</span></span>|<span data-ttu-id="304ca-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-186">String</span></span>|<span data-ttu-id="304ca-187">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="304ca-187">The internal committed content version.</span></span> <span data-ttu-id="304ca-188">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="304ca-189">fileName</span><span class="sxs-lookup"><span data-stu-id="304ca-189">fileName</span></span>|<span data-ttu-id="304ca-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-190">String</span></span>|<span data-ttu-id="304ca-191">Der Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="304ca-191">The name of the main Lob application file.</span></span> <span data-ttu-id="304ca-192">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="304ca-193">size</span><span class="sxs-lookup"><span data-stu-id="304ca-193">size</span></span>|<span data-ttu-id="304ca-194">Int64</span><span class="sxs-lookup"><span data-stu-id="304ca-194">Int64</span></span>|<span data-ttu-id="304ca-195">Die Gesamtgröße, einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="304ca-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="304ca-196">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="304ca-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="304ca-197">commandLine</span><span class="sxs-lookup"><span data-stu-id="304ca-197">Command-line:</span></span>|<span data-ttu-id="304ca-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-198">String</span></span>|<span data-ttu-id="304ca-199">Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="304ca-199">The command line.</span></span>|
|<span data-ttu-id="304ca-200">productCode</span><span class="sxs-lookup"><span data-stu-id="304ca-200">ProductCode</span></span>|<span data-ttu-id="304ca-201">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-201">String</span></span>|<span data-ttu-id="304ca-202">Produktcode</span><span class="sxs-lookup"><span data-stu-id="304ca-202">The product code.</span></span>|
|<span data-ttu-id="304ca-203">productVersion</span><span class="sxs-lookup"><span data-stu-id="304ca-203">productVersion</span></span>|<span data-ttu-id="304ca-204">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="304ca-204">String</span></span>|<span data-ttu-id="304ca-205">Produktversion der branchenspezifischen Windows Mobile-MSI-App.</span><span class="sxs-lookup"><span data-stu-id="304ca-205">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="304ca-206">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="304ca-206">ignoreVersionDetection</span></span>|<span data-ttu-id="304ca-207">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="304ca-207">Boolean</span></span>|<span data-ttu-id="304ca-208">Boolescher Wert, der steuert, ob nach der Installation der App auf einem Gerät die App-Version zur Erkennung der App verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="304ca-208">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="304ca-209">Setzen Sie diese Eigenschaft auf „true“ bei branchenspezifischen Windows Mobile-MSI-Apps, die sich selbstständig aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="304ca-209">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="304ca-210">Antwort</span><span class="sxs-lookup"><span data-stu-id="304ca-210">Response</span></span>
<span data-ttu-id="304ca-211">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="304ca-211">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_apps_windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="304ca-212">Beispiel</span><span class="sxs-lookup"><span data-stu-id="304ca-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="304ca-213">Anforderung</span><span class="sxs-lookup"><span data-stu-id="304ca-213">Request</span></span>
<span data-ttu-id="304ca-214">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="304ca-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 919

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="304ca-215">Antwort</span><span class="sxs-lookup"><span data-stu-id="304ca-215">Response</span></span>
<span data-ttu-id="304ca-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="304ca-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1027

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```



