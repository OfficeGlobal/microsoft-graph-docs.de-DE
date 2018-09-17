# <a name="update-windowsmobilemsi"></a><span data-ttu-id="099a7-101">windowsMobileMSI aktualisieren</span><span class="sxs-lookup"><span data-stu-id="099a7-101">Update windowsMobileMSI</span></span>

> <span data-ttu-id="099a7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="099a7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="099a7-103">Aktualisiert die Eigenschaften von Objekten des Typs [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-103">Update the properties of a [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="099a7-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="099a7-104">Prerequisites</span></span>
<span data-ttu-id="099a7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="099a7-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="099a7-107">Permission type</span></span>|<span data-ttu-id="099a7-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="099a7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="099a7-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="099a7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="099a7-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="099a7-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="099a7-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="099a7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="099a7-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="099a7-112">Not supported.</span></span>|
|<span data-ttu-id="099a7-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="099a7-113">Application</span></span>|<span data-ttu-id="099a7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="099a7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="099a7-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="099a7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="099a7-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="099a7-116">Request headers</span></span>
|<span data-ttu-id="099a7-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="099a7-117">Header</span></span>|<span data-ttu-id="099a7-118">Wert</span><span class="sxs-lookup"><span data-stu-id="099a7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="099a7-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="099a7-119">Authorization</span></span>|<span data-ttu-id="099a7-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="099a7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="099a7-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="099a7-121">Accept</span></span>|<span data-ttu-id="099a7-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="099a7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="099a7-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="099a7-123">Request body</span></span>
<span data-ttu-id="099a7-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="099a7-124">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="099a7-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="099a7-125">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span></span>

|<span data-ttu-id="099a7-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="099a7-126">Property</span></span>|<span data-ttu-id="099a7-127">Typ</span><span class="sxs-lookup"><span data-stu-id="099a7-127">Type</span></span>|<span data-ttu-id="099a7-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="099a7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="099a7-129">ID</span><span class="sxs-lookup"><span data-stu-id="099a7-129">id</span></span>|<span data-ttu-id="099a7-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-130">String</span></span>|<span data-ttu-id="099a7-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="099a7-131">Key of the entity.</span></span> <span data-ttu-id="099a7-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="099a7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="099a7-133">displayName</span></span>|<span data-ttu-id="099a7-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-134">String</span></span>|<span data-ttu-id="099a7-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="099a7-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="099a7-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="099a7-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="099a7-137">description</span></span>|<span data-ttu-id="099a7-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-138">String</span></span>|<span data-ttu-id="099a7-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="099a7-139">The description of the app.</span></span> <span data-ttu-id="099a7-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="099a7-141">Verleger</span><span class="sxs-lookup"><span data-stu-id="099a7-141">publisher</span></span>|<span data-ttu-id="099a7-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-142">String</span></span>|<span data-ttu-id="099a7-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="099a7-143">The publisher of the app.</span></span> <span data-ttu-id="099a7-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="099a7-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="099a7-145">largeIcon</span></span>|[<span data-ttu-id="099a7-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="099a7-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="099a7-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="099a7-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="099a7-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="099a7-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="099a7-149">createdDateTime</span></span>|<span data-ttu-id="099a7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="099a7-150">DateTimeOffset</span></span>|<span data-ttu-id="099a7-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="099a7-151">The date and time the app was created.</span></span> <span data-ttu-id="099a7-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="099a7-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="099a7-153">lastModifiedDateTime</span></span>|<span data-ttu-id="099a7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="099a7-154">DateTimeOffset</span></span>|<span data-ttu-id="099a7-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="099a7-155">The date and time the app was last modified.</span></span> <span data-ttu-id="099a7-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="099a7-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="099a7-157">isFeatured</span></span>|<span data-ttu-id="099a7-158">boolesch</span><span class="sxs-lookup"><span data-stu-id="099a7-158">Boolean</span></span>|<span data-ttu-id="099a7-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="099a7-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="099a7-160">privacyInformationUrl</span></span>|<span data-ttu-id="099a7-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-161">String</span></span>|<span data-ttu-id="099a7-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="099a7-162">The privacy statement Url.</span></span> <span data-ttu-id="099a7-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="099a7-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="099a7-164">informationUrl</span></span>|<span data-ttu-id="099a7-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-165">String</span></span>|<span data-ttu-id="099a7-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="099a7-166">The more information Url.</span></span> <span data-ttu-id="099a7-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="099a7-168">Besitzer</span><span class="sxs-lookup"><span data-stu-id="099a7-168">owner</span></span>|<span data-ttu-id="099a7-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-169">String</span></span>|<span data-ttu-id="099a7-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="099a7-170">The owner of the app.</span></span> <span data-ttu-id="099a7-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="099a7-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="099a7-172">developer</span></span>|<span data-ttu-id="099a7-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-173">String</span></span>|<span data-ttu-id="099a7-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="099a7-174">The developer of the app.</span></span> <span data-ttu-id="099a7-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="099a7-176">Notizen</span><span class="sxs-lookup"><span data-stu-id="099a7-176">notes</span></span>|<span data-ttu-id="099a7-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-177">String</span></span>|<span data-ttu-id="099a7-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="099a7-178">Notes for the app.</span></span> <span data-ttu-id="099a7-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="099a7-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="099a7-180">publishingState</span></span>|[<span data-ttu-id="099a7-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="099a7-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="099a7-p114">Der Veröffentlichungsstand der App. Die App kann nur dann zugewiesen werden, wenn die App veröffentlicht wird. Vererbt von [mobileApp](../resources/intune_apps_mobileapp.md). Die möglichen Werte sind: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="099a7-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="099a7-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="099a7-186">committedContentVersion</span></span>|<span data-ttu-id="099a7-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-187">String</span></span>|<span data-ttu-id="099a7-188">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="099a7-188">The internal committed content version.</span></span> <span data-ttu-id="099a7-189">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="099a7-190">fileName</span><span class="sxs-lookup"><span data-stu-id="099a7-190">fileName</span></span>|<span data-ttu-id="099a7-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-191">String</span></span>|<span data-ttu-id="099a7-192">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="099a7-192">The name of the main Lob application file.</span></span> <span data-ttu-id="099a7-193">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="099a7-194">Größe</span><span class="sxs-lookup"><span data-stu-id="099a7-194">size</span></span>|<span data-ttu-id="099a7-195">Int64</span><span class="sxs-lookup"><span data-stu-id="099a7-195">Int64</span></span>|<span data-ttu-id="099a7-196">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="099a7-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="099a7-197">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="099a7-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="099a7-198">commandLine</span><span class="sxs-lookup"><span data-stu-id="099a7-198">commandLine</span></span>|<span data-ttu-id="099a7-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-199">String</span></span>|<span data-ttu-id="099a7-200">Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="099a7-200">The command line.</span></span>|
|<span data-ttu-id="099a7-201">productCode</span><span class="sxs-lookup"><span data-stu-id="099a7-201">productCode</span></span>|<span data-ttu-id="099a7-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-202">String</span></span>|<span data-ttu-id="099a7-203">Produktcode</span><span class="sxs-lookup"><span data-stu-id="099a7-203">The product code.</span></span>|
|<span data-ttu-id="099a7-204">productVersion</span><span class="sxs-lookup"><span data-stu-id="099a7-204">productVersion</span></span>|<span data-ttu-id="099a7-205">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="099a7-205">String</span></span>|<span data-ttu-id="099a7-206">Produktversion der branchenspezifischen Windows Mobile-MSI-App.</span><span class="sxs-lookup"><span data-stu-id="099a7-206">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="099a7-207">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="099a7-207">ignoreVersionDetection</span></span>|<span data-ttu-id="099a7-208">boolesch</span><span class="sxs-lookup"><span data-stu-id="099a7-208">Boolean</span></span>|<span data-ttu-id="099a7-209">Boolescher Wert, der steuert, ob nach der Installation der App auf einem Gerät die App-Version zur Erkennung der App verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="099a7-209">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="099a7-210">Setzen Sie diese Eigenschaft auf „true“ bei branchenspezifischen Windows Mobile-MSI-Apps, die sich selbstständig aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="099a7-210">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="099a7-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="099a7-211">Response</span></span>
<span data-ttu-id="099a7-212">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="099a7-212">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="099a7-213">Beispiel</span><span class="sxs-lookup"><span data-stu-id="099a7-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="099a7-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="099a7-214">Request</span></span>
<span data-ttu-id="099a7-215">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="099a7-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 864

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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="099a7-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="099a7-216">Response</span></span>
<span data-ttu-id="099a7-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="099a7-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








