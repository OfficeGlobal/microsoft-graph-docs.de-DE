# <a name="create-managedandroidlobapp"></a><span data-ttu-id="1a1b2-101">managedAndroidLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="1a1b2-101">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="1a1b2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a1b2-103">Erstellen eines neuen [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-103">Create a new [plannerBucket](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a1b2-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1a1b2-104">Prerequisites</span></span>
<span data-ttu-id="1a1b2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1a1b2-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1a1b2-107">Permission type</span></span>|<span data-ttu-id="1a1b2-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1a1b2-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a1b2-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1a1b2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1a1b2-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a1b2-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1a1b2-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1a1b2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a1b2-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a1b2-112">Not supported.</span></span>|
|<span data-ttu-id="1a1b2-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1a1b2-113">Application</span></span>|<span data-ttu-id="1a1b2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a1b2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a1b2-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a1b2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1a1b2-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a1b2-116">Request headers</span></span>
|<span data-ttu-id="1a1b2-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1a1b2-117">Header</span></span>|<span data-ttu-id="1a1b2-118">Wert</span><span class="sxs-lookup"><span data-stu-id="1a1b2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a1b2-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1a1b2-119">Authorization</span></span>|<span data-ttu-id="1a1b2-120">Bearer&lt;token&gt; erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1a1b2-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1a1b2-121">Accept</span></span>|<span data-ttu-id="1a1b2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1a1b2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a1b2-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a1b2-123">Request body</span></span>
<span data-ttu-id="1a1b2-124">Geben Sie im Anforderungstext eine JSON-Darstellung des managedAndroidLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="1a1b2-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedAndroidLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="1a1b2-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1a1b2-126">Property</span></span>|<span data-ttu-id="1a1b2-127">Typ</span><span class="sxs-lookup"><span data-stu-id="1a1b2-127">Type</span></span>|<span data-ttu-id="1a1b2-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a1b2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a1b2-129">id</span><span class="sxs-lookup"><span data-stu-id="1a1b2-129">id</span></span>|<span data-ttu-id="1a1b2-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-130">String</span></span>|<span data-ttu-id="1a1b2-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-131">Key of the setting.</span></span> <span data-ttu-id="1a1b2-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1a1b2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1a1b2-133">displayName</span></span>|<span data-ttu-id="1a1b2-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-134">String</span></span>|<span data-ttu-id="1a1b2-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1a1b2-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1a1b2-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a1b2-137">description</span></span>|<span data-ttu-id="1a1b2-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-138">String</span></span>|<span data-ttu-id="1a1b2-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-139">The description of the app.</span></span> <span data-ttu-id="1a1b2-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1a1b2-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="1a1b2-141">Publisher</span></span>|<span data-ttu-id="1a1b2-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-142">String</span></span>|<span data-ttu-id="1a1b2-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-143">The name of the app.</span></span> <span data-ttu-id="1a1b2-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1a1b2-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1a1b2-145">largeIcon</span></span>|[<span data-ttu-id="1a1b2-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1a1b2-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="1a1b2-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1a1b2-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1a1b2-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a1b2-149">createdDateTime</span></span>|<span data-ttu-id="1a1b2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a1b2-150">DateTimeOffset</span></span>|<span data-ttu-id="1a1b2-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-151">The date and time the group was created.</span></span> <span data-ttu-id="1a1b2-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1a1b2-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a1b2-153">lastModifiedDateTime</span></span>|<span data-ttu-id="1a1b2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a1b2-154">DateTimeOffset</span></span>|<span data-ttu-id="1a1b2-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="1a1b2-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1a1b2-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1a1b2-157">isFeatured</span></span>|<span data-ttu-id="1a1b2-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a1b2-158">Boolean</span></span>|<span data-ttu-id="1a1b2-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1a1b2-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1a1b2-160">privacyInformationUrl</span></span>|<span data-ttu-id="1a1b2-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-161">String</span></span>|<span data-ttu-id="1a1b2-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-162">The privacy statement Url.</span></span> <span data-ttu-id="1a1b2-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1a1b2-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1a1b2-164">informationUrl</span></span>|<span data-ttu-id="1a1b2-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-165">String</span></span>|<span data-ttu-id="1a1b2-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-166">The more information Url.</span></span> <span data-ttu-id="1a1b2-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1a1b2-168">owner</span><span class="sxs-lookup"><span data-stu-id="1a1b2-168">owner</span></span>|<span data-ttu-id="1a1b2-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-169">String</span></span>|<span data-ttu-id="1a1b2-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-170">The owner of the app.</span></span> <span data-ttu-id="1a1b2-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1a1b2-172">developer</span><span class="sxs-lookup"><span data-stu-id="1a1b2-172">developer</span></span>|<span data-ttu-id="1a1b2-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-173">String</span></span>|<span data-ttu-id="1a1b2-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-174">The name of the app.</span></span> <span data-ttu-id="1a1b2-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1a1b2-176">notes</span><span class="sxs-lookup"><span data-stu-id="1a1b2-176">notes</span></span>|<span data-ttu-id="1a1b2-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-177">String</span></span>|<span data-ttu-id="1a1b2-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-178">Notes for the app.</span></span> <span data-ttu-id="1a1b2-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1a1b2-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="1a1b2-180">publishingState</span></span>|<span data-ttu-id="1a1b2-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-181">String</span></span>|<span data-ttu-id="1a1b2-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-182">The publishing state for the app.</span></span> <span data-ttu-id="1a1b2-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1a1b2-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1a1b2-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="1a1b2-185">appAvailability</span></span>|<span data-ttu-id="1a1b2-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-186">String</span></span>|<span data-ttu-id="1a1b2-187">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-187">The Application's availability.</span></span> <span data-ttu-id="1a1b2-188">Geerbt von [managedApp](../resources/intune_apps_managedapp.md). Mögliche Werte sind: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="1a1b2-189">Version</span><span class="sxs-lookup"><span data-stu-id="1a1b2-189">version</span></span>|<span data-ttu-id="1a1b2-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-190">String</span></span>|<span data-ttu-id="1a1b2-191">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-191">The Application's version.</span></span> <span data-ttu-id="1a1b2-192">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="1a1b2-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="1a1b2-193">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1a1b2-193">committedContentVersion</span></span>|<span data-ttu-id="1a1b2-194">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-194">String</span></span>|<span data-ttu-id="1a1b2-195">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-195">The internal committed content version.</span></span> <span data-ttu-id="1a1b2-196">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-196">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1a1b2-197">fileName</span><span class="sxs-lookup"><span data-stu-id="1a1b2-197">fileName</span></span>|<span data-ttu-id="1a1b2-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-198">String</span></span>|<span data-ttu-id="1a1b2-199">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-199">The name of the main Lob application file.</span></span> <span data-ttu-id="1a1b2-200">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-200">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1a1b2-201">size</span><span class="sxs-lookup"><span data-stu-id="1a1b2-201">size</span></span>|<span data-ttu-id="1a1b2-202">Int64</span><span class="sxs-lookup"><span data-stu-id="1a1b2-202">Int64</span></span>|<span data-ttu-id="1a1b2-203">Gesamtgröße, einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-203">The total size, including all uploaded files.</span></span> <span data-ttu-id="1a1b2-204">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a1b2-204">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1a1b2-205">packageId</span><span class="sxs-lookup"><span data-stu-id="1a1b2-205">packageId</span></span>|<span data-ttu-id="1a1b2-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-206">String</span></span>|<span data-ttu-id="1a1b2-207">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-207">The package identifier.</span></span>|
|<span data-ttu-id="1a1b2-208">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1a1b2-208">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1a1b2-209">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1a1b2-209">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="1a1b2-210">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-210">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1a1b2-211">versionName</span><span class="sxs-lookup"><span data-stu-id="1a1b2-211">versionName</span></span>|<span data-ttu-id="1a1b2-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-212">String</span></span>|<span data-ttu-id="1a1b2-213">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-213">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1a1b2-214">versionCode</span><span class="sxs-lookup"><span data-stu-id="1a1b2-214">versionCode</span></span>|<span data-ttu-id="1a1b2-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a1b2-215">String</span></span>|<span data-ttu-id="1a1b2-216">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-216">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="1a1b2-217">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a1b2-217">Response</span></span>
<span data-ttu-id="1a1b2-218">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-218">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_apps_managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a1b2-219">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1a1b2-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a1b2-220">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a1b2-220">Request</span></span>
<span data-ttu-id="1a1b2-221">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1217

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

### <a name="response"></a><span data-ttu-id="1a1b2-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a1b2-222">Response</span></span>
<span data-ttu-id="1a1b2-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a1b2-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



