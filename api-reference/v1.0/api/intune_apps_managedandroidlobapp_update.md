# <a name="update-managedandroidlobapp"></a><span data-ttu-id="5d86a-101">managedAndroidLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5d86a-101">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="5d86a-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5d86a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d86a-103">Aktualisieren der Eigenschaften eines [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5d86a-103">Update the properties of a [calendar](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5d86a-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5d86a-104">Prerequisites</span></span>
<span data-ttu-id="5d86a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5d86a-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d86a-107">Permission type</span></span>|<span data-ttu-id="5d86a-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d86a-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d86a-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d86a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5d86a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d86a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5d86a-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d86a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d86a-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d86a-112">Not supported.</span></span>|
|<span data-ttu-id="5d86a-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d86a-113">Application</span></span>|<span data-ttu-id="5d86a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d86a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d86a-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d86a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="5d86a-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d86a-116">Request headers</span></span>
|<span data-ttu-id="5d86a-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5d86a-117">Header</span></span>|<span data-ttu-id="5d86a-118">Wert</span><span class="sxs-lookup"><span data-stu-id="5d86a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d86a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d86a-119">Authorization</span></span>|<span data-ttu-id="5d86a-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5d86a-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5d86a-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5d86a-121">Accept</span></span>|<span data-ttu-id="5d86a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5d86a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d86a-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5d86a-123">Request body</span></span>
<span data-ttu-id="5d86a-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5d86a-124">In the request body, supply a JSON representation of [message](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="5d86a-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="5d86a-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="5d86a-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d86a-126">Property</span></span>|<span data-ttu-id="5d86a-127">Typ</span><span class="sxs-lookup"><span data-stu-id="5d86a-127">Type</span></span>|<span data-ttu-id="5d86a-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d86a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d86a-129">id</span><span class="sxs-lookup"><span data-stu-id="5d86a-129">id</span></span>|<span data-ttu-id="5d86a-130">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-130">String</span></span>|<span data-ttu-id="5d86a-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="5d86a-131">Key of the setting.</span></span> <span data-ttu-id="5d86a-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5d86a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5d86a-133">displayName</span></span>|<span data-ttu-id="5d86a-134">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-134">String</span></span>|<span data-ttu-id="5d86a-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="5d86a-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5d86a-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5d86a-137">description</span><span class="sxs-lookup"><span data-stu-id="5d86a-137">description</span></span>|<span data-ttu-id="5d86a-138">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-138">String</span></span>|<span data-ttu-id="5d86a-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="5d86a-139">The description of the app.</span></span> <span data-ttu-id="5d86a-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5d86a-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="5d86a-141">Publisher</span></span>|<span data-ttu-id="5d86a-142">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-142">String</span></span>|<span data-ttu-id="5d86a-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="5d86a-143">The name of the app.</span></span> <span data-ttu-id="5d86a-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5d86a-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5d86a-145">largeIcon</span></span>|[<span data-ttu-id="5d86a-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5d86a-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="5d86a-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5d86a-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5d86a-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5d86a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d86a-149">createdDateTime</span></span>|<span data-ttu-id="5d86a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d86a-150">DateTimeOffset</span></span>|<span data-ttu-id="5d86a-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="5d86a-151">The date and time the group was created.</span></span> <span data-ttu-id="5d86a-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5d86a-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d86a-153">lastModifiedDateTime</span></span>|<span data-ttu-id="5d86a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d86a-154">DateTimeOffset</span></span>|<span data-ttu-id="5d86a-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="5d86a-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="5d86a-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5d86a-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5d86a-157">isFeatured</span></span>|<span data-ttu-id="5d86a-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d86a-158">Boolean</span></span>|<span data-ttu-id="5d86a-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5d86a-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5d86a-160">privacyInformationUrl</span></span>|<span data-ttu-id="5d86a-161">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-161">String</span></span>|<span data-ttu-id="5d86a-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="5d86a-162">The privacy statement Url.</span></span> <span data-ttu-id="5d86a-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5d86a-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5d86a-164">informationUrl</span></span>|<span data-ttu-id="5d86a-165">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-165">String</span></span>|<span data-ttu-id="5d86a-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="5d86a-166">The more information Url.</span></span> <span data-ttu-id="5d86a-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5d86a-168">owner</span><span class="sxs-lookup"><span data-stu-id="5d86a-168">owner</span></span>|<span data-ttu-id="5d86a-169">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-169">String</span></span>|<span data-ttu-id="5d86a-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="5d86a-170">The owner of the app.</span></span> <span data-ttu-id="5d86a-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5d86a-172">developer</span><span class="sxs-lookup"><span data-stu-id="5d86a-172">developer</span></span>|<span data-ttu-id="5d86a-173">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-173">String</span></span>|<span data-ttu-id="5d86a-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="5d86a-174">The name of the app.</span></span> <span data-ttu-id="5d86a-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5d86a-176">notes</span><span class="sxs-lookup"><span data-stu-id="5d86a-176">notes</span></span>|<span data-ttu-id="5d86a-177">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-177">String</span></span>|<span data-ttu-id="5d86a-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="5d86a-178">Notes for the app.</span></span> <span data-ttu-id="5d86a-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="5d86a-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="5d86a-180">publishingState</span></span>|<span data-ttu-id="5d86a-181">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-181">String</span></span>|<span data-ttu-id="5d86a-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="5d86a-182">The publishing state for the app.</span></span> <span data-ttu-id="5d86a-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="5d86a-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5d86a-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="5d86a-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5d86a-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="5d86a-185">appAvailability</span></span>|<span data-ttu-id="5d86a-186">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-186">String</span></span>|<span data-ttu-id="5d86a-187">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="5d86a-187">The Application's availability.</span></span> <span data-ttu-id="5d86a-188">Geerbt von [managedApp](../resources/intune_apps_managedapp.md). Mögliche Werte sind: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="5d86a-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="5d86a-189">Version</span><span class="sxs-lookup"><span data-stu-id="5d86a-189">version</span></span>|<span data-ttu-id="5d86a-190">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-190">String</span></span>|<span data-ttu-id="5d86a-191">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="5d86a-191">The Application's version.</span></span> <span data-ttu-id="5d86a-192">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="5d86a-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="5d86a-193">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="5d86a-193">committedContentVersion</span></span>|<span data-ttu-id="5d86a-194">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-194">String</span></span>|<span data-ttu-id="5d86a-195">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="5d86a-195">The internal committed content version.</span></span> <span data-ttu-id="5d86a-196">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-196">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="5d86a-197">fileName</span><span class="sxs-lookup"><span data-stu-id="5d86a-197">fileName</span></span>|<span data-ttu-id="5d86a-198">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-198">String</span></span>|<span data-ttu-id="5d86a-199">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="5d86a-199">The name of the main Lob application file.</span></span> <span data-ttu-id="5d86a-200">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-200">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="5d86a-201">size</span><span class="sxs-lookup"><span data-stu-id="5d86a-201">size</span></span>|<span data-ttu-id="5d86a-202">Int64</span><span class="sxs-lookup"><span data-stu-id="5d86a-202">Int64</span></span>|<span data-ttu-id="5d86a-203">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="5d86a-203">The total size, including all uploaded files.</span></span> <span data-ttu-id="5d86a-204">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d86a-204">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="5d86a-205">packageId</span><span class="sxs-lookup"><span data-stu-id="5d86a-205">packageId</span></span>|<span data-ttu-id="5d86a-206">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-206">String</span></span>|<span data-ttu-id="5d86a-207">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="5d86a-207">The package identifier.</span></span>|
|<span data-ttu-id="5d86a-208">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5d86a-208">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5d86a-209">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5d86a-209">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="5d86a-210">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="5d86a-210">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="5d86a-211">versionName</span><span class="sxs-lookup"><span data-stu-id="5d86a-211">versionName</span></span>|<span data-ttu-id="5d86a-212">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-212">String</span></span>|<span data-ttu-id="5d86a-213">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="5d86a-213">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5d86a-214">versionCode</span><span class="sxs-lookup"><span data-stu-id="5d86a-214">versionCode</span></span>|<span data-ttu-id="5d86a-215">String</span><span class="sxs-lookup"><span data-stu-id="5d86a-215">String</span></span>|<span data-ttu-id="5d86a-216">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="5d86a-216">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="5d86a-217">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d86a-217">Response</span></span>
<span data-ttu-id="5d86a-218">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d86a-218">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d86a-219">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d86a-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="5d86a-220">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d86a-220">Request</span></span>
<span data-ttu-id="5d86a-221">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d86a-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1158

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

### <a name="response"></a><span data-ttu-id="5d86a-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d86a-222">Response</span></span>
<span data-ttu-id="5d86a-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d86a-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



