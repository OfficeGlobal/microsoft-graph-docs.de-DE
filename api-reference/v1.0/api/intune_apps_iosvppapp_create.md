# <a name="create-iosvppapp"></a><span data-ttu-id="6f921-101">Erstellen von „iosVppApp“</span><span class="sxs-lookup"><span data-stu-id="6f921-101">Create iosVppApp</span></span>

> <span data-ttu-id="6f921-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6f921-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f921-103">Erstellen eines neuen [iosVppApp](../resources/intune_apps_iosvppapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6f921-103">Create a new [plannerBucket](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f921-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6f921-104">Prerequisites</span></span>
<span data-ttu-id="6f921-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6f921-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f921-107">Permission type</span></span>|<span data-ttu-id="6f921-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f921-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f921-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f921-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6f921-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f921-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6f921-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f921-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f921-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f921-112">Not supported.</span></span>|
|<span data-ttu-id="6f921-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f921-113">Application</span></span>|<span data-ttu-id="6f921-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f921-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f921-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f921-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6f921-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f921-116">Request headers</span></span>
|<span data-ttu-id="6f921-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6f921-117">Header</span></span>|<span data-ttu-id="6f921-118">Wert</span><span class="sxs-lookup"><span data-stu-id="6f921-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f921-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f921-119">Authorization</span></span>|<span data-ttu-id="6f921-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6f921-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6f921-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6f921-121">Accept</span></span>|<span data-ttu-id="6f921-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6f921-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f921-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f921-123">Request body</span></span>
<span data-ttu-id="6f921-124">Geben Sie im Anforderungstext eine JSON-Darstellung des iosVppApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="6f921-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="6f921-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosVppApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6f921-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="6f921-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f921-126">Property</span></span>|<span data-ttu-id="6f921-127">Typ</span><span class="sxs-lookup"><span data-stu-id="6f921-127">Type</span></span>|<span data-ttu-id="6f921-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f921-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f921-129">id</span><span class="sxs-lookup"><span data-stu-id="6f921-129">id</span></span>|<span data-ttu-id="6f921-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-130">String</span></span>|<span data-ttu-id="6f921-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="6f921-131">Key of the setting.</span></span> <span data-ttu-id="6f921-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f921-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6f921-133">displayName</span></span>|<span data-ttu-id="6f921-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-134">String</span></span>|<span data-ttu-id="6f921-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="6f921-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6f921-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f921-137">description</span><span class="sxs-lookup"><span data-stu-id="6f921-137">description</span></span>|<span data-ttu-id="6f921-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-138">String</span></span>|<span data-ttu-id="6f921-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="6f921-139">The description of the app.</span></span> <span data-ttu-id="6f921-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f921-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="6f921-141">Publisher</span></span>|<span data-ttu-id="6f921-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-142">String</span></span>|<span data-ttu-id="6f921-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="6f921-143">The name of the app.</span></span> <span data-ttu-id="6f921-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f921-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6f921-145">largeIcon</span></span>|[<span data-ttu-id="6f921-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6f921-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="6f921-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="6f921-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6f921-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f921-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f921-149">createdDateTime</span></span>|<span data-ttu-id="6f921-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f921-150">DateTimeOffset</span></span>|<span data-ttu-id="6f921-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="6f921-151">The date and time the group was created.</span></span> <span data-ttu-id="6f921-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f921-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f921-153">lastModifiedDateTime</span></span>|<span data-ttu-id="6f921-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f921-154">DateTimeOffset</span></span>|<span data-ttu-id="6f921-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="6f921-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="6f921-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f921-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6f921-157">isFeatured</span></span>|<span data-ttu-id="6f921-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6f921-158">Boolean</span></span>|<span data-ttu-id="6f921-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f921-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6f921-160">privacyInformationUrl</span></span>|<span data-ttu-id="6f921-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-161">String</span></span>|<span data-ttu-id="6f921-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="6f921-162">The privacy statement Url.</span></span> <span data-ttu-id="6f921-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f921-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6f921-164">informationUrl</span></span>|<span data-ttu-id="6f921-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-165">String</span></span>|<span data-ttu-id="6f921-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="6f921-166">The more information Url.</span></span> <span data-ttu-id="6f921-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f921-168">owner</span><span class="sxs-lookup"><span data-stu-id="6f921-168">owner</span></span>|<span data-ttu-id="6f921-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-169">String</span></span>|<span data-ttu-id="6f921-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="6f921-170">The owner of the app.</span></span> <span data-ttu-id="6f921-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f921-172">developer</span><span class="sxs-lookup"><span data-stu-id="6f921-172">developer</span></span>|<span data-ttu-id="6f921-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-173">String</span></span>|<span data-ttu-id="6f921-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="6f921-174">The name of the app.</span></span> <span data-ttu-id="6f921-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f921-176">notes</span><span class="sxs-lookup"><span data-stu-id="6f921-176">notes</span></span>|<span data-ttu-id="6f921-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-177">String</span></span>|<span data-ttu-id="6f921-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="6f921-178">Notes for the app.</span></span> <span data-ttu-id="6f921-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6f921-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6f921-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="6f921-180">publishingState</span></span>|<span data-ttu-id="6f921-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-181">String</span></span>|<span data-ttu-id="6f921-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="6f921-182">The publishing state for the app.</span></span> <span data-ttu-id="6f921-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="6f921-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6f921-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6f921-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6f921-185">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6f921-185">usedLicenseCount</span></span>|<span data-ttu-id="6f921-186">Int32</span><span class="sxs-lookup"><span data-stu-id="6f921-186">Int32</span></span>|<span data-ttu-id="6f921-187">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="6f921-187">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="6f921-188">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6f921-188">totalLicenseCount</span></span>|<span data-ttu-id="6f921-189">Int32</span><span class="sxs-lookup"><span data-stu-id="6f921-189">Int32</span></span>|<span data-ttu-id="6f921-190">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="6f921-190">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="6f921-191">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="6f921-191">releaseDateTime</span></span>|<span data-ttu-id="6f921-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f921-192">DateTimeOffset</span></span>|<span data-ttu-id="6f921-193">Datum und Uhrzeit der Veröffentlichung der VPP-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="6f921-193">The VPP application release date and time.</span></span>|
|<span data-ttu-id="6f921-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6f921-194">appStoreUrl</span></span>|<span data-ttu-id="6f921-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-195">String</span></span>|<span data-ttu-id="6f921-196">Store-URL</span><span class="sxs-lookup"><span data-stu-id="6f921-196">The store URL.</span></span>|
|<span data-ttu-id="6f921-197">licensingType</span><span class="sxs-lookup"><span data-stu-id="6f921-197">licensingType</span></span>|[<span data-ttu-id="6f921-198">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="6f921-198">vppLicensingType</span></span>](../resources/intune_apps_vpplicensingtype.md)|<span data-ttu-id="6f921-199">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="6f921-199">The supported License Type.</span></span>|
|<span data-ttu-id="6f921-200">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="6f921-200">applicableDeviceType</span></span>|[<span data-ttu-id="6f921-201">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="6f921-201">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="6f921-202">Gültiger iOS-Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="6f921-202">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="6f921-203">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="6f921-203">vppTokenOrganizationName</span></span>|<span data-ttu-id="6f921-204">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-204">String</span></span>|<span data-ttu-id="6f921-205">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="6f921-205">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="6f921-206">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="6f921-206">vppTokenAccountType</span></span>|<span data-ttu-id="6f921-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-207">String</span></span>|<span data-ttu-id="6f921-208">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="6f921-208">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="6f921-209">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="6f921-209">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="6f921-210">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="6f921-210">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="6f921-211">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="6f921-211">vppTokenAppleId</span></span>|<span data-ttu-id="6f921-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-212">String</span></span>|<span data-ttu-id="6f921-213">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="6f921-213">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="6f921-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="6f921-214">bundleId</span></span>|<span data-ttu-id="6f921-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6f921-215">String</span></span>|<span data-ttu-id="6f921-216">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="6f921-216">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="6f921-217">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f921-217">Response</span></span>
<span data-ttu-id="6f921-218">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosVppApp](../resources/intune_apps_iosvppapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f921-218">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f921-219">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f921-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f921-220">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f921-220">Request</span></span>
<span data-ttu-id="6f921-221">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f921-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1286

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="6f921-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f921-222">Response</span></span>
<span data-ttu-id="6f921-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f921-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1394

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```



