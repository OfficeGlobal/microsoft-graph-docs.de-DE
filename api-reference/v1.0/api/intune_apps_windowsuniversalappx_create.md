# <a name="create-windowsuniversalappx"></a><span data-ttu-id="251b4-101">windowsUniversalAppX erstellen</span><span class="sxs-lookup"><span data-stu-id="251b4-101">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="251b4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="251b4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="251b4-103">Erstellen eines neuen [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="251b4-103">Create a new [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="251b4-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="251b4-104">Prerequisites</span></span>
<span data-ttu-id="251b4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="251b4-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="251b4-107">Permission type</span></span>|<span data-ttu-id="251b4-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="251b4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="251b4-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="251b4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="251b4-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="251b4-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="251b4-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="251b4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="251b4-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="251b4-112">Not supported.</span></span>|
|<span data-ttu-id="251b4-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="251b4-113">Application</span></span>|<span data-ttu-id="251b4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="251b4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="251b4-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="251b4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="251b4-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="251b4-116">Request headers</span></span>
|<span data-ttu-id="251b4-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="251b4-117">Header</span></span>|<span data-ttu-id="251b4-118">Wert</span><span class="sxs-lookup"><span data-stu-id="251b4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="251b4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="251b4-119">Authorization</span></span>|<span data-ttu-id="251b4-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="251b4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="251b4-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="251b4-121">Accept</span></span>|<span data-ttu-id="251b4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="251b4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="251b4-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="251b4-123">Request body</span></span>
<span data-ttu-id="251b4-124">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsUniversalAppX-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="251b4-124">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="251b4-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsUniversalAppX erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="251b4-125">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="251b4-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="251b4-126">Property</span></span>|<span data-ttu-id="251b4-127">Typ</span><span class="sxs-lookup"><span data-stu-id="251b4-127">Type</span></span>|<span data-ttu-id="251b4-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="251b4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="251b4-129">id</span><span class="sxs-lookup"><span data-stu-id="251b4-129">id</span></span>|<span data-ttu-id="251b4-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-130">String</span></span>|<span data-ttu-id="251b4-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="251b4-131">Key of the entity.</span></span> <span data-ttu-id="251b4-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="251b4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="251b4-133">displayName</span></span>|<span data-ttu-id="251b4-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-134">String</span></span>|<span data-ttu-id="251b4-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="251b4-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="251b4-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="251b4-137">description</span><span class="sxs-lookup"><span data-stu-id="251b4-137">description</span></span>|<span data-ttu-id="251b4-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-138">String</span></span>|<span data-ttu-id="251b4-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="251b4-139">The description of the app.</span></span> <span data-ttu-id="251b4-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="251b4-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="251b4-141">publisher</span></span>|<span data-ttu-id="251b4-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-142">String</span></span>|<span data-ttu-id="251b4-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="251b4-143">The publisher of the app.</span></span> <span data-ttu-id="251b4-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="251b4-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="251b4-145">largeIcon</span></span>|[<span data-ttu-id="251b4-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="251b4-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="251b4-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="251b4-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="251b4-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="251b4-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="251b4-149">createdDateTime</span></span>|<span data-ttu-id="251b4-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="251b4-150">DateTimeOffset</span></span>|<span data-ttu-id="251b4-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="251b4-151">The date and time the app was created.</span></span> <span data-ttu-id="251b4-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="251b4-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="251b4-153">lastModifiedDateTime</span></span>|<span data-ttu-id="251b4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="251b4-154">DateTimeOffset</span></span>|<span data-ttu-id="251b4-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="251b4-155">The date and time the app was last modified.</span></span> <span data-ttu-id="251b4-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="251b4-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="251b4-157">isFeatured</span></span>|<span data-ttu-id="251b4-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="251b4-158">Boolean</span></span>|<span data-ttu-id="251b4-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="251b4-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="251b4-160">privacyInformationUrl</span></span>|<span data-ttu-id="251b4-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-161">String</span></span>|<span data-ttu-id="251b4-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="251b4-162">The privacy statement Url.</span></span> <span data-ttu-id="251b4-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="251b4-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="251b4-164">informationUrl</span></span>|<span data-ttu-id="251b4-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-165">String</span></span>|<span data-ttu-id="251b4-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="251b4-166">The more information Url.</span></span> <span data-ttu-id="251b4-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="251b4-168">owner</span><span class="sxs-lookup"><span data-stu-id="251b4-168">owner</span></span>|<span data-ttu-id="251b4-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-169">String</span></span>|<span data-ttu-id="251b4-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="251b4-170">The owner of the app.</span></span> <span data-ttu-id="251b4-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="251b4-172">developer</span><span class="sxs-lookup"><span data-stu-id="251b4-172">developer</span></span>|<span data-ttu-id="251b4-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-173">String</span></span>|<span data-ttu-id="251b4-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="251b4-174">The developer of the app.</span></span> <span data-ttu-id="251b4-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="251b4-176">notes</span><span class="sxs-lookup"><span data-stu-id="251b4-176">notes</span></span>|<span data-ttu-id="251b4-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-177">String</span></span>|<span data-ttu-id="251b4-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="251b4-178">Notes for the app.</span></span> <span data-ttu-id="251b4-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="251b4-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="251b4-180">publishingState</span></span>|[<span data-ttu-id="251b4-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="251b4-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="251b4-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="251b4-182">The publishing state for the app.</span></span> <span data-ttu-id="251b4-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="251b4-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="251b4-184">Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="251b4-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="251b4-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="251b4-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="251b4-186">committedContentVersion</span></span>|<span data-ttu-id="251b4-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-187">String</span></span>|<span data-ttu-id="251b4-188">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="251b4-188">The internal committed content version.</span></span> <span data-ttu-id="251b4-189">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="251b4-190">fileName</span><span class="sxs-lookup"><span data-stu-id="251b4-190">fileName</span></span>|<span data-ttu-id="251b4-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-191">String</span></span>|<span data-ttu-id="251b4-192">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="251b4-192">The name of the main Lob application file.</span></span> <span data-ttu-id="251b4-193">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="251b4-194">size</span><span class="sxs-lookup"><span data-stu-id="251b4-194">size</span></span>|<span data-ttu-id="251b4-195">Int64</span><span class="sxs-lookup"><span data-stu-id="251b4-195">Int64</span></span>|<span data-ttu-id="251b4-196">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="251b4-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="251b4-197">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="251b4-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="251b4-198">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="251b4-198">applicableArchitectures</span></span>|[<span data-ttu-id="251b4-199">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="251b4-199">windowsArchitecture</span></span>](../resources/intune_apps_windowsarchitecture.md)|<span data-ttu-id="251b4-200">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="251b4-200">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="251b4-201">Mögliche Werte: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="251b4-201">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="251b4-202">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="251b4-202">applicableDeviceTypes</span></span>|[<span data-ttu-id="251b4-203">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="251b4-203">windowsDeviceType</span></span>](../resources/intune_apps_windowsdevicetype.md)|<span data-ttu-id="251b4-204">Die Windows-Gerätetypen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="251b4-204">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="251b4-205">Mögliche Werte: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="251b4-205">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="251b4-206">identityName</span><span class="sxs-lookup"><span data-stu-id="251b4-206">identityName</span></span>|<span data-ttu-id="251b4-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-207">String</span></span>|<span data-ttu-id="251b4-208">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="251b4-208">The Identity Name.</span></span>|
|<span data-ttu-id="251b4-209">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="251b4-209">identityPublisherHash</span></span>|<span data-ttu-id="251b4-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-210">String</span></span>|<span data-ttu-id="251b4-211">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="251b4-211">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="251b4-212">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="251b4-212">identityResourceIdentifier</span></span>|<span data-ttu-id="251b4-213">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-213">String</span></span>|<span data-ttu-id="251b4-214">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="251b4-214">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="251b4-215">isBundle</span><span class="sxs-lookup"><span data-stu-id="251b4-215">isBundle</span></span>|<span data-ttu-id="251b4-216">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="251b4-216">Boolean</span></span>|<span data-ttu-id="251b4-217">Gibt an, ob die App ein Bundle ist.</span><span class="sxs-lookup"><span data-stu-id="251b4-217">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="251b4-218">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="251b4-218">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="251b4-219">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="251b4-219">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="251b4-220">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="251b4-220">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="251b4-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="251b4-221">identityVersion</span></span>|<span data-ttu-id="251b4-222">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="251b4-222">String</span></span>|<span data-ttu-id="251b4-223">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="251b4-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="251b4-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="251b4-224">Response</span></span>
<span data-ttu-id="251b4-225">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="251b4-225">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="251b4-226">Beispiel</span><span class="sxs-lookup"><span data-stu-id="251b4-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="251b4-227">Anforderung</span><span class="sxs-lookup"><span data-stu-id="251b4-227">Request</span></span>
<span data-ttu-id="251b4-228">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="251b4-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="251b4-229">Antwort</span><span class="sxs-lookup"><span data-stu-id="251b4-229">Response</span></span>
<span data-ttu-id="251b4-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="251b4-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```



