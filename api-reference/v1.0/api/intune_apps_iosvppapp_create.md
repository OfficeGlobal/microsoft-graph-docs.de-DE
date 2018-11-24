# <a name="create-iosvppapp"></a><span data-ttu-id="73f10-101">Erstellen von „iosVppApp“</span><span class="sxs-lookup"><span data-stu-id="73f10-101">Create iosVppApp</span></span>

> <span data-ttu-id="73f10-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="73f10-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73f10-103">Erstellen eines neuen [iosVppApp](../resources/intune_apps_iosvppapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="73f10-103">Create a new [iosVppApp](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73f10-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="73f10-104">Prerequisites</span></span>
<span data-ttu-id="73f10-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="73f10-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73f10-107">Permission type</span></span>|<span data-ttu-id="73f10-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73f10-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73f10-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73f10-109">Delegated (work or school account)</span></span>|<span data-ttu-id="73f10-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73f10-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73f10-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73f10-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73f10-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73f10-112">Not supported.</span></span>|
|<span data-ttu-id="73f10-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73f10-113">Application</span></span>|<span data-ttu-id="73f10-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73f10-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73f10-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73f10-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="73f10-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73f10-116">Request headers</span></span>
|<span data-ttu-id="73f10-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="73f10-117">Header</span></span>|<span data-ttu-id="73f10-118">Wert</span><span class="sxs-lookup"><span data-stu-id="73f10-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73f10-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="73f10-119">Authorization</span></span>|<span data-ttu-id="73f10-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="73f10-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73f10-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="73f10-121">Accept</span></span>|<span data-ttu-id="73f10-122">application/json</span><span class="sxs-lookup"><span data-stu-id="73f10-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73f10-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73f10-123">Request body</span></span>
<span data-ttu-id="73f10-124">Geben Sie im Anforderungstext eine JSON-Darstellung des iosVppApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="73f10-124">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="73f10-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosVppApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="73f10-125">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="73f10-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73f10-126">Property</span></span>|<span data-ttu-id="73f10-127">Typ</span><span class="sxs-lookup"><span data-stu-id="73f10-127">Type</span></span>|<span data-ttu-id="73f10-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73f10-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73f10-129">id</span><span class="sxs-lookup"><span data-stu-id="73f10-129">id</span></span>|<span data-ttu-id="73f10-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f10-130">String</span></span>|<span data-ttu-id="73f10-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="73f10-131">Key of the entity.</span></span> <span data-ttu-id="73f10-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73f10-133">displayName</span><span class="sxs-lookup"><span data-stu-id="73f10-133">displayName</span></span>|<span data-ttu-id="73f10-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f10-134">String</span></span>|<span data-ttu-id="73f10-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="73f10-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="73f10-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73f10-137">description</span><span class="sxs-lookup"><span data-stu-id="73f10-137">description</span></span>|<span data-ttu-id="73f10-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f10-138">String</span></span>|<span data-ttu-id="73f10-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="73f10-139">The description of the app.</span></span> <span data-ttu-id="73f10-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73f10-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="73f10-141">publisher</span></span>|<span data-ttu-id="73f10-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f10-142">String</span></span>|<span data-ttu-id="73f10-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="73f10-143">The publisher of the app.</span></span> <span data-ttu-id="73f10-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73f10-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="73f10-145">largeIcon</span></span>|[<span data-ttu-id="73f10-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="73f10-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="73f10-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="73f10-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="73f10-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73f10-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73f10-149">createdDateTime</span></span>|<span data-ttu-id="73f10-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73f10-150">DateTimeOffset</span></span>|<span data-ttu-id="73f10-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="73f10-151">The date and time the app was created.</span></span> <span data-ttu-id="73f10-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73f10-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73f10-153">lastModifiedDateTime</span></span>|<span data-ttu-id="73f10-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73f10-154">DateTimeOffset</span></span>|<span data-ttu-id="73f10-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="73f10-155">The date and time the app was last modified.</span></span> <span data-ttu-id="73f10-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73f10-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="73f10-157">isFeatured</span></span>|<span data-ttu-id="73f10-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="73f10-158">Boolean</span></span>|<span data-ttu-id="73f10-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73f10-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="73f10-160">privacyInformationUrl</span></span>|<span data-ttu-id="73f10-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f10-161">String</span></span>|<span data-ttu-id="73f10-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="73f10-162">The privacy statement Url.</span></span> <span data-ttu-id="73f10-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73f10-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="73f10-164">informationUrl</span></span>|<span data-ttu-id="73f10-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f10-165">String</span></span>|<span data-ttu-id="73f10-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="73f10-166">The more information Url.</span></span> <span data-ttu-id="73f10-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73f10-168">owner</span><span class="sxs-lookup"><span data-stu-id="73f10-168">owner</span></span>|<span data-ttu-id="73f10-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f10-169">String</span></span>|<span data-ttu-id="73f10-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="73f10-170">The owner of the app.</span></span> <span data-ttu-id="73f10-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73f10-172">developer</span><span class="sxs-lookup"><span data-stu-id="73f10-172">developer</span></span>|<span data-ttu-id="73f10-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f10-173">String</span></span>|<span data-ttu-id="73f10-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="73f10-174">The developer of the app.</span></span> <span data-ttu-id="73f10-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73f10-176">notes</span><span class="sxs-lookup"><span data-stu-id="73f10-176">notes</span></span>|<span data-ttu-id="73f10-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f10-177">String</span></span>|<span data-ttu-id="73f10-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="73f10-178">Notes for the app.</span></span> <span data-ttu-id="73f10-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="73f10-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="73f10-180">publishingState</span></span>|[<span data-ttu-id="73f10-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="73f10-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="73f10-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="73f10-182">The publishing state for the app.</span></span> <span data-ttu-id="73f10-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="73f10-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="73f10-184">Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73f10-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="73f10-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="73f10-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="73f10-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="73f10-186">usedLicenseCount</span></span>|<span data-ttu-id="73f10-187">Int32</span><span class="sxs-lookup"><span data-stu-id="73f10-187">Int32</span></span>|<span data-ttu-id="73f10-188">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="73f10-188">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="73f10-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="73f10-189">totalLicenseCount</span></span>|<span data-ttu-id="73f10-190">Int32</span><span class="sxs-lookup"><span data-stu-id="73f10-190">Int32</span></span>|<span data-ttu-id="73f10-191">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="73f10-191">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="73f10-192">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="73f10-192">releaseDateTime</span></span>|<span data-ttu-id="73f10-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73f10-193">DateTimeOffset</span></span>|<span data-ttu-id="73f10-194">Datum und Uhrzeit der Veröffentlichung der VPP-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="73f10-194">The VPP application release date and time.</span></span>|
|<span data-ttu-id="73f10-195">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="73f10-195">appStoreUrl</span></span>|<span data-ttu-id="73f10-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f10-196">String</span></span>|<span data-ttu-id="73f10-197">Store-URL</span><span class="sxs-lookup"><span data-stu-id="73f10-197">The store URL.</span></span>|
|<span data-ttu-id="73f10-198">licensingType</span><span class="sxs-lookup"><span data-stu-id="73f10-198">licensingType</span></span>|[<span data-ttu-id="73f10-199">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="73f10-199">vppLicensingType</span></span>](../resources/intune_apps_vpplicensingtype.md)|<span data-ttu-id="73f10-200">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="73f10-200">The supported License Type.</span></span>|
|<span data-ttu-id="73f10-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="73f10-201">applicableDeviceType</span></span>|[<span data-ttu-id="73f10-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="73f10-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="73f10-203">Gültiger iOS-Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="73f10-203">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="73f10-204">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="73f10-204">vppTokenOrganizationName</span></span>|<span data-ttu-id="73f10-205">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f10-205">String</span></span>|<span data-ttu-id="73f10-206">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="73f10-206">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="73f10-207">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="73f10-207">vppTokenAccountType</span></span>|[<span data-ttu-id="73f10-208">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="73f10-208">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="73f10-209">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="73f10-209">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="73f10-210">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="73f10-210">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="73f10-211">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="73f10-211">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="73f10-212">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="73f10-212">vppTokenAppleId</span></span>|<span data-ttu-id="73f10-213">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f10-213">String</span></span>|<span data-ttu-id="73f10-214">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="73f10-214">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="73f10-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="73f10-215">bundleId</span></span>|<span data-ttu-id="73f10-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f10-216">String</span></span>|<span data-ttu-id="73f10-217">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="73f10-217">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="73f10-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="73f10-218">Response</span></span>
<span data-ttu-id="73f10-219">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosVppApp](../resources/intune_apps_iosvppapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73f10-219">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73f10-220">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73f10-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="73f10-221">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73f10-221">Request</span></span>
<span data-ttu-id="73f10-222">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73f10-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1222

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

### <a name="response"></a><span data-ttu-id="73f10-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="73f10-223">Response</span></span>
<span data-ttu-id="73f10-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73f10-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



