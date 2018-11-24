# <a name="create-ioslobapp"></a><span data-ttu-id="154d3-101">iosLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="154d3-101">Create iosLobApp</span></span>

> <span data-ttu-id="154d3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="154d3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="154d3-103">Erstellt ein neues [iosLobApp](../resources/intune_apps_ioslobapp.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="154d3-103">Create a new [iosLobApp](../resources/intune_apps_ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="154d3-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="154d3-104">Prerequisites</span></span>
<span data-ttu-id="154d3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="154d3-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="154d3-107">Permission type</span></span>|<span data-ttu-id="154d3-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="154d3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="154d3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="154d3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="154d3-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="154d3-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="154d3-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="154d3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="154d3-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="154d3-112">Not supported.</span></span>|
|<span data-ttu-id="154d3-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="154d3-113">Application</span></span>|<span data-ttu-id="154d3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="154d3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="154d3-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="154d3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="154d3-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="154d3-116">Request headers</span></span>
|<span data-ttu-id="154d3-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="154d3-117">Header</span></span>|<span data-ttu-id="154d3-118">Wert</span><span class="sxs-lookup"><span data-stu-id="154d3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="154d3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="154d3-119">Authorization</span></span>|<span data-ttu-id="154d3-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="154d3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="154d3-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="154d3-121">Accept</span></span>|<span data-ttu-id="154d3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="154d3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="154d3-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="154d3-123">Request body</span></span>
<span data-ttu-id="154d3-124">Geben Sie im Anforderungstext eine JSON-Darstellung des iosLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="154d3-124">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="154d3-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="154d3-125">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="154d3-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="154d3-126">Property</span></span>|<span data-ttu-id="154d3-127">Typ</span><span class="sxs-lookup"><span data-stu-id="154d3-127">Type</span></span>|<span data-ttu-id="154d3-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="154d3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="154d3-129">id</span><span class="sxs-lookup"><span data-stu-id="154d3-129">id</span></span>|<span data-ttu-id="154d3-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-130">String</span></span>|<span data-ttu-id="154d3-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="154d3-131">Key of the entity.</span></span> <span data-ttu-id="154d3-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="154d3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="154d3-133">displayName</span></span>|<span data-ttu-id="154d3-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-134">String</span></span>|<span data-ttu-id="154d3-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="154d3-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="154d3-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="154d3-137">description</span><span class="sxs-lookup"><span data-stu-id="154d3-137">description</span></span>|<span data-ttu-id="154d3-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-138">String</span></span>|<span data-ttu-id="154d3-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="154d3-139">The description of the app.</span></span> <span data-ttu-id="154d3-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="154d3-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="154d3-141">publisher</span></span>|<span data-ttu-id="154d3-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-142">String</span></span>|<span data-ttu-id="154d3-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="154d3-143">The publisher of the app.</span></span> <span data-ttu-id="154d3-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="154d3-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="154d3-145">largeIcon</span></span>|[<span data-ttu-id="154d3-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="154d3-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="154d3-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="154d3-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="154d3-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="154d3-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="154d3-149">createdDateTime</span></span>|<span data-ttu-id="154d3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="154d3-150">DateTimeOffset</span></span>|<span data-ttu-id="154d3-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="154d3-151">The date and time the app was created.</span></span> <span data-ttu-id="154d3-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="154d3-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="154d3-153">lastModifiedDateTime</span></span>|<span data-ttu-id="154d3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="154d3-154">DateTimeOffset</span></span>|<span data-ttu-id="154d3-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="154d3-155">The date and time the app was last modified.</span></span> <span data-ttu-id="154d3-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="154d3-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="154d3-157">isFeatured</span></span>|<span data-ttu-id="154d3-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="154d3-158">Boolean</span></span>|<span data-ttu-id="154d3-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="154d3-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="154d3-160">privacyInformationUrl</span></span>|<span data-ttu-id="154d3-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-161">String</span></span>|<span data-ttu-id="154d3-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="154d3-162">The privacy statement Url.</span></span> <span data-ttu-id="154d3-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="154d3-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="154d3-164">informationUrl</span></span>|<span data-ttu-id="154d3-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-165">String</span></span>|<span data-ttu-id="154d3-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="154d3-166">The more information Url.</span></span> <span data-ttu-id="154d3-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="154d3-168">owner</span><span class="sxs-lookup"><span data-stu-id="154d3-168">owner</span></span>|<span data-ttu-id="154d3-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-169">String</span></span>|<span data-ttu-id="154d3-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="154d3-170">The owner of the app.</span></span> <span data-ttu-id="154d3-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="154d3-172">developer</span><span class="sxs-lookup"><span data-stu-id="154d3-172">developer</span></span>|<span data-ttu-id="154d3-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-173">String</span></span>|<span data-ttu-id="154d3-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="154d3-174">The developer of the app.</span></span> <span data-ttu-id="154d3-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="154d3-176">notes</span><span class="sxs-lookup"><span data-stu-id="154d3-176">notes</span></span>|<span data-ttu-id="154d3-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-177">String</span></span>|<span data-ttu-id="154d3-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="154d3-178">Notes for the app.</span></span> <span data-ttu-id="154d3-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="154d3-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="154d3-180">publishingState</span></span>|[<span data-ttu-id="154d3-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="154d3-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="154d3-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="154d3-182">The publishing state for the app.</span></span> <span data-ttu-id="154d3-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="154d3-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="154d3-184">Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="154d3-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="154d3-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="154d3-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="154d3-186">committedContentVersion</span></span>|<span data-ttu-id="154d3-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-187">String</span></span>|<span data-ttu-id="154d3-188">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="154d3-188">The internal committed content version.</span></span> <span data-ttu-id="154d3-189">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="154d3-190">fileName</span><span class="sxs-lookup"><span data-stu-id="154d3-190">fileName</span></span>|<span data-ttu-id="154d3-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-191">String</span></span>|<span data-ttu-id="154d3-192">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="154d3-192">The name of the main Lob application file.</span></span> <span data-ttu-id="154d3-193">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="154d3-194">size</span><span class="sxs-lookup"><span data-stu-id="154d3-194">size</span></span>|<span data-ttu-id="154d3-195">Int64</span><span class="sxs-lookup"><span data-stu-id="154d3-195">Int64</span></span>|<span data-ttu-id="154d3-196">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="154d3-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="154d3-197">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="154d3-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="154d3-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="154d3-198">bundleId</span></span>|<span data-ttu-id="154d3-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-199">String</span></span>|<span data-ttu-id="154d3-200">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="154d3-200">The Identity Name.</span></span>|
|<span data-ttu-id="154d3-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="154d3-201">applicableDeviceType</span></span>|[<span data-ttu-id="154d3-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="154d3-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="154d3-203">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="154d3-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="154d3-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="154d3-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="154d3-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="154d3-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="154d3-206">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="154d3-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="154d3-207">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="154d3-207">expirationDateTime</span></span>|<span data-ttu-id="154d3-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="154d3-208">DateTimeOffset</span></span>|<span data-ttu-id="154d3-209">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="154d3-209">The expiration time.</span></span>|
|<span data-ttu-id="154d3-210">versionNumber</span><span class="sxs-lookup"><span data-stu-id="154d3-210">versionNumber</span></span>|<span data-ttu-id="154d3-211">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-211">String</span></span>|<span data-ttu-id="154d3-212">Die Versionsnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="154d3-212">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="154d3-213">buildNumber</span><span class="sxs-lookup"><span data-stu-id="154d3-213">buildNumber</span></span>|<span data-ttu-id="154d3-214">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="154d3-214">String</span></span>|<span data-ttu-id="154d3-215">Die Buildnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="154d3-215">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="154d3-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="154d3-216">Response</span></span>
<span data-ttu-id="154d3-217">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosLobApp](../resources/intune_apps_ioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="154d3-217">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune_apps_ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="154d3-218">Beispiel</span><span class="sxs-lookup"><span data-stu-id="154d3-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="154d3-219">Anforderung</span><span class="sxs-lookup"><span data-stu-id="154d3-219">Request</span></span>
<span data-ttu-id="154d3-220">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="154d3-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1209

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="154d3-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="154d3-221">Response</span></span>
<span data-ttu-id="154d3-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="154d3-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1381

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



