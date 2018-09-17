# <a name="create-managedandroidlobapp"></a><span data-ttu-id="8a103-101">managedAndroidLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="8a103-101">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="8a103-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8a103-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a103-103">Erstellen eines neuen [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8a103-103">Create a new [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8a103-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8a103-104">Prerequisites</span></span>
<span data-ttu-id="8a103-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8a103-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8a103-107">Permission type</span></span>|<span data-ttu-id="8a103-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8a103-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a103-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8a103-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8a103-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a103-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8a103-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8a103-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a103-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a103-112">Not supported.</span></span>|
|<span data-ttu-id="8a103-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8a103-113">Application</span></span>|<span data-ttu-id="8a103-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a103-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a103-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a103-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8a103-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8a103-116">Request headers</span></span>
|<span data-ttu-id="8a103-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8a103-117">Header</span></span>|<span data-ttu-id="8a103-118">Wert</span><span class="sxs-lookup"><span data-stu-id="8a103-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a103-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8a103-119">Authorization</span></span>|<span data-ttu-id="8a103-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8a103-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a103-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="8a103-121">Accept</span></span>|<span data-ttu-id="8a103-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="8a103-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a103-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8a103-123">Request body</span></span>
<span data-ttu-id="8a103-124">Geben Sie im Anforderungstext eine JSON-Darstellung des managedAndroidLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8a103-124">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="8a103-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedAndroidLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8a103-125">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="8a103-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8a103-126">Property</span></span>|<span data-ttu-id="8a103-127">Typ</span><span class="sxs-lookup"><span data-stu-id="8a103-127">Type</span></span>|<span data-ttu-id="8a103-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a103-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a103-129">ID</span><span class="sxs-lookup"><span data-stu-id="8a103-129">id</span></span>|<span data-ttu-id="8a103-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-130">String</span></span>|<span data-ttu-id="8a103-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8a103-131">Key of the entity.</span></span> <span data-ttu-id="8a103-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8a103-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8a103-133">displayName</span></span>|<span data-ttu-id="8a103-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-134">String</span></span>|<span data-ttu-id="8a103-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="8a103-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8a103-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8a103-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a103-137">description</span></span>|<span data-ttu-id="8a103-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-138">String</span></span>|<span data-ttu-id="8a103-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="8a103-139">The description of the app.</span></span> <span data-ttu-id="8a103-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8a103-141">Verleger</span><span class="sxs-lookup"><span data-stu-id="8a103-141">publisher</span></span>|<span data-ttu-id="8a103-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-142">String</span></span>|<span data-ttu-id="8a103-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="8a103-143">The publisher of the app.</span></span> <span data-ttu-id="8a103-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8a103-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8a103-145">largeIcon</span></span>|[<span data-ttu-id="8a103-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8a103-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="8a103-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="8a103-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8a103-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8a103-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a103-149">createdDateTime</span></span>|<span data-ttu-id="8a103-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a103-150">DateTimeOffset</span></span>|<span data-ttu-id="8a103-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="8a103-151">The date and time the app was created.</span></span> <span data-ttu-id="8a103-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8a103-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a103-153">lastModifiedDateTime</span></span>|<span data-ttu-id="8a103-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a103-154">DateTimeOffset</span></span>|<span data-ttu-id="8a103-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="8a103-155">The date and time the app was last modified.</span></span> <span data-ttu-id="8a103-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8a103-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8a103-157">isFeatured</span></span>|<span data-ttu-id="8a103-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="8a103-158">Boolean</span></span>|<span data-ttu-id="8a103-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8a103-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8a103-160">privacyInformationUrl</span></span>|<span data-ttu-id="8a103-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-161">String</span></span>|<span data-ttu-id="8a103-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="8a103-162">The privacy statement Url.</span></span> <span data-ttu-id="8a103-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8a103-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8a103-164">informationUrl</span></span>|<span data-ttu-id="8a103-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-165">String</span></span>|<span data-ttu-id="8a103-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="8a103-166">The more information Url.</span></span> <span data-ttu-id="8a103-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8a103-168">Besitzer</span><span class="sxs-lookup"><span data-stu-id="8a103-168">owner</span></span>|<span data-ttu-id="8a103-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-169">String</span></span>|<span data-ttu-id="8a103-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="8a103-170">The owner of the app.</span></span> <span data-ttu-id="8a103-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8a103-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="8a103-172">developer</span></span>|<span data-ttu-id="8a103-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-173">String</span></span>|<span data-ttu-id="8a103-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="8a103-174">The developer of the app.</span></span> <span data-ttu-id="8a103-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8a103-176">Notizen</span><span class="sxs-lookup"><span data-stu-id="8a103-176">notes</span></span>|<span data-ttu-id="8a103-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-177">String</span></span>|<span data-ttu-id="8a103-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="8a103-178">Notes for the app.</span></span> <span data-ttu-id="8a103-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8a103-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="8a103-180">publishingState</span></span>|[<span data-ttu-id="8a103-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8a103-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="8a103-p114">Der Veröffentlichungsstand der App. Die App kann nur dann zugewiesen werden, wenn die App veröffentlicht wurde. Vererbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8a103-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8a103-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="8a103-186">appAvailability</span></span>|[<span data-ttu-id="8a103-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="8a103-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="8a103-p115">Verfügbarkeit der Anwendung. Geerbt von [managedApp](../resources/intune_apps_managedapp.md). Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="8a103-p115">The Application's availability. Inherited from [managedApp](../resources/intune_apps_managedapp.md). The possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="8a103-191">Version</span><span class="sxs-lookup"><span data-stu-id="8a103-191">version</span></span>|<span data-ttu-id="8a103-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-192">String</span></span>|<span data-ttu-id="8a103-193">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="8a103-193">The Application's version.</span></span> <span data-ttu-id="8a103-194">Geerbt von [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8a103-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="8a103-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8a103-195">committedContentVersion</span></span>|<span data-ttu-id="8a103-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-196">String</span></span>|<span data-ttu-id="8a103-197">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="8a103-197">The internal committed content version.</span></span> <span data-ttu-id="8a103-198">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8a103-199">fileName</span><span class="sxs-lookup"><span data-stu-id="8a103-199">fileName</span></span>|<span data-ttu-id="8a103-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-200">String</span></span>|<span data-ttu-id="8a103-201">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="8a103-201">The name of the main Lob application file.</span></span> <span data-ttu-id="8a103-202">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8a103-203">Größe</span><span class="sxs-lookup"><span data-stu-id="8a103-203">size</span></span>|<span data-ttu-id="8a103-204">Int64</span><span class="sxs-lookup"><span data-stu-id="8a103-204">Int64</span></span>|<span data-ttu-id="8a103-205">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="8a103-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="8a103-206">Geerbt von [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a103-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8a103-207">packageId</span><span class="sxs-lookup"><span data-stu-id="8a103-207">packageId</span></span>|<span data-ttu-id="8a103-208">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-208">String</span></span>|<span data-ttu-id="8a103-209">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="8a103-209">The package identifier.</span></span>|
|<span data-ttu-id="8a103-210">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8a103-210">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8a103-211">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8a103-211">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="8a103-212">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="8a103-212">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8a103-213">versionName</span><span class="sxs-lookup"><span data-stu-id="8a103-213">versionName</span></span>|<span data-ttu-id="8a103-214">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-214">String</span></span>|<span data-ttu-id="8a103-215">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="8a103-215">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8a103-216">versionCode</span><span class="sxs-lookup"><span data-stu-id="8a103-216">versionCode</span></span>|<span data-ttu-id="8a103-217">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a103-217">String</span></span>|<span data-ttu-id="8a103-218">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="8a103-218">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="8a103-219">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a103-219">Response</span></span>
<span data-ttu-id="8a103-220">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a103-220">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a103-221">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a103-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="8a103-222">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a103-222">Request</span></span>
<span data-ttu-id="8a103-223">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8a103-223">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8a103-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a103-224">Response</span></span>
<span data-ttu-id="8a103-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a103-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








