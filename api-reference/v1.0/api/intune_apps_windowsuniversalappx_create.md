# <a name="create-windowsuniversalappx"></a><span data-ttu-id="3afa8-101">windowsUniversalAppX erstellen</span><span class="sxs-lookup"><span data-stu-id="3afa8-101">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="3afa8-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3afa8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3afa8-103">Erstellen eines neuen [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3afa8-103">Create a new [plannerBucket](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3afa8-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3afa8-104">Prerequisites</span></span>
<span data-ttu-id="3afa8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3afa8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3afa8-107">Permission type</span></span>|<span data-ttu-id="3afa8-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3afa8-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3afa8-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3afa8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3afa8-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3afa8-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3afa8-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3afa8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3afa8-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3afa8-112">Not supported.</span></span>|
|<span data-ttu-id="3afa8-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3afa8-113">Application</span></span>|<span data-ttu-id="3afa8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3afa8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3afa8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3afa8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3afa8-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3afa8-116">Request headers</span></span>
|<span data-ttu-id="3afa8-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3afa8-117">Header</span></span>|<span data-ttu-id="3afa8-118">Wert</span><span class="sxs-lookup"><span data-stu-id="3afa8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3afa8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3afa8-119">Authorization</span></span>|<span data-ttu-id="3afa8-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3afa8-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3afa8-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3afa8-121">Accept</span></span>|<span data-ttu-id="3afa8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3afa8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3afa8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3afa8-123">Request body</span></span>
<span data-ttu-id="3afa8-124">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsUniversalAppX-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3afa8-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="3afa8-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsUniversalAppX erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3afa8-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="3afa8-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3afa8-126">Property</span></span>|<span data-ttu-id="3afa8-127">Typ</span><span class="sxs-lookup"><span data-stu-id="3afa8-127">Type</span></span>|<span data-ttu-id="3afa8-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3afa8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3afa8-129">id</span><span class="sxs-lookup"><span data-stu-id="3afa8-129">id</span></span>|<span data-ttu-id="3afa8-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-130">String</span></span>|<span data-ttu-id="3afa8-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="3afa8-131">Key of the setting.</span></span> <span data-ttu-id="3afa8-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3afa8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3afa8-133">displayName</span></span>|<span data-ttu-id="3afa8-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-134">String</span></span>|<span data-ttu-id="3afa8-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="3afa8-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3afa8-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3afa8-137">description</span><span class="sxs-lookup"><span data-stu-id="3afa8-137">description</span></span>|<span data-ttu-id="3afa8-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-138">String</span></span>|<span data-ttu-id="3afa8-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="3afa8-139">The description of the app.</span></span> <span data-ttu-id="3afa8-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3afa8-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="3afa8-141">Publisher</span></span>|<span data-ttu-id="3afa8-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-142">String</span></span>|<span data-ttu-id="3afa8-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="3afa8-143">The name of the app.</span></span> <span data-ttu-id="3afa8-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3afa8-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3afa8-145">largeIcon</span></span>|[<span data-ttu-id="3afa8-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3afa8-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="3afa8-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="3afa8-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3afa8-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3afa8-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3afa8-149">createdDateTime</span></span>|<span data-ttu-id="3afa8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3afa8-150">DateTimeOffset</span></span>|<span data-ttu-id="3afa8-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="3afa8-151">The date and time the group was created.</span></span> <span data-ttu-id="3afa8-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3afa8-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3afa8-153">lastModifiedDateTime</span></span>|<span data-ttu-id="3afa8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3afa8-154">DateTimeOffset</span></span>|<span data-ttu-id="3afa8-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="3afa8-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="3afa8-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3afa8-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3afa8-157">isFeatured</span></span>|<span data-ttu-id="3afa8-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3afa8-158">Boolean</span></span>|<span data-ttu-id="3afa8-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3afa8-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3afa8-160">privacyInformationUrl</span></span>|<span data-ttu-id="3afa8-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-161">String</span></span>|<span data-ttu-id="3afa8-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="3afa8-162">The privacy statement Url.</span></span> <span data-ttu-id="3afa8-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3afa8-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3afa8-164">informationUrl</span></span>|<span data-ttu-id="3afa8-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-165">String</span></span>|<span data-ttu-id="3afa8-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="3afa8-166">The more information Url.</span></span> <span data-ttu-id="3afa8-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3afa8-168">owner</span><span class="sxs-lookup"><span data-stu-id="3afa8-168">owner</span></span>|<span data-ttu-id="3afa8-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-169">String</span></span>|<span data-ttu-id="3afa8-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="3afa8-170">The owner of the app.</span></span> <span data-ttu-id="3afa8-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3afa8-172">developer</span><span class="sxs-lookup"><span data-stu-id="3afa8-172">developer</span></span>|<span data-ttu-id="3afa8-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-173">String</span></span>|<span data-ttu-id="3afa8-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="3afa8-174">The name of the app.</span></span> <span data-ttu-id="3afa8-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3afa8-176">notes</span><span class="sxs-lookup"><span data-stu-id="3afa8-176">notes</span></span>|<span data-ttu-id="3afa8-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-177">String</span></span>|<span data-ttu-id="3afa8-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="3afa8-178">Notes for the app.</span></span> <span data-ttu-id="3afa8-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3afa8-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="3afa8-180">publishingState</span></span>|<span data-ttu-id="3afa8-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-181">String</span></span>|<span data-ttu-id="3afa8-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="3afa8-182">The publishing state for the app.</span></span> <span data-ttu-id="3afa8-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="3afa8-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3afa8-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="3afa8-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3afa8-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3afa8-185">committedContentVersion</span></span>|<span data-ttu-id="3afa8-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-186">String</span></span>|<span data-ttu-id="3afa8-187">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="3afa8-187">The internal committed content version.</span></span> <span data-ttu-id="3afa8-188">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="3afa8-189">fileName</span><span class="sxs-lookup"><span data-stu-id="3afa8-189">fileName</span></span>|<span data-ttu-id="3afa8-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-190">String</span></span>|<span data-ttu-id="3afa8-191">Der Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="3afa8-191">The name of the main Lob application file.</span></span> <span data-ttu-id="3afa8-192">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="3afa8-193">size</span><span class="sxs-lookup"><span data-stu-id="3afa8-193">size</span></span>|<span data-ttu-id="3afa8-194">Int64</span><span class="sxs-lookup"><span data-stu-id="3afa8-194">Int64</span></span>|<span data-ttu-id="3afa8-195">Die Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="3afa8-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="3afa8-196">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3afa8-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="3afa8-197">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="3afa8-197">applicableArchitectures</span></span>|<span data-ttu-id="3afa8-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-198">String</span></span>|<span data-ttu-id="3afa8-199">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="3afa8-199">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="3afa8-200">Mögliche Werte: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="3afa8-200">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="3afa8-201">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="3afa8-201">applicableDeviceTypes</span></span>|<span data-ttu-id="3afa8-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-202">String</span></span>|<span data-ttu-id="3afa8-203">Die Windows-Gerätetypen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="3afa8-203">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="3afa8-204">Mögliche Werte: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="3afa8-204">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="3afa8-205">identityName</span><span class="sxs-lookup"><span data-stu-id="3afa8-205">identityName</span></span>|<span data-ttu-id="3afa8-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-206">String</span></span>|<span data-ttu-id="3afa8-207">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="3afa8-207">The Identity Name.</span></span>|
|<span data-ttu-id="3afa8-208">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="3afa8-208">identityPublisherHash</span></span>|<span data-ttu-id="3afa8-209">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-209">String</span></span>|<span data-ttu-id="3afa8-210">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="3afa8-210">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="3afa8-211">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="3afa8-211">identityResourceIdentifier</span></span>|<span data-ttu-id="3afa8-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-212">String</span></span>|<span data-ttu-id="3afa8-213">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="3afa8-213">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="3afa8-214">isBundle</span><span class="sxs-lookup"><span data-stu-id="3afa8-214">isBundle</span></span>|<span data-ttu-id="3afa8-215">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3afa8-215">Boolean</span></span>|<span data-ttu-id="3afa8-216">Gibt an, ob die App ein Bundle ist.</span><span class="sxs-lookup"><span data-stu-id="3afa8-216">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="3afa8-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3afa8-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3afa8-218">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3afa8-218">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="3afa8-219">Der Wert für die Mindestversion des verwendbaren Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="3afa8-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="3afa8-220">identityVersion</span><span class="sxs-lookup"><span data-stu-id="3afa8-220">identityVersion</span></span>|<span data-ttu-id="3afa8-221">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3afa8-221">String</span></span>|<span data-ttu-id="3afa8-222">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="3afa8-222">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="3afa8-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="3afa8-223">Response</span></span>
<span data-ttu-id="3afa8-224">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3afa8-224">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3afa8-225">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3afa8-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="3afa8-226">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3afa8-226">Request</span></span>
<span data-ttu-id="3afa8-227">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3afa8-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3afa8-228">Antwort</span><span class="sxs-lookup"><span data-stu-id="3afa8-228">Response</span></span>
<span data-ttu-id="3afa8-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3afa8-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



