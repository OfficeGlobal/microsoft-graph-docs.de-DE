# <a name="create-windowsuniversalappx"></a><span data-ttu-id="36572-101">windowsUniversalAppX erstellen</span><span class="sxs-lookup"><span data-stu-id="36572-101">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="36572-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="36572-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36572-103">Erstellen eines neuen [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="36572-103">Create a new [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36572-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="36572-104">Prerequisites</span></span>
<span data-ttu-id="36572-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="36572-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="36572-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="36572-107">Permission type</span></span>|<span data-ttu-id="36572-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="36572-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36572-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="36572-109">Delegated (work or school account)</span></span>|<span data-ttu-id="36572-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36572-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="36572-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="36572-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36572-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36572-112">Not supported.</span></span>|
|<span data-ttu-id="36572-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="36572-113">Application</span></span>|<span data-ttu-id="36572-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36572-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36572-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="36572-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="36572-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="36572-116">Request headers</span></span>
|<span data-ttu-id="36572-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="36572-117">Header</span></span>|<span data-ttu-id="36572-118">Wert</span><span class="sxs-lookup"><span data-stu-id="36572-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36572-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="36572-119">Authorization</span></span>|<span data-ttu-id="36572-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="36572-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36572-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="36572-121">Accept</span></span>|<span data-ttu-id="36572-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="36572-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36572-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="36572-123">Request body</span></span>
<span data-ttu-id="36572-124">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsUniversalAppX-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="36572-124">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="36572-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsUniversalAppX erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="36572-125">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="36572-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="36572-126">Property</span></span>|<span data-ttu-id="36572-127">Typ</span><span class="sxs-lookup"><span data-stu-id="36572-127">Type</span></span>|<span data-ttu-id="36572-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36572-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36572-129">ID</span><span class="sxs-lookup"><span data-stu-id="36572-129">id</span></span>|<span data-ttu-id="36572-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-130">String</span></span>|<span data-ttu-id="36572-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="36572-131">Key of the entity.</span></span> <span data-ttu-id="36572-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="36572-133">displayName</span><span class="sxs-lookup"><span data-stu-id="36572-133">displayName</span></span>|<span data-ttu-id="36572-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-134">String</span></span>|<span data-ttu-id="36572-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="36572-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="36572-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="36572-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36572-137">description</span></span>|<span data-ttu-id="36572-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-138">String</span></span>|<span data-ttu-id="36572-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="36572-139">The description of the app.</span></span> <span data-ttu-id="36572-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="36572-141">Verleger</span><span class="sxs-lookup"><span data-stu-id="36572-141">publisher</span></span>|<span data-ttu-id="36572-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-142">String</span></span>|<span data-ttu-id="36572-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="36572-143">The publisher of the app.</span></span> <span data-ttu-id="36572-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="36572-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="36572-145">largeIcon</span></span>|[<span data-ttu-id="36572-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="36572-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="36572-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="36572-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="36572-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="36572-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36572-149">createdDateTime</span></span>|<span data-ttu-id="36572-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36572-150">DateTimeOffset</span></span>|<span data-ttu-id="36572-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="36572-151">The date and time the app was created.</span></span> <span data-ttu-id="36572-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="36572-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36572-153">lastModifiedDateTime</span></span>|<span data-ttu-id="36572-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36572-154">DateTimeOffset</span></span>|<span data-ttu-id="36572-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="36572-155">The date and time the app was last modified.</span></span> <span data-ttu-id="36572-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="36572-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="36572-157">isFeatured</span></span>|<span data-ttu-id="36572-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="36572-158">Boolean</span></span>|<span data-ttu-id="36572-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="36572-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="36572-160">privacyInformationUrl</span></span>|<span data-ttu-id="36572-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-161">String</span></span>|<span data-ttu-id="36572-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="36572-162">The privacy statement Url.</span></span> <span data-ttu-id="36572-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="36572-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="36572-164">informationUrl</span></span>|<span data-ttu-id="36572-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-165">String</span></span>|<span data-ttu-id="36572-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="36572-166">The more information Url.</span></span> <span data-ttu-id="36572-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="36572-168">Besitzer</span><span class="sxs-lookup"><span data-stu-id="36572-168">owner</span></span>|<span data-ttu-id="36572-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-169">String</span></span>|<span data-ttu-id="36572-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="36572-170">The owner of the app.</span></span> <span data-ttu-id="36572-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="36572-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="36572-172">developer</span></span>|<span data-ttu-id="36572-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-173">String</span></span>|<span data-ttu-id="36572-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="36572-174">The developer of the app.</span></span> <span data-ttu-id="36572-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="36572-176">Notiz</span><span class="sxs-lookup"><span data-stu-id="36572-176">notes</span></span>|<span data-ttu-id="36572-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-177">String</span></span>|<span data-ttu-id="36572-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="36572-178">Notes for the app.</span></span> <span data-ttu-id="36572-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="36572-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="36572-180">publishingState</span></span>|[<span data-ttu-id="36572-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="36572-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="36572-p114">Der Veröffentlichungsstand der App. Die App kann nur dann zugewiesen werden, wenn die App veröffentlicht wird. Vererbt von [mobileApp](../resources/intune_apps_mobileapp.md). Die möglichen Werte sind: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="36572-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="36572-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="36572-186">committedContentVersion</span></span>|<span data-ttu-id="36572-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-187">String</span></span>|<span data-ttu-id="36572-188">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="36572-188">The internal committed content version.</span></span> <span data-ttu-id="36572-189">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="36572-190">fileName</span><span class="sxs-lookup"><span data-stu-id="36572-190">fileName</span></span>|<span data-ttu-id="36572-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-191">String</span></span>|<span data-ttu-id="36572-192">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="36572-192">The name of the main Lob application file.</span></span> <span data-ttu-id="36572-193">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="36572-194">Größe</span><span class="sxs-lookup"><span data-stu-id="36572-194">size</span></span>|<span data-ttu-id="36572-195">Int64</span><span class="sxs-lookup"><span data-stu-id="36572-195">Int64</span></span>|<span data-ttu-id="36572-196">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="36572-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="36572-197">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="36572-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="36572-198">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="36572-198">applicableArchitectures</span></span>|[<span data-ttu-id="36572-199">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="36572-199">windowsArchitecture</span></span>](../resources/intune_apps_windowsarchitecture.md)|<span data-ttu-id="36572-p118">Die Windows-Architekture(n), für die diese App ausgeführt werden kann. Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="36572-p118">The Windows architecture(s) for which this app can run on. The possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="36572-202">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="36572-202">applicableDeviceTypes</span></span>|[<span data-ttu-id="36572-203">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="36572-203">windowsDeviceType</span></span>](../resources/intune_apps_windowsdevicetype.md)|<span data-ttu-id="36572-p119">Die Windows-Gerätetypen, für die diese App ausgeführt werden kann. Mögliche Werte sind: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="36572-p119">The Windows device type(s) for which this app can run on. The possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="36572-206">identityName</span><span class="sxs-lookup"><span data-stu-id="36572-206">identityName</span></span>|<span data-ttu-id="36572-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-207">String</span></span>|<span data-ttu-id="36572-208">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="36572-208">The Identity Name.</span></span>|
|<span data-ttu-id="36572-209">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="36572-209">identityPublisherHash</span></span>|<span data-ttu-id="36572-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-210">String</span></span>|<span data-ttu-id="36572-211">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="36572-211">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="36572-212">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="36572-212">identityResourceIdentifier</span></span>|<span data-ttu-id="36572-213">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-213">String</span></span>|<span data-ttu-id="36572-214">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="36572-214">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="36572-215">isBundle</span><span class="sxs-lookup"><span data-stu-id="36572-215">isBundle</span></span>|<span data-ttu-id="36572-216">Boolesch</span><span class="sxs-lookup"><span data-stu-id="36572-216">Boolean</span></span>|<span data-ttu-id="36572-217">Gibt an, ob die App ein Bundle ist.</span><span class="sxs-lookup"><span data-stu-id="36572-217">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="36572-218">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="36572-218">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="36572-219">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="36572-219">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="36572-220">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="36572-220">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="36572-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="36572-221">identityVersion</span></span>|<span data-ttu-id="36572-222">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="36572-222">String</span></span>|<span data-ttu-id="36572-223">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="36572-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="36572-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="36572-224">Response</span></span>
<span data-ttu-id="36572-225">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="36572-225">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36572-226">Beispiel</span><span class="sxs-lookup"><span data-stu-id="36572-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="36572-227">Anforderung</span><span class="sxs-lookup"><span data-stu-id="36572-227">Request</span></span>
<span data-ttu-id="36572-228">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36572-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1253

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

### <a name="response"></a><span data-ttu-id="36572-229">Antwort</span><span class="sxs-lookup"><span data-stu-id="36572-229">Response</span></span>
<span data-ttu-id="36572-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36572-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








