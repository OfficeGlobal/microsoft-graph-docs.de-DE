# <a name="update-androidlobapp"></a><span data-ttu-id="b4ad0-101">AndroidLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b4ad0-101">Update androidLobApp</span></span>

> <span data-ttu-id="b4ad0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4ad0-103">Aktualisieren der Eigenschaften eines [androidLobApp](../resources/intune_apps_androidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-103">Update the properties of a [androidLobApp](../resources/intune_apps_androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4ad0-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b4ad0-104">Prerequisites</span></span>
<span data-ttu-id="b4ad0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b4ad0-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4ad0-107">Permission type</span></span>|<span data-ttu-id="b4ad0-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4ad0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4ad0-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4ad0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b4ad0-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4ad0-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4ad0-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4ad0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4ad0-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4ad0-112">Not supported.</span></span>|
|<span data-ttu-id="b4ad0-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4ad0-113">Application</span></span>|<span data-ttu-id="b4ad0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4ad0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4ad0-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4ad0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b4ad0-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4ad0-116">Request headers</span></span>
|<span data-ttu-id="b4ad0-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b4ad0-117">Header</span></span>|<span data-ttu-id="b4ad0-118">Wert</span><span class="sxs-lookup"><span data-stu-id="b4ad0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4ad0-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b4ad0-119">Authorization</span></span>|<span data-ttu-id="b4ad0-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b4ad0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4ad0-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="b4ad0-121">Accept</span></span>|<span data-ttu-id="b4ad0-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="b4ad0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4ad0-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4ad0-123">Request body</span></span>
<span data-ttu-id="b4ad0-124">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidLobApp](../resources/intune_apps_androidlobapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-124">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune_apps_androidlobapp.md) object.</span></span>

<span data-ttu-id="b4ad0-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidLobApp](../resources/intune_apps_androidlobapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-125">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune_apps_androidlobapp.md).</span></span>

|<span data-ttu-id="b4ad0-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4ad0-126">Property</span></span>|<span data-ttu-id="b4ad0-127">Typ</span><span class="sxs-lookup"><span data-stu-id="b4ad0-127">Type</span></span>|<span data-ttu-id="b4ad0-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4ad0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4ad0-129">id</span><span class="sxs-lookup"><span data-stu-id="b4ad0-129">id</span></span>|<span data-ttu-id="b4ad0-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-130">String</span></span>|<span data-ttu-id="b4ad0-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b4ad0-131">Key of the entity.</span></span> <span data-ttu-id="b4ad0-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4ad0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b4ad0-133">displayName</span></span>|<span data-ttu-id="b4ad0-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-134">String</span></span>|<span data-ttu-id="b4ad0-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b4ad0-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4ad0-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4ad0-137">description</span></span>|<span data-ttu-id="b4ad0-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-138">String</span></span>|<span data-ttu-id="b4ad0-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-139">The description of the app.</span></span> <span data-ttu-id="b4ad0-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4ad0-141">Verleger</span><span class="sxs-lookup"><span data-stu-id="b4ad0-141">publisher</span></span>|<span data-ttu-id="b4ad0-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-142">String</span></span>|<span data-ttu-id="b4ad0-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-143">The publisher of the app.</span></span> <span data-ttu-id="b4ad0-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4ad0-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b4ad0-145">largeIcon</span></span>|[<span data-ttu-id="b4ad0-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b4ad0-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="b4ad0-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b4ad0-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4ad0-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4ad0-149">createdDateTime</span></span>|<span data-ttu-id="b4ad0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4ad0-150">DateTimeOffset</span></span>|<span data-ttu-id="b4ad0-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-151">The date and time the app was created.</span></span> <span data-ttu-id="b4ad0-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4ad0-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4ad0-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b4ad0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4ad0-154">DateTimeOffset</span></span>|<span data-ttu-id="b4ad0-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-155">The date and time the app was last modified.</span></span> <span data-ttu-id="b4ad0-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4ad0-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b4ad0-157">isFeatured</span></span>|<span data-ttu-id="b4ad0-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b4ad0-158">Boolean</span></span>|<span data-ttu-id="b4ad0-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4ad0-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b4ad0-160">privacyInformationUrl</span></span>|<span data-ttu-id="b4ad0-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-161">String</span></span>|<span data-ttu-id="b4ad0-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-162">The privacy statement Url.</span></span> <span data-ttu-id="b4ad0-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4ad0-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b4ad0-164">informationUrl</span></span>|<span data-ttu-id="b4ad0-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-165">String</span></span>|<span data-ttu-id="b4ad0-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-166">The more information Url.</span></span> <span data-ttu-id="b4ad0-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4ad0-168">Besitzer</span><span class="sxs-lookup"><span data-stu-id="b4ad0-168">owner</span></span>|<span data-ttu-id="b4ad0-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-169">String</span></span>|<span data-ttu-id="b4ad0-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-170">The owner of the app.</span></span> <span data-ttu-id="b4ad0-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4ad0-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="b4ad0-172">developer</span></span>|<span data-ttu-id="b4ad0-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-173">String</span></span>|<span data-ttu-id="b4ad0-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-174">The developer of the app.</span></span> <span data-ttu-id="b4ad0-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4ad0-176">Notizen</span><span class="sxs-lookup"><span data-stu-id="b4ad0-176">notes</span></span>|<span data-ttu-id="b4ad0-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-177">String</span></span>|<span data-ttu-id="b4ad0-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-178">Notes for the app.</span></span> <span data-ttu-id="b4ad0-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b4ad0-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="b4ad0-180">publishingState</span></span>|[<span data-ttu-id="b4ad0-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b4ad0-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="b4ad0-182">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-182">The publishing state for the app.</span></span> <span data-ttu-id="b4ad0-183">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b4ad0-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="b4ad0-185">Mögliche Werte sind `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="b4ad0-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b4ad0-186">committedContentVersion</span></span>|<span data-ttu-id="b4ad0-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-187">String</span></span>|<span data-ttu-id="b4ad0-188">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-188">The internal committed content version.</span></span> <span data-ttu-id="b4ad0-189">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="b4ad0-190">fileName</span><span class="sxs-lookup"><span data-stu-id="b4ad0-190">fileName</span></span>|<span data-ttu-id="b4ad0-191">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-191">String</span></span>|<span data-ttu-id="b4ad0-192">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-192">The name of the main Lob application file.</span></span> <span data-ttu-id="b4ad0-193">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="b4ad0-194">Größe</span><span class="sxs-lookup"><span data-stu-id="b4ad0-194">size</span></span>|<span data-ttu-id="b4ad0-195">Int64</span><span class="sxs-lookup"><span data-stu-id="b4ad0-195">Int64</span></span>|<span data-ttu-id="b4ad0-196">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="b4ad0-197">Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4ad0-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="b4ad0-198">packageId</span><span class="sxs-lookup"><span data-stu-id="b4ad0-198">packageId</span></span>|<span data-ttu-id="b4ad0-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-199">String</span></span>|<span data-ttu-id="b4ad0-200">Der Paketbezeichner.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-200">The package identifier.</span></span>|
|<span data-ttu-id="b4ad0-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b4ad0-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b4ad0-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b4ad0-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="b4ad0-203">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-203">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b4ad0-204">versionName</span><span class="sxs-lookup"><span data-stu-id="b4ad0-204">versionName</span></span>|<span data-ttu-id="b4ad0-205">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-205">String</span></span>|<span data-ttu-id="b4ad0-206">Der Versionsname der branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-206">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b4ad0-207">versionCode</span><span class="sxs-lookup"><span data-stu-id="b4ad0-207">versionCode</span></span>|<span data-ttu-id="b4ad0-208">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4ad0-208">String</span></span>|<span data-ttu-id="b4ad0-209">Der Versionscode der branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-209">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="b4ad0-210">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4ad0-210">Response</span></span>
<span data-ttu-id="b4ad0-211">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [androidLobApp](../resources/intune_apps_androidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-211">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune_apps_androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4ad0-212">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4ad0-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4ad0-213">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4ad0-213">Request</span></span>
<span data-ttu-id="b4ad0-214">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1087

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

### <a name="response"></a><span data-ttu-id="b4ad0-215">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4ad0-215">Response</span></span>
<span data-ttu-id="b4ad0-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4ad0-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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



