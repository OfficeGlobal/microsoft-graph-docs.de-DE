# <a name="create-ioslobapp"></a><span data-ttu-id="d17bc-101">iosLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="d17bc-101">Create iosLobApp</span></span>

> <span data-ttu-id="d17bc-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d17bc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d17bc-103">Erstellt ein neues [iosLobApp](../resources/intune_apps_ioslobapp.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d17bc-103">Create a new [plannerBucket](../resources/intune_apps_ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d17bc-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d17bc-104">Prerequisites</span></span>
<span data-ttu-id="d17bc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d17bc-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d17bc-107">Permission type</span></span>|<span data-ttu-id="d17bc-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d17bc-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d17bc-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d17bc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d17bc-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d17bc-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d17bc-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d17bc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d17bc-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d17bc-112">Not supported.</span></span>|
|<span data-ttu-id="d17bc-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d17bc-113">Application</span></span>|<span data-ttu-id="d17bc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d17bc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d17bc-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d17bc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d17bc-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d17bc-116">Request headers</span></span>
|<span data-ttu-id="d17bc-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d17bc-117">Header</span></span>|<span data-ttu-id="d17bc-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d17bc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d17bc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d17bc-119">Authorization</span></span>|<span data-ttu-id="d17bc-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d17bc-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d17bc-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d17bc-121">Accept</span></span>|<span data-ttu-id="d17bc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d17bc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d17bc-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d17bc-123">Request body</span></span>
<span data-ttu-id="d17bc-124">Geben Sie im Anforderungstext eine JSON-Darstellung des iosLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d17bc-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="d17bc-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d17bc-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="d17bc-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d17bc-126">Property</span></span>|<span data-ttu-id="d17bc-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d17bc-127">Type</span></span>|<span data-ttu-id="d17bc-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d17bc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d17bc-129">id</span><span class="sxs-lookup"><span data-stu-id="d17bc-129">id</span></span>|<span data-ttu-id="d17bc-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-130">String</span></span>|<span data-ttu-id="d17bc-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="d17bc-131">Key of the setting.</span></span> <span data-ttu-id="d17bc-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d17bc-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d17bc-133">displayName</span></span>|<span data-ttu-id="d17bc-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-134">String</span></span>|<span data-ttu-id="d17bc-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="d17bc-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d17bc-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d17bc-137">description</span><span class="sxs-lookup"><span data-stu-id="d17bc-137">description</span></span>|<span data-ttu-id="d17bc-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-138">String</span></span>|<span data-ttu-id="d17bc-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="d17bc-139">The description of the app.</span></span> <span data-ttu-id="d17bc-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d17bc-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="d17bc-141">Publisher</span></span>|<span data-ttu-id="d17bc-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-142">String</span></span>|<span data-ttu-id="d17bc-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="d17bc-143">The name of the app.</span></span> <span data-ttu-id="d17bc-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d17bc-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d17bc-145">largeIcon</span></span>|[<span data-ttu-id="d17bc-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d17bc-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="d17bc-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="d17bc-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d17bc-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d17bc-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d17bc-149">createdDateTime</span></span>|<span data-ttu-id="d17bc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d17bc-150">DateTimeOffset</span></span>|<span data-ttu-id="d17bc-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="d17bc-151">The date and time the group was created.</span></span> <span data-ttu-id="d17bc-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d17bc-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d17bc-153">lastModifiedDateTime</span></span>|<span data-ttu-id="d17bc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d17bc-154">DateTimeOffset</span></span>|<span data-ttu-id="d17bc-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="d17bc-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="d17bc-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d17bc-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d17bc-157">isFeatured</span></span>|<span data-ttu-id="d17bc-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d17bc-158">Boolean</span></span>|<span data-ttu-id="d17bc-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d17bc-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d17bc-160">privacyInformationUrl</span></span>|<span data-ttu-id="d17bc-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-161">String</span></span>|<span data-ttu-id="d17bc-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="d17bc-162">The privacy statement Url.</span></span> <span data-ttu-id="d17bc-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d17bc-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d17bc-164">informationUrl</span></span>|<span data-ttu-id="d17bc-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-165">String</span></span>|<span data-ttu-id="d17bc-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="d17bc-166">The more information Url.</span></span> <span data-ttu-id="d17bc-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d17bc-168">owner</span><span class="sxs-lookup"><span data-stu-id="d17bc-168">owner</span></span>|<span data-ttu-id="d17bc-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-169">String</span></span>|<span data-ttu-id="d17bc-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="d17bc-170">The owner of the app.</span></span> <span data-ttu-id="d17bc-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d17bc-172">developer</span><span class="sxs-lookup"><span data-stu-id="d17bc-172">developer</span></span>|<span data-ttu-id="d17bc-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-173">String</span></span>|<span data-ttu-id="d17bc-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="d17bc-174">The name of the app.</span></span> <span data-ttu-id="d17bc-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d17bc-176">notes</span><span class="sxs-lookup"><span data-stu-id="d17bc-176">notes</span></span>|<span data-ttu-id="d17bc-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-177">String</span></span>|<span data-ttu-id="d17bc-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="d17bc-178">Notes for the app.</span></span> <span data-ttu-id="d17bc-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d17bc-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="d17bc-180">publishingState</span></span>|<span data-ttu-id="d17bc-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-181">String</span></span>|<span data-ttu-id="d17bc-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="d17bc-182">The publishing state for the app.</span></span> <span data-ttu-id="d17bc-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="d17bc-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d17bc-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="d17bc-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d17bc-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d17bc-185">committedContentVersion</span></span>|<span data-ttu-id="d17bc-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-186">String</span></span>|<span data-ttu-id="d17bc-187">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="d17bc-187">The internal committed content version.</span></span> <span data-ttu-id="d17bc-188">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="d17bc-189">fileName</span><span class="sxs-lookup"><span data-stu-id="d17bc-189">fileName</span></span>|<span data-ttu-id="d17bc-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-190">String</span></span>|<span data-ttu-id="d17bc-191">Der Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="d17bc-191">The name of the main Lob application file.</span></span> <span data-ttu-id="d17bc-192">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="d17bc-193">size</span><span class="sxs-lookup"><span data-stu-id="d17bc-193">size</span></span>|<span data-ttu-id="d17bc-194">Int64</span><span class="sxs-lookup"><span data-stu-id="d17bc-194">Int64</span></span>|<span data-ttu-id="d17bc-195">Die Gesamtgröße, einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="d17bc-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="d17bc-196">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d17bc-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="d17bc-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="d17bc-197">bundleId</span></span>|<span data-ttu-id="d17bc-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-198">String</span></span>|<span data-ttu-id="d17bc-199">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="d17bc-199">The Identity Name.</span></span>|
|<span data-ttu-id="d17bc-200">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="d17bc-200">applicableDeviceType</span></span>|[<span data-ttu-id="d17bc-201">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="d17bc-201">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="d17bc-202">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="d17bc-202">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="d17bc-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d17bc-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d17bc-204">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d17bc-204">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="d17bc-205">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="d17bc-205">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d17bc-206">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d17bc-206">expirationDateTime</span></span>|<span data-ttu-id="d17bc-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d17bc-207">DateTimeOffset</span></span>|<span data-ttu-id="d17bc-208">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="d17bc-208">: The expiration time for the subscription.</span></span>|
|<span data-ttu-id="d17bc-209">versionNumber</span><span class="sxs-lookup"><span data-stu-id="d17bc-209">versionNumber</span></span>|<span data-ttu-id="d17bc-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-210">String</span></span>|<span data-ttu-id="d17bc-211">Die Versionsnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="d17bc-211">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d17bc-212">buildNumber</span><span class="sxs-lookup"><span data-stu-id="d17bc-212">buildNumber</span></span>|<span data-ttu-id="d17bc-213">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d17bc-213">String</span></span>|<span data-ttu-id="d17bc-214">Die Buildnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="d17bc-214">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="d17bc-215">Antwort</span><span class="sxs-lookup"><span data-stu-id="d17bc-215">Response</span></span>
<span data-ttu-id="d17bc-216">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosLobApp](../resources/intune_apps_ioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d17bc-216">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_apps_ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d17bc-217">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d17bc-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="d17bc-218">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d17bc-218">Request</span></span>
<span data-ttu-id="d17bc-219">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d17bc-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1253

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
    "v11_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="d17bc-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="d17bc-220">Response</span></span>
<span data-ttu-id="d17bc-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d17bc-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1361

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
    "v11_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



