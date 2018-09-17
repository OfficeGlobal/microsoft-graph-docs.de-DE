# <a name="create-ioslobapp"></a><span data-ttu-id="04e56-101">iosLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="04e56-101">Create iosLobApp</span></span>

> <span data-ttu-id="04e56-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="04e56-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04e56-103">Erstellt ein neues [iosLobApp](../resources/intune_apps_ioslobapp.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="04e56-103">Create a new [iosLobApp](../resources/intune_apps_ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04e56-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="04e56-104">Prerequisites</span></span>
<span data-ttu-id="04e56-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04e56-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04e56-107">Permission type</span></span>|<span data-ttu-id="04e56-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04e56-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04e56-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04e56-109">Delegated (work or school account)</span></span>|<span data-ttu-id="04e56-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04e56-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04e56-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04e56-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04e56-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04e56-112">Not supported.</span></span>|
|<span data-ttu-id="04e56-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04e56-113">Application</span></span>|<span data-ttu-id="04e56-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04e56-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04e56-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04e56-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="04e56-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04e56-116">Request headers</span></span>
|<span data-ttu-id="04e56-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="04e56-117">Header</span></span>|<span data-ttu-id="04e56-118">Wert</span><span class="sxs-lookup"><span data-stu-id="04e56-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04e56-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="04e56-119">Authorization</span></span>|<span data-ttu-id="04e56-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="04e56-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04e56-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="04e56-121">Accept</span></span>|<span data-ttu-id="04e56-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="04e56-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04e56-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04e56-123">Request body</span></span>
<span data-ttu-id="04e56-124">Geben Sie im Anforderungstext eine JSON-Darstellung des iosLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="04e56-124">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="04e56-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="04e56-125">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="04e56-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="04e56-126">Property</span></span>|<span data-ttu-id="04e56-127">Typ</span><span class="sxs-lookup"><span data-stu-id="04e56-127">Type</span></span>|<span data-ttu-id="04e56-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04e56-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04e56-129">ID</span><span class="sxs-lookup"><span data-stu-id="04e56-129">id</span></span>|<span data-ttu-id="04e56-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-130">String</span></span>|<span data-ttu-id="04e56-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="04e56-131">Key of the entity.</span></span> <span data-ttu-id="04e56-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04e56-133">displayName</span><span class="sxs-lookup"><span data-stu-id="04e56-133">displayName</span></span>|<span data-ttu-id="04e56-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-134">String</span></span>|<span data-ttu-id="04e56-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="04e56-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="04e56-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04e56-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04e56-137">description</span></span>|<span data-ttu-id="04e56-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-138">String</span></span>|<span data-ttu-id="04e56-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="04e56-139">The description of the app.</span></span> <span data-ttu-id="04e56-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04e56-141">Verleger</span><span class="sxs-lookup"><span data-stu-id="04e56-141">publisher</span></span>|<span data-ttu-id="04e56-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-142">String</span></span>|<span data-ttu-id="04e56-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="04e56-143">The publisher of the app.</span></span> <span data-ttu-id="04e56-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04e56-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="04e56-145">largeIcon</span></span>|[<span data-ttu-id="04e56-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="04e56-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="04e56-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="04e56-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="04e56-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04e56-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04e56-149">createdDateTime</span></span>|<span data-ttu-id="04e56-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04e56-150">DateTimeOffset</span></span>|<span data-ttu-id="04e56-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="04e56-151">The date and time the app was created.</span></span> <span data-ttu-id="04e56-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04e56-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04e56-153">lastModifiedDateTime</span></span>|<span data-ttu-id="04e56-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04e56-154">DateTimeOffset</span></span>|<span data-ttu-id="04e56-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="04e56-155">The date and time the app was last modified.</span></span> <span data-ttu-id="04e56-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04e56-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="04e56-157">isFeatured</span></span>|<span data-ttu-id="04e56-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="04e56-158">Boolean</span></span>|<span data-ttu-id="04e56-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04e56-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="04e56-160">privacyInformationUrl</span></span>|<span data-ttu-id="04e56-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-161">String</span></span>|<span data-ttu-id="04e56-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="04e56-162">The privacy statement Url.</span></span> <span data-ttu-id="04e56-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04e56-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="04e56-164">informationUrl</span></span>|<span data-ttu-id="04e56-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-165">String</span></span>|<span data-ttu-id="04e56-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="04e56-166">The more information Url.</span></span> <span data-ttu-id="04e56-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04e56-168">Besitzer</span><span class="sxs-lookup"><span data-stu-id="04e56-168">owner</span></span>|<span data-ttu-id="04e56-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-169">String</span></span>|<span data-ttu-id="04e56-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="04e56-170">The owner of the app.</span></span> <span data-ttu-id="04e56-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04e56-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="04e56-172">developer</span></span>|<span data-ttu-id="04e56-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-173">String</span></span>|<span data-ttu-id="04e56-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="04e56-174">The developer of the app.</span></span> <span data-ttu-id="04e56-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04e56-176">Notiz</span><span class="sxs-lookup"><span data-stu-id="04e56-176">notes</span></span>|<span data-ttu-id="04e56-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-177">String</span></span>|<span data-ttu-id="04e56-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="04e56-178">Notes for the app.</span></span> <span data-ttu-id="04e56-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04e56-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="04e56-180">publishingState</span></span>|[<span data-ttu-id="04e56-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="04e56-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="04e56-p114">Der Veröffentlichungsstand der App. Die App kann nur dann zugewiesen werden, wenn die App veröffentlicht wurde. Vererbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="04e56-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="04e56-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="04e56-186">committedContentVersion</span></span>|<span data-ttu-id="04e56-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-187">String</span></span>|<span data-ttu-id="04e56-188">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="04e56-188">The internal committed content version.</span></span> <span data-ttu-id="04e56-189">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="04e56-190">fileName</span><span class="sxs-lookup"><span data-stu-id="04e56-190">fileName</span></span>|<span data-ttu-id="04e56-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-191">String</span></span>|<span data-ttu-id="04e56-192">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="04e56-192">The name of the main Lob application file.</span></span> <span data-ttu-id="04e56-193">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="04e56-194">Größe</span><span class="sxs-lookup"><span data-stu-id="04e56-194">size</span></span>|<span data-ttu-id="04e56-195">Int64</span><span class="sxs-lookup"><span data-stu-id="04e56-195">Int64</span></span>|<span data-ttu-id="04e56-196">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="04e56-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="04e56-197">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="04e56-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="04e56-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="04e56-198">bundleId</span></span>|<span data-ttu-id="04e56-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-199">String</span></span>|<span data-ttu-id="04e56-200">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="04e56-200">The Identity Name.</span></span>|
|<span data-ttu-id="04e56-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="04e56-201">applicableDeviceType</span></span>|[<span data-ttu-id="04e56-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="04e56-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="04e56-203">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="04e56-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="04e56-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="04e56-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="04e56-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="04e56-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="04e56-206">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="04e56-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="04e56-207">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="04e56-207">expirationDateTime</span></span>|<span data-ttu-id="04e56-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04e56-208">DateTimeOffset</span></span>|<span data-ttu-id="04e56-209">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="04e56-209">The expiration time.</span></span>|
|<span data-ttu-id="04e56-210">versionNumber</span><span class="sxs-lookup"><span data-stu-id="04e56-210">versionNumber</span></span>|<span data-ttu-id="04e56-211">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-211">String</span></span>|<span data-ttu-id="04e56-212">Die Versionsnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="04e56-212">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="04e56-213">buildNumber</span><span class="sxs-lookup"><span data-stu-id="04e56-213">buildNumber</span></span>|<span data-ttu-id="04e56-214">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04e56-214">String</span></span>|<span data-ttu-id="04e56-215">Die Buildnummer der branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="04e56-215">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="04e56-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="04e56-216">Response</span></span>
<span data-ttu-id="04e56-217">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosLobApp](../resources/intune_apps_ioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04e56-217">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune_apps_ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04e56-218">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04e56-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="04e56-219">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04e56-219">Request</span></span>
<span data-ttu-id="04e56-220">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04e56-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04e56-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="04e56-221">Response</span></span>
<span data-ttu-id="04e56-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04e56-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








