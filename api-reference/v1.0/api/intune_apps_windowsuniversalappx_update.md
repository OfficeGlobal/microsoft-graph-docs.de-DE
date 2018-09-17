# <a name="update-windowsuniversalappx"></a><span data-ttu-id="80edd-101">windowsUniversalAppX aktualisieren</span><span class="sxs-lookup"><span data-stu-id="80edd-101">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="80edd-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="80edd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80edd-103">Aktualisieren der Eigenschaften eines [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="80edd-103">Update the properties of a [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80edd-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="80edd-104">Prerequisites</span></span>
<span data-ttu-id="80edd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="80edd-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80edd-107">Permission type</span></span>|<span data-ttu-id="80edd-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80edd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80edd-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80edd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="80edd-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80edd-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="80edd-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80edd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80edd-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80edd-112">Not supported.</span></span>|
|<span data-ttu-id="80edd-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80edd-113">Application</span></span>|<span data-ttu-id="80edd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80edd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80edd-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80edd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="80edd-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80edd-116">Request headers</span></span>
|<span data-ttu-id="80edd-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="80edd-117">Header</span></span>|<span data-ttu-id="80edd-118">Wert</span><span class="sxs-lookup"><span data-stu-id="80edd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80edd-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="80edd-119">Authorization</span></span>|<span data-ttu-id="80edd-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="80edd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80edd-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="80edd-121">Accept</span></span>|<span data-ttu-id="80edd-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="80edd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80edd-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80edd-123">Request body</span></span>
<span data-ttu-id="80edd-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="80edd-124">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="80edd-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="80edd-125">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span></span>

|<span data-ttu-id="80edd-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80edd-126">Property</span></span>|<span data-ttu-id="80edd-127">Typ</span><span class="sxs-lookup"><span data-stu-id="80edd-127">Type</span></span>|<span data-ttu-id="80edd-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80edd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80edd-129">ID</span><span class="sxs-lookup"><span data-stu-id="80edd-129">id</span></span>|<span data-ttu-id="80edd-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-130">String</span></span>|<span data-ttu-id="80edd-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="80edd-131">Key of the entity.</span></span> <span data-ttu-id="80edd-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="80edd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="80edd-133">displayName</span></span>|<span data-ttu-id="80edd-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-134">String</span></span>|<span data-ttu-id="80edd-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="80edd-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="80edd-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="80edd-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80edd-137">description</span></span>|<span data-ttu-id="80edd-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-138">String</span></span>|<span data-ttu-id="80edd-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="80edd-139">The description of the app.</span></span> <span data-ttu-id="80edd-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="80edd-141">Verleger</span><span class="sxs-lookup"><span data-stu-id="80edd-141">publisher</span></span>|<span data-ttu-id="80edd-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-142">String</span></span>|<span data-ttu-id="80edd-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="80edd-143">The publisher of the app.</span></span> <span data-ttu-id="80edd-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="80edd-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="80edd-145">largeIcon</span></span>|[<span data-ttu-id="80edd-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="80edd-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="80edd-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="80edd-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="80edd-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="80edd-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80edd-149">createdDateTime</span></span>|<span data-ttu-id="80edd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80edd-150">DateTimeOffset</span></span>|<span data-ttu-id="80edd-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="80edd-151">The date and time the app was created.</span></span> <span data-ttu-id="80edd-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="80edd-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80edd-153">lastModifiedDateTime</span></span>|<span data-ttu-id="80edd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80edd-154">DateTimeOffset</span></span>|<span data-ttu-id="80edd-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="80edd-155">The date and time the app was last modified.</span></span> <span data-ttu-id="80edd-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="80edd-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="80edd-157">isFeatured</span></span>|<span data-ttu-id="80edd-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="80edd-158">Boolean</span></span>|<span data-ttu-id="80edd-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="80edd-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="80edd-160">privacyInformationUrl</span></span>|<span data-ttu-id="80edd-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-161">String</span></span>|<span data-ttu-id="80edd-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="80edd-162">The privacy statement Url.</span></span> <span data-ttu-id="80edd-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="80edd-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="80edd-164">informationUrl</span></span>|<span data-ttu-id="80edd-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-165">String</span></span>|<span data-ttu-id="80edd-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="80edd-166">The more information Url.</span></span> <span data-ttu-id="80edd-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="80edd-168">owner</span><span class="sxs-lookup"><span data-stu-id="80edd-168">owner</span></span>|<span data-ttu-id="80edd-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-169">String</span></span>|<span data-ttu-id="80edd-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="80edd-170">The owner of the app.</span></span> <span data-ttu-id="80edd-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="80edd-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="80edd-172">developer</span></span>|<span data-ttu-id="80edd-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-173">String</span></span>|<span data-ttu-id="80edd-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="80edd-174">The developer of the app.</span></span> <span data-ttu-id="80edd-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="80edd-176">Hinweise</span><span class="sxs-lookup"><span data-stu-id="80edd-176">notes</span></span>|<span data-ttu-id="80edd-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-177">String</span></span>|<span data-ttu-id="80edd-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="80edd-178">Notes for the app.</span></span> <span data-ttu-id="80edd-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="80edd-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="80edd-180">publishingState</span></span>|[<span data-ttu-id="80edd-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="80edd-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="80edd-182">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="80edd-182">The publishing state for the app.</span></span> <span data-ttu-id="80edd-183">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="80edd-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="80edd-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="80edd-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="80edd-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="80edd-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="80edd-186">committedContentVersion</span></span>|<span data-ttu-id="80edd-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-187">String</span></span>|<span data-ttu-id="80edd-188">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="80edd-188">The internal committed content version.</span></span> <span data-ttu-id="80edd-189">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="80edd-190">fileName</span><span class="sxs-lookup"><span data-stu-id="80edd-190">fileName</span></span>|<span data-ttu-id="80edd-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-191">String</span></span>|<span data-ttu-id="80edd-192">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="80edd-192">The name of the main Lob application file.</span></span> <span data-ttu-id="80edd-193">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="80edd-194">size</span><span class="sxs-lookup"><span data-stu-id="80edd-194">size</span></span>|<span data-ttu-id="80edd-195">Int64</span><span class="sxs-lookup"><span data-stu-id="80edd-195">Int64</span></span>|<span data-ttu-id="80edd-196">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="80edd-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="80edd-197">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="80edd-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="80edd-198">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="80edd-198">applicableArchitectures</span></span>|[<span data-ttu-id="80edd-199">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="80edd-199">windowsArchitecture</span></span>](../resources/intune_apps_windowsarchitecture.md)|<span data-ttu-id="80edd-200">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="80edd-200">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="80edd-201">Mögliche Werte: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="80edd-201">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="80edd-202">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="80edd-202">applicableDeviceTypes</span></span>|[<span data-ttu-id="80edd-203">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="80edd-203">windowsDeviceType</span></span>](../resources/intune_apps_windowsdevicetype.md)|<span data-ttu-id="80edd-204">Die Windows-Gerätetypen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="80edd-204">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="80edd-205">Mögliche Werte: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="80edd-205">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="80edd-206">identityName</span><span class="sxs-lookup"><span data-stu-id="80edd-206">identityName</span></span>|<span data-ttu-id="80edd-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-207">String</span></span>|<span data-ttu-id="80edd-208">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="80edd-208">The Identity Name.</span></span>|
|<span data-ttu-id="80edd-209">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="80edd-209">identityPublisherHash</span></span>|<span data-ttu-id="80edd-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-210">String</span></span>|<span data-ttu-id="80edd-211">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="80edd-211">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="80edd-212">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="80edd-212">identityResourceIdentifier</span></span>|<span data-ttu-id="80edd-213">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-213">String</span></span>|<span data-ttu-id="80edd-214">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="80edd-214">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="80edd-215">isBundle</span><span class="sxs-lookup"><span data-stu-id="80edd-215">isBundle</span></span>|<span data-ttu-id="80edd-216">Boolesch</span><span class="sxs-lookup"><span data-stu-id="80edd-216">Boolean</span></span>|<span data-ttu-id="80edd-217">Gibt an, ob die App ein Bundle ist.</span><span class="sxs-lookup"><span data-stu-id="80edd-217">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="80edd-218">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="80edd-218">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="80edd-219">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="80edd-219">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="80edd-220">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="80edd-220">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="80edd-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="80edd-221">identityVersion</span></span>|<span data-ttu-id="80edd-222">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80edd-222">String</span></span>|<span data-ttu-id="80edd-223">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="80edd-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="80edd-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="80edd-224">Response</span></span>
<span data-ttu-id="80edd-225">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="80edd-225">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80edd-226">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80edd-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="80edd-227">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80edd-227">Request</span></span>
<span data-ttu-id="80edd-228">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80edd-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1194

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

### <a name="response"></a><span data-ttu-id="80edd-229">Antwort</span><span class="sxs-lookup"><span data-stu-id="80edd-229">Response</span></span>
<span data-ttu-id="80edd-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80edd-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








