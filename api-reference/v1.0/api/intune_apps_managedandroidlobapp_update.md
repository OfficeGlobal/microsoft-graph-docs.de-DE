# <a name="update-managedandroidlobapp"></a><span data-ttu-id="bba45-101">managedAndroidLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bba45-101">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="bba45-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bba45-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bba45-103">Aktualisieren der Eigenschaften eines [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bba45-103">Update the properties of a [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bba45-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bba45-104">Prerequisites</span></span>
<span data-ttu-id="bba45-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bba45-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bba45-107">Permission type</span></span>|<span data-ttu-id="bba45-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bba45-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bba45-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bba45-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bba45-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bba45-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bba45-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bba45-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bba45-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bba45-112">Not supported.</span></span>|
|<span data-ttu-id="bba45-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bba45-113">Application</span></span>|<span data-ttu-id="bba45-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bba45-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bba45-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bba45-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="bba45-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bba45-116">Request headers</span></span>
|<span data-ttu-id="bba45-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bba45-117">Header</span></span>|<span data-ttu-id="bba45-118">Wert</span><span class="sxs-lookup"><span data-stu-id="bba45-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bba45-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="bba45-119">Authorization</span></span>|<span data-ttu-id="bba45-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bba45-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bba45-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bba45-121">Accept</span></span>|<span data-ttu-id="bba45-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bba45-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bba45-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bba45-123">Request body</span></span>
<span data-ttu-id="bba45-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bba45-124">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="bba45-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="bba45-125">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).</span></span>

|<span data-ttu-id="bba45-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bba45-126">Property</span></span>|<span data-ttu-id="bba45-127">Typ</span><span class="sxs-lookup"><span data-stu-id="bba45-127">Type</span></span>|<span data-ttu-id="bba45-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bba45-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bba45-129">id</span><span class="sxs-lookup"><span data-stu-id="bba45-129">id</span></span>|<span data-ttu-id="bba45-130">String</span><span class="sxs-lookup"><span data-stu-id="bba45-130">String</span></span>|<span data-ttu-id="bba45-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="bba45-131">Key of the entity.</span></span> <span data-ttu-id="bba45-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bba45-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bba45-133">displayName</span></span>|<span data-ttu-id="bba45-134">String</span><span class="sxs-lookup"><span data-stu-id="bba45-134">String</span></span>|<span data-ttu-id="bba45-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="bba45-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bba45-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bba45-137">description</span><span class="sxs-lookup"><span data-stu-id="bba45-137">description</span></span>|<span data-ttu-id="bba45-138">String</span><span class="sxs-lookup"><span data-stu-id="bba45-138">String</span></span>|<span data-ttu-id="bba45-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="bba45-139">The description of the app.</span></span> <span data-ttu-id="bba45-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bba45-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="bba45-141">publisher</span></span>|<span data-ttu-id="bba45-142">String</span><span class="sxs-lookup"><span data-stu-id="bba45-142">String</span></span>|<span data-ttu-id="bba45-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="bba45-143">The publisher of the app.</span></span> <span data-ttu-id="bba45-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bba45-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bba45-145">largeIcon</span></span>|[<span data-ttu-id="bba45-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bba45-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="bba45-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="bba45-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bba45-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bba45-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bba45-149">createdDateTime</span></span>|<span data-ttu-id="bba45-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bba45-150">DateTimeOffset</span></span>|<span data-ttu-id="bba45-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="bba45-151">The date and time the app was created.</span></span> <span data-ttu-id="bba45-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bba45-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bba45-153">lastModifiedDateTime</span></span>|<span data-ttu-id="bba45-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bba45-154">DateTimeOffset</span></span>|<span data-ttu-id="bba45-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="bba45-155">The date and time the app was last modified.</span></span> <span data-ttu-id="bba45-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bba45-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bba45-157">isFeatured</span></span>|<span data-ttu-id="bba45-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="bba45-158">Boolean</span></span>|<span data-ttu-id="bba45-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bba45-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bba45-160">privacyInformationUrl</span></span>|<span data-ttu-id="bba45-161">String</span><span class="sxs-lookup"><span data-stu-id="bba45-161">String</span></span>|<span data-ttu-id="bba45-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="bba45-162">The privacy statement Url.</span></span> <span data-ttu-id="bba45-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bba45-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bba45-164">informationUrl</span></span>|<span data-ttu-id="bba45-165">String</span><span class="sxs-lookup"><span data-stu-id="bba45-165">String</span></span>|<span data-ttu-id="bba45-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="bba45-166">The more information Url.</span></span> <span data-ttu-id="bba45-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bba45-168">owner</span><span class="sxs-lookup"><span data-stu-id="bba45-168">owner</span></span>|<span data-ttu-id="bba45-169">String</span><span class="sxs-lookup"><span data-stu-id="bba45-169">String</span></span>|<span data-ttu-id="bba45-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="bba45-170">The owner of the app.</span></span> <span data-ttu-id="bba45-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bba45-172">developer</span><span class="sxs-lookup"><span data-stu-id="bba45-172">developer</span></span>|<span data-ttu-id="bba45-173">String</span><span class="sxs-lookup"><span data-stu-id="bba45-173">String</span></span>|<span data-ttu-id="bba45-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="bba45-174">The developer of the app.</span></span> <span data-ttu-id="bba45-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bba45-176">notes</span><span class="sxs-lookup"><span data-stu-id="bba45-176">notes</span></span>|<span data-ttu-id="bba45-177">String</span><span class="sxs-lookup"><span data-stu-id="bba45-177">String</span></span>|<span data-ttu-id="bba45-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="bba45-178">Notes for the app.</span></span> <span data-ttu-id="bba45-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="bba45-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="bba45-180">publishingState</span></span>|[<span data-ttu-id="bba45-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bba45-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="bba45-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="bba45-182">The publishing state for the app.</span></span> <span data-ttu-id="bba45-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="bba45-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bba45-184">Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="bba45-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="bba45-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bba45-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="bba45-186">appAvailability</span></span>|[<span data-ttu-id="bba45-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="bba45-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="bba45-188">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="bba45-188">The Application's availability.</span></span> <span data-ttu-id="bba45-189">Geerbt von [ManagedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md).</span></span> <span data-ttu-id="bba45-190">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="bba45-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="bba45-191">version</span><span class="sxs-lookup"><span data-stu-id="bba45-191">version</span></span>|<span data-ttu-id="bba45-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bba45-192">String</span></span>|<span data-ttu-id="bba45-193">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="bba45-193">The Application's version.</span></span> <span data-ttu-id="bba45-194">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="bba45-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="bba45-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="bba45-195">committedContentVersion</span></span>|<span data-ttu-id="bba45-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bba45-196">String</span></span>|<span data-ttu-id="bba45-197">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="bba45-197">The internal committed content version.</span></span> <span data-ttu-id="bba45-198">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bba45-199">fileName</span><span class="sxs-lookup"><span data-stu-id="bba45-199">fileName</span></span>|<span data-ttu-id="bba45-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bba45-200">String</span></span>|<span data-ttu-id="bba45-201">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="bba45-201">The name of the main Lob application file.</span></span> <span data-ttu-id="bba45-202">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bba45-203">size</span><span class="sxs-lookup"><span data-stu-id="bba45-203">size</span></span>|<span data-ttu-id="bba45-204">Int64</span><span class="sxs-lookup"><span data-stu-id="bba45-204">Int64</span></span>|<span data-ttu-id="bba45-205">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="bba45-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="bba45-206">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bba45-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bba45-207">packageId</span><span class="sxs-lookup"><span data-stu-id="bba45-207">packageId</span></span>|<span data-ttu-id="bba45-208">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bba45-208">String</span></span>|<span data-ttu-id="bba45-209">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="bba45-209">The package identifier.</span></span>|
|<span data-ttu-id="bba45-210">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bba45-210">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="bba45-211">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bba45-211">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="bba45-212">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="bba45-212">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="bba45-213">versionName</span><span class="sxs-lookup"><span data-stu-id="bba45-213">versionName</span></span>|<span data-ttu-id="bba45-214">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bba45-214">String</span></span>|<span data-ttu-id="bba45-215">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="bba45-215">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="bba45-216">versionCode</span><span class="sxs-lookup"><span data-stu-id="bba45-216">versionCode</span></span>|<span data-ttu-id="bba45-217">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bba45-217">String</span></span>|<span data-ttu-id="bba45-218">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="bba45-218">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="bba45-219">Antwort</span><span class="sxs-lookup"><span data-stu-id="bba45-219">Response</span></span>
<span data-ttu-id="bba45-220">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bba45-220">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bba45-221">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bba45-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="bba45-222">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bba45-222">Request</span></span>
<span data-ttu-id="bba45-223">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bba45-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1153

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="bba45-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="bba45-224">Response</span></span>
<span data-ttu-id="bba45-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bba45-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1325

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



