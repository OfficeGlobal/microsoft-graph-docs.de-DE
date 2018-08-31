# <a name="update-managedioslobapp"></a><span data-ttu-id="430e5-101">managedIOSLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="430e5-101">Update managedIOSLobApp</span></span>

> <span data-ttu-id="430e5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="430e5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="430e5-103">Aktualisieren der Eigenschaften eines [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="430e5-103">Update the properties of a [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="430e5-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="430e5-104">Prerequisites</span></span>
<span data-ttu-id="430e5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="430e5-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="430e5-107">Permission type</span></span>|<span data-ttu-id="430e5-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="430e5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="430e5-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="430e5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="430e5-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="430e5-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="430e5-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="430e5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="430e5-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="430e5-112">Not supported.</span></span>|
|<span data-ttu-id="430e5-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="430e5-113">Application</span></span>|<span data-ttu-id="430e5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="430e5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="430e5-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="430e5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="430e5-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="430e5-116">Request headers</span></span>
|<span data-ttu-id="430e5-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="430e5-117">Header</span></span>|<span data-ttu-id="430e5-118">Wert</span><span class="sxs-lookup"><span data-stu-id="430e5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="430e5-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="430e5-119">Authorization</span></span>|<span data-ttu-id="430e5-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="430e5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="430e5-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="430e5-121">Accept</span></span>|<span data-ttu-id="430e5-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="430e5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="430e5-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="430e5-123">Request body</span></span>
<span data-ttu-id="430e5-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="430e5-124">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object.</span></span>

<span data-ttu-id="430e5-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="430e5-125">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span></span>

|<span data-ttu-id="430e5-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="430e5-126">Property</span></span>|<span data-ttu-id="430e5-127">Typ</span><span class="sxs-lookup"><span data-stu-id="430e5-127">Type</span></span>|<span data-ttu-id="430e5-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="430e5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="430e5-129">id</span><span class="sxs-lookup"><span data-stu-id="430e5-129">id</span></span>|<span data-ttu-id="430e5-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-130">String</span></span>|<span data-ttu-id="430e5-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="430e5-131">Key of the entity.</span></span> <span data-ttu-id="430e5-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="430e5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="430e5-133">displayName</span></span>|<span data-ttu-id="430e5-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-134">String</span></span>|<span data-ttu-id="430e5-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="430e5-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="430e5-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="430e5-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="430e5-137">description</span></span>|<span data-ttu-id="430e5-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-138">String</span></span>|<span data-ttu-id="430e5-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="430e5-139">The description of the app.</span></span> <span data-ttu-id="430e5-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="430e5-141">Verleger</span><span class="sxs-lookup"><span data-stu-id="430e5-141">publisher</span></span>|<span data-ttu-id="430e5-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-142">String</span></span>|<span data-ttu-id="430e5-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="430e5-143">The publisher of the app.</span></span> <span data-ttu-id="430e5-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="430e5-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="430e5-145">largeIcon</span></span>|[<span data-ttu-id="430e5-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="430e5-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="430e5-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="430e5-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="430e5-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="430e5-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="430e5-149">createdDateTime</span></span>|<span data-ttu-id="430e5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="430e5-150">DateTimeOffset</span></span>|<span data-ttu-id="430e5-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="430e5-151">The date and time the app was created.</span></span> <span data-ttu-id="430e5-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="430e5-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="430e5-153">lastModifiedDateTime</span></span>|<span data-ttu-id="430e5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="430e5-154">DateTimeOffset</span></span>|<span data-ttu-id="430e5-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="430e5-155">The date and time the app was last modified.</span></span> <span data-ttu-id="430e5-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="430e5-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="430e5-157">isFeatured</span></span>|<span data-ttu-id="430e5-158">boolesch</span><span class="sxs-lookup"><span data-stu-id="430e5-158">Boolean</span></span>|<span data-ttu-id="430e5-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="430e5-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="430e5-160">privacyInformationUrl</span></span>|<span data-ttu-id="430e5-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-161">String</span></span>|<span data-ttu-id="430e5-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="430e5-162">The privacy statement Url.</span></span> <span data-ttu-id="430e5-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="430e5-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="430e5-164">informationUrl</span></span>|<span data-ttu-id="430e5-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-165">String</span></span>|<span data-ttu-id="430e5-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="430e5-166">The more information Url.</span></span> <span data-ttu-id="430e5-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="430e5-168">Besitzer</span><span class="sxs-lookup"><span data-stu-id="430e5-168">owner</span></span>|<span data-ttu-id="430e5-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-169">String</span></span>|<span data-ttu-id="430e5-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="430e5-170">The owner of the app.</span></span> <span data-ttu-id="430e5-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="430e5-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="430e5-172">developer</span></span>|<span data-ttu-id="430e5-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-173">String</span></span>|<span data-ttu-id="430e5-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="430e5-174">The developer of the app.</span></span> <span data-ttu-id="430e5-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="430e5-176">Notizen</span><span class="sxs-lookup"><span data-stu-id="430e5-176">notes</span></span>|<span data-ttu-id="430e5-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-177">String</span></span>|<span data-ttu-id="430e5-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="430e5-178">Notes for the app.</span></span> <span data-ttu-id="430e5-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="430e5-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="430e5-180">publishingState</span></span>|[<span data-ttu-id="430e5-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="430e5-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="430e5-182">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="430e5-182">The publishing state for the app.</span></span> <span data-ttu-id="430e5-183">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="430e5-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="430e5-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="430e5-185">Mögliche Werte sind `notPublished`, `processing`,`published`.</span><span class="sxs-lookup"><span data-stu-id="430e5-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="430e5-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="430e5-186">appAvailability</span></span>|[<span data-ttu-id="430e5-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="430e5-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="430e5-188">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="430e5-188">The Application's availability.</span></span> <span data-ttu-id="430e5-189">Geerbt von [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span> <span data-ttu-id="430e5-190">Mögliche Werte sind: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="430e5-190">The possible values are:</span></span>|
|<span data-ttu-id="430e5-191">Version</span><span class="sxs-lookup"><span data-stu-id="430e5-191">version</span></span>|<span data-ttu-id="430e5-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-192">String</span></span>|<span data-ttu-id="430e5-193">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="430e5-193">The Application's version.</span></span> <span data-ttu-id="430e5-194">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="430e5-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="430e5-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="430e5-195">committedContentVersion</span></span>|<span data-ttu-id="430e5-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-196">String</span></span>|<span data-ttu-id="430e5-197">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="430e5-197">The internal committed content version.</span></span> <span data-ttu-id="430e5-198">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="430e5-199">fileName</span><span class="sxs-lookup"><span data-stu-id="430e5-199">fileName</span></span>|<span data-ttu-id="430e5-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-200">String</span></span>|<span data-ttu-id="430e5-201">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="430e5-201">The name of the main Lob application file.</span></span> <span data-ttu-id="430e5-202">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="430e5-203">Größe</span><span class="sxs-lookup"><span data-stu-id="430e5-203">size</span></span>|<span data-ttu-id="430e5-204">Int64</span><span class="sxs-lookup"><span data-stu-id="430e5-204">Int64</span></span>|<span data-ttu-id="430e5-205">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="430e5-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="430e5-206">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="430e5-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="430e5-207">bundled</span><span class="sxs-lookup"><span data-stu-id="430e5-207">bundleId</span></span>|<span data-ttu-id="430e5-208">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-208">String</span></span>|<span data-ttu-id="430e5-209">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="430e5-209">The Identity Name.</span></span>|
|<span data-ttu-id="430e5-210">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="430e5-210">applicableDeviceType</span></span>|[<span data-ttu-id="430e5-211">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="430e5-211">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="430e5-212">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="430e5-212">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="430e5-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="430e5-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="430e5-214">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="430e5-214">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="430e5-215">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="430e5-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="430e5-216">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="430e5-216">expirationDateTime</span></span>|<span data-ttu-id="430e5-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="430e5-217">DateTimeOffset</span></span>|<span data-ttu-id="430e5-218">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="430e5-218">The expiration time.</span></span>|
|<span data-ttu-id="430e5-219">versionNumber</span><span class="sxs-lookup"><span data-stu-id="430e5-219">versionNumber</span></span>|<span data-ttu-id="430e5-220">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-220">String</span></span>|<span data-ttu-id="430e5-221">Die Versionsnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="430e5-221">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="430e5-222">buildNumber</span><span class="sxs-lookup"><span data-stu-id="430e5-222">buildNumber</span></span>|<span data-ttu-id="430e5-223">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="430e5-223">String</span></span>|<span data-ttu-id="430e5-224">Die Buildnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="430e5-224">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="430e5-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="430e5-225">Response</span></span>
<span data-ttu-id="430e5-226">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="430e5-226">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="430e5-227">Beispiel</span><span class="sxs-lookup"><span data-stu-id="430e5-227">Example</span></span>
### <a name="request"></a><span data-ttu-id="430e5-228">Anforderung</span><span class="sxs-lookup"><span data-stu-id="430e5-228">Request</span></span>
<span data-ttu-id="430e5-229">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="430e5-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1276

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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="430e5-230">Antwort</span><span class="sxs-lookup"><span data-stu-id="430e5-230">Response</span></span>
<span data-ttu-id="430e5-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="430e5-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1439

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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



