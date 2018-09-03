# <a name="create-iosvppapp"></a><span data-ttu-id="0aaf0-101">Erstellen von „iosVppApp“</span><span class="sxs-lookup"><span data-stu-id="0aaf0-101">Create iosVppApp</span></span>

> <span data-ttu-id="0aaf0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0aaf0-103">Erstellen eines neuen [iosVppApp](../resources/intune_apps_iosvppapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-103">Create a new [iosVppApp](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0aaf0-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0aaf0-104">Prerequisites</span></span>
<span data-ttu-id="0aaf0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0aaf0-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0aaf0-107">Permission type</span></span>|<span data-ttu-id="0aaf0-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0aaf0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0aaf0-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0aaf0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0aaf0-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0aaf0-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0aaf0-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0aaf0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0aaf0-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0aaf0-112">Not supported.</span></span>|
|<span data-ttu-id="0aaf0-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0aaf0-113">Application</span></span>|<span data-ttu-id="0aaf0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0aaf0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0aaf0-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0aaf0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0aaf0-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0aaf0-116">Request headers</span></span>
|<span data-ttu-id="0aaf0-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0aaf0-117">Header</span></span>|<span data-ttu-id="0aaf0-118">Wert</span><span class="sxs-lookup"><span data-stu-id="0aaf0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0aaf0-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0aaf0-119">Authorization</span></span>|<span data-ttu-id="0aaf0-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0aaf0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0aaf0-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="0aaf0-121">Accept</span></span>|<span data-ttu-id="0aaf0-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="0aaf0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aaf0-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0aaf0-123">Request body</span></span>
<span data-ttu-id="0aaf0-124">Geben Sie im Anforderungstext eine JSON-Darstellung des iosVppApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-124">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="0aaf0-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosVppApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-125">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="0aaf0-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0aaf0-126">Property</span></span>|<span data-ttu-id="0aaf0-127">Typ</span><span class="sxs-lookup"><span data-stu-id="0aaf0-127">Type</span></span>|<span data-ttu-id="0aaf0-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0aaf0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0aaf0-129">id</span><span class="sxs-lookup"><span data-stu-id="0aaf0-129">id</span></span>|<span data-ttu-id="0aaf0-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aaf0-130">String</span></span>|<span data-ttu-id="0aaf0-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0aaf0-131">Key of the entity.</span></span> <span data-ttu-id="0aaf0-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0aaf0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0aaf0-133">displayName</span></span>|<span data-ttu-id="0aaf0-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aaf0-134">String</span></span>|<span data-ttu-id="0aaf0-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0aaf0-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0aaf0-137">description</span><span class="sxs-lookup"><span data-stu-id="0aaf0-137">description</span></span>|<span data-ttu-id="0aaf0-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aaf0-138">String</span></span>|<span data-ttu-id="0aaf0-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-139">The description of the app.</span></span> <span data-ttu-id="0aaf0-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0aaf0-141">publisher</span><span class="sxs-lookup"><span data-stu-id="0aaf0-141">publisher</span></span>|<span data-ttu-id="0aaf0-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aaf0-142">String</span></span>|<span data-ttu-id="0aaf0-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-143">The publisher of the app.</span></span> <span data-ttu-id="0aaf0-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0aaf0-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0aaf0-145">largeIcon</span></span>|[<span data-ttu-id="0aaf0-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0aaf0-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="0aaf0-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0aaf0-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0aaf0-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0aaf0-149">createdDateTime</span></span>|<span data-ttu-id="0aaf0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0aaf0-150">DateTimeOffset</span></span>|<span data-ttu-id="0aaf0-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-151">The date and time the app was created.</span></span> <span data-ttu-id="0aaf0-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0aaf0-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0aaf0-153">lastModifiedDateTime</span></span>|<span data-ttu-id="0aaf0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0aaf0-154">DateTimeOffset</span></span>|<span data-ttu-id="0aaf0-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-155">The date and time the app was last modified.</span></span> <span data-ttu-id="0aaf0-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0aaf0-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0aaf0-157">isFeatured</span></span>|<span data-ttu-id="0aaf0-158">boolesch</span><span class="sxs-lookup"><span data-stu-id="0aaf0-158">Boolean</span></span>|<span data-ttu-id="0aaf0-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0aaf0-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0aaf0-160">privacyInformationUrl</span></span>|<span data-ttu-id="0aaf0-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aaf0-161">String</span></span>|<span data-ttu-id="0aaf0-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-162">The privacy statement Url.</span></span> <span data-ttu-id="0aaf0-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0aaf0-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0aaf0-164">informationUrl</span></span>|<span data-ttu-id="0aaf0-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aaf0-165">String</span></span>|<span data-ttu-id="0aaf0-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-166">The more information Url.</span></span> <span data-ttu-id="0aaf0-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0aaf0-168">Besitzer</span><span class="sxs-lookup"><span data-stu-id="0aaf0-168">owner</span></span>|<span data-ttu-id="0aaf0-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aaf0-169">String</span></span>|<span data-ttu-id="0aaf0-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-170">The owner of the app.</span></span> <span data-ttu-id="0aaf0-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0aaf0-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="0aaf0-172">developer</span></span>|<span data-ttu-id="0aaf0-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aaf0-173">String</span></span>|<span data-ttu-id="0aaf0-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-174">The developer of the app.</span></span> <span data-ttu-id="0aaf0-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0aaf0-176">Hinweise</span><span class="sxs-lookup"><span data-stu-id="0aaf0-176">notes</span></span>|<span data-ttu-id="0aaf0-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aaf0-177">String</span></span>|<span data-ttu-id="0aaf0-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-178">Notes for the app.</span></span> <span data-ttu-id="0aaf0-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0aaf0-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="0aaf0-180">publishingState</span></span>|[<span data-ttu-id="0aaf0-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0aaf0-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="0aaf0-182">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-182">The publishing state for the app.</span></span> <span data-ttu-id="0aaf0-183">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0aaf0-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0aaf0-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="0aaf0-185">Die möglichen Werte sind: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="0aaf0-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="0aaf0-186">usedLicenseCount</span></span>|<span data-ttu-id="0aaf0-187">Int32</span><span class="sxs-lookup"><span data-stu-id="0aaf0-187">Int32</span></span>|<span data-ttu-id="0aaf0-188">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-188">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="0aaf0-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="0aaf0-189">totalLicenseCount</span></span>|<span data-ttu-id="0aaf0-190">Int32</span><span class="sxs-lookup"><span data-stu-id="0aaf0-190">Int32</span></span>|<span data-ttu-id="0aaf0-191">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-191">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="0aaf0-192">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="0aaf0-192">releaseDateTime</span></span>|<span data-ttu-id="0aaf0-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0aaf0-193">DateTimeOffset</span></span>|<span data-ttu-id="0aaf0-194">Datum und Uhrzeit der Veröffentlichung der VPP-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-194">The VPP application release date and time.</span></span>|
|<span data-ttu-id="0aaf0-195">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0aaf0-195">appStoreUrl</span></span>|<span data-ttu-id="0aaf0-196">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aaf0-196">String</span></span>|<span data-ttu-id="0aaf0-197">Store-URL</span><span class="sxs-lookup"><span data-stu-id="0aaf0-197">The store URL.</span></span>|
|<span data-ttu-id="0aaf0-198">licensingType</span><span class="sxs-lookup"><span data-stu-id="0aaf0-198">licensingType</span></span>|[<span data-ttu-id="0aaf0-199">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="0aaf0-199">vppLicensingType</span></span>](../resources/intune_apps_vpplicensingtype.md)|<span data-ttu-id="0aaf0-200">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="0aaf0-200">The supported License Type.</span></span>|
|<span data-ttu-id="0aaf0-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="0aaf0-201">applicableDeviceType</span></span>|[<span data-ttu-id="0aaf0-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="0aaf0-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="0aaf0-203">Gültiger iOS-Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="0aaf0-203">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="0aaf0-204">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="0aaf0-204">vppTokenOrganizationName</span></span>|<span data-ttu-id="0aaf0-205">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aaf0-205">String</span></span>|<span data-ttu-id="0aaf0-206">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="0aaf0-206">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="0aaf0-207">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="0aaf0-207">vppTokenAccountType</span></span>|[<span data-ttu-id="0aaf0-208">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="0aaf0-208">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="0aaf0-209">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-209">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="0aaf0-210">Die möglichen Werte sind: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-210">The possible values are:</span></span> <span data-ttu-id="0aaf0-211">Die möglichen Werte sind: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-211">The possible values are:</span></span>|
|<span data-ttu-id="0aaf0-212">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="0aaf0-212">vppTokenAppleId</span></span>|<span data-ttu-id="0aaf0-213">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aaf0-213">String</span></span>|<span data-ttu-id="0aaf0-214">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="0aaf0-214">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="0aaf0-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="0aaf0-215">bundleId</span></span>|<span data-ttu-id="0aaf0-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0aaf0-216">String</span></span>|<span data-ttu-id="0aaf0-217">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="0aaf0-217">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="0aaf0-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="0aaf0-218">Response</span></span>
<span data-ttu-id="0aaf0-219">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosVppApp](../resources/intune_apps_iosvppapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-219">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aaf0-220">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0aaf0-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="0aaf0-221">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0aaf0-221">Request</span></span>
<span data-ttu-id="0aaf0-222">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-222">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0aaf0-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="0aaf0-223">Response</span></span>
<span data-ttu-id="0aaf0-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0aaf0-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



