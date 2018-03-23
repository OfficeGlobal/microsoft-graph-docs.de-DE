# <a name="update-managedioslobapp"></a><span data-ttu-id="a68af-101">managedIOSLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a68af-101">Update managedIOSLobApp</span></span>

> <span data-ttu-id="a68af-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a68af-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a68af-103">Aktualisieren der Eigenschaften eines [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a68af-103">Update the properties of a [calendar](../resources/intune_apps_managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a68af-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a68af-104">Prerequisites</span></span>
<span data-ttu-id="a68af-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a68af-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a68af-107">Permission type</span></span>|<span data-ttu-id="a68af-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a68af-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a68af-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a68af-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a68af-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a68af-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a68af-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a68af-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a68af-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a68af-112">Not supported.</span></span>|
|<span data-ttu-id="a68af-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a68af-113">Application</span></span>|<span data-ttu-id="a68af-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a68af-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a68af-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a68af-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="a68af-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a68af-116">Request headers</span></span>
|<span data-ttu-id="a68af-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a68af-117">Header</span></span>|<span data-ttu-id="a68af-118">Wert</span><span class="sxs-lookup"><span data-stu-id="a68af-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a68af-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a68af-119">Authorization</span></span>|<span data-ttu-id="a68af-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a68af-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a68af-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a68af-121">Accept</span></span>|<span data-ttu-id="a68af-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a68af-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a68af-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a68af-123">Request body</span></span>
<span data-ttu-id="a68af-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a68af-124">In the request body, supply a JSON representation of [Attachment](../resources/intune_apps_managedioslobapp.md) object.</span></span>

<span data-ttu-id="a68af-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a68af-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="a68af-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a68af-126">Property</span></span>|<span data-ttu-id="a68af-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a68af-127">Type</span></span>|<span data-ttu-id="a68af-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a68af-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a68af-129">id</span><span class="sxs-lookup"><span data-stu-id="a68af-129">id</span></span>|<span data-ttu-id="a68af-130">String</span><span class="sxs-lookup"><span data-stu-id="a68af-130">String</span></span>|<span data-ttu-id="a68af-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="a68af-131">Key of the setting.</span></span> <span data-ttu-id="a68af-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a68af-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a68af-133">displayName</span></span>|<span data-ttu-id="a68af-134">String</span><span class="sxs-lookup"><span data-stu-id="a68af-134">String</span></span>|<span data-ttu-id="a68af-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="a68af-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a68af-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a68af-137">description</span><span class="sxs-lookup"><span data-stu-id="a68af-137">description</span></span>|<span data-ttu-id="a68af-138">String</span><span class="sxs-lookup"><span data-stu-id="a68af-138">String</span></span>|<span data-ttu-id="a68af-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="a68af-139">The description of the app.</span></span> <span data-ttu-id="a68af-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a68af-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="a68af-141">Publisher</span></span>|<span data-ttu-id="a68af-142">String</span><span class="sxs-lookup"><span data-stu-id="a68af-142">String</span></span>|<span data-ttu-id="a68af-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="a68af-143">The name of the app.</span></span> <span data-ttu-id="a68af-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a68af-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a68af-145">largeIcon</span></span>|[<span data-ttu-id="a68af-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a68af-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="a68af-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a68af-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a68af-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a68af-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a68af-149">createdDateTime</span></span>|<span data-ttu-id="a68af-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a68af-150">DateTimeOffset</span></span>|<span data-ttu-id="a68af-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="a68af-151">The date and time the group was created.</span></span> <span data-ttu-id="a68af-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a68af-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a68af-153">lastModifiedDateTime</span></span>|<span data-ttu-id="a68af-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a68af-154">DateTimeOffset</span></span>|<span data-ttu-id="a68af-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="a68af-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="a68af-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a68af-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a68af-157">isFeatured</span></span>|<span data-ttu-id="a68af-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="a68af-158">Boolean</span></span>|<span data-ttu-id="a68af-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a68af-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a68af-160">privacyInformationUrl</span></span>|<span data-ttu-id="a68af-161">String</span><span class="sxs-lookup"><span data-stu-id="a68af-161">String</span></span>|<span data-ttu-id="a68af-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="a68af-162">The privacy statement Url.</span></span> <span data-ttu-id="a68af-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a68af-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a68af-164">informationUrl</span></span>|<span data-ttu-id="a68af-165">String</span><span class="sxs-lookup"><span data-stu-id="a68af-165">String</span></span>|<span data-ttu-id="a68af-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="a68af-166">The more information Url.</span></span> <span data-ttu-id="a68af-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a68af-168">owner</span><span class="sxs-lookup"><span data-stu-id="a68af-168">owner</span></span>|<span data-ttu-id="a68af-169">String</span><span class="sxs-lookup"><span data-stu-id="a68af-169">String</span></span>|<span data-ttu-id="a68af-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="a68af-170">The owner of the app.</span></span> <span data-ttu-id="a68af-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a68af-172">developer</span><span class="sxs-lookup"><span data-stu-id="a68af-172">developer</span></span>|<span data-ttu-id="a68af-173">String</span><span class="sxs-lookup"><span data-stu-id="a68af-173">String</span></span>|<span data-ttu-id="a68af-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="a68af-174">The name of the app.</span></span> <span data-ttu-id="a68af-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a68af-176">notes</span><span class="sxs-lookup"><span data-stu-id="a68af-176">notes</span></span>|<span data-ttu-id="a68af-177">String</span><span class="sxs-lookup"><span data-stu-id="a68af-177">String</span></span>|<span data-ttu-id="a68af-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="a68af-178">Notes for the app.</span></span> <span data-ttu-id="a68af-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="a68af-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="a68af-180">publishingState</span></span>|<span data-ttu-id="a68af-181">String</span><span class="sxs-lookup"><span data-stu-id="a68af-181">String</span></span>|<span data-ttu-id="a68af-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="a68af-182">The publishing state for the app.</span></span> <span data-ttu-id="a68af-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="a68af-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a68af-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="a68af-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a68af-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="a68af-185">appAvailability</span></span>|<span data-ttu-id="a68af-186">String</span><span class="sxs-lookup"><span data-stu-id="a68af-186">String</span></span>|<span data-ttu-id="a68af-187">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="a68af-187">The Application's availability.</span></span> <span data-ttu-id="a68af-188">Geerbt von [managedApp](../resources/intune_apps_managedapp.md). Mögliche Werte sind: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="a68af-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="a68af-189">Version</span><span class="sxs-lookup"><span data-stu-id="a68af-189">version</span></span>|<span data-ttu-id="a68af-190">String</span><span class="sxs-lookup"><span data-stu-id="a68af-190">String</span></span>|<span data-ttu-id="a68af-191">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="a68af-191">The Application's version.</span></span> <span data-ttu-id="a68af-192">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="a68af-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="a68af-193">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a68af-193">committedContentVersion</span></span>|<span data-ttu-id="a68af-194">String</span><span class="sxs-lookup"><span data-stu-id="a68af-194">String</span></span>|<span data-ttu-id="a68af-195">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="a68af-195">The internal committed content version.</span></span> <span data-ttu-id="a68af-196">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-196">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a68af-197">fileName</span><span class="sxs-lookup"><span data-stu-id="a68af-197">fileName</span></span>|<span data-ttu-id="a68af-198">String</span><span class="sxs-lookup"><span data-stu-id="a68af-198">String</span></span>|<span data-ttu-id="a68af-199">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="a68af-199">The name of the main Lob application file.</span></span> <span data-ttu-id="a68af-200">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-200">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a68af-201">size</span><span class="sxs-lookup"><span data-stu-id="a68af-201">size</span></span>|<span data-ttu-id="a68af-202">Int64</span><span class="sxs-lookup"><span data-stu-id="a68af-202">Int64</span></span>|<span data-ttu-id="a68af-203">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="a68af-203">The total size, including all uploaded files.</span></span> <span data-ttu-id="a68af-204">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a68af-204">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a68af-205">bundleId</span><span class="sxs-lookup"><span data-stu-id="a68af-205">bundleId</span></span>|<span data-ttu-id="a68af-206">String</span><span class="sxs-lookup"><span data-stu-id="a68af-206">String</span></span>|<span data-ttu-id="a68af-207">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="a68af-207">The Identity Name.</span></span>|
|<span data-ttu-id="a68af-208">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="a68af-208">applicableDeviceType</span></span>|[<span data-ttu-id="a68af-209">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="a68af-209">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="a68af-210">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="a68af-210">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="a68af-211">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a68af-211">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a68af-212">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a68af-212">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="a68af-213">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="a68af-213">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="a68af-214">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a68af-214">expirationDateTime</span></span>|<span data-ttu-id="a68af-215">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a68af-215">DateTimeOffset</span></span>|<span data-ttu-id="a68af-216">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="a68af-216">: The expiration time for the subscription.</span></span>|
|<span data-ttu-id="a68af-217">versionNumber</span><span class="sxs-lookup"><span data-stu-id="a68af-217">versionNumber</span></span>|<span data-ttu-id="a68af-218">String</span><span class="sxs-lookup"><span data-stu-id="a68af-218">String</span></span>|<span data-ttu-id="a68af-219">Die Versionsnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="a68af-219">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a68af-220">buildNumber</span><span class="sxs-lookup"><span data-stu-id="a68af-220">buildNumber</span></span>|<span data-ttu-id="a68af-221">String</span><span class="sxs-lookup"><span data-stu-id="a68af-221">String</span></span>|<span data-ttu-id="a68af-222">Die Buildnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="a68af-222">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="a68af-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="a68af-223">Response</span></span>
<span data-ttu-id="a68af-224">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a68af-224">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a68af-225">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a68af-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="a68af-226">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a68af-226">Request</span></span>
<span data-ttu-id="a68af-227">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a68af-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a68af-228">Antwort</span><span class="sxs-lookup"><span data-stu-id="a68af-228">Response</span></span>
<span data-ttu-id="a68af-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a68af-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



