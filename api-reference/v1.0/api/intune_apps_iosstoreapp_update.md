# <a name="update-iosstoreapp"></a><span data-ttu-id="2a7f6-101">iosStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2a7f6-101">Update iosStoreApp</span></span>

> <span data-ttu-id="2a7f6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a7f6-103">Aktualisieren der Eigenschaften eines [iosStoreApp](../resources/intune_apps_iosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-103">Update the properties of a [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a7f6-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2a7f6-104">Prerequisites</span></span>
<span data-ttu-id="2a7f6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2a7f6-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a7f6-107">Permission type</span></span>|<span data-ttu-id="2a7f6-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a7f6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a7f6-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a7f6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2a7f6-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a7f6-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2a7f6-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a7f6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a7f6-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a7f6-112">Not supported.</span></span>|
|<span data-ttu-id="2a7f6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a7f6-113">Application</span></span>|<span data-ttu-id="2a7f6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a7f6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a7f6-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a7f6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="2a7f6-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a7f6-116">Request headers</span></span>
|<span data-ttu-id="2a7f6-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2a7f6-117">Header</span></span>|<span data-ttu-id="2a7f6-118">Wert</span><span class="sxs-lookup"><span data-stu-id="2a7f6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a7f6-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2a7f6-119">Authorization</span></span>|<span data-ttu-id="2a7f6-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a7f6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a7f6-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="2a7f6-121">Accept</span></span>|<span data-ttu-id="2a7f6-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="2a7f6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a7f6-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a7f6-123">Request body</span></span>
<span data-ttu-id="2a7f6-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosStoreApp](../resources/intune_apps_iosstoreapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-124">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object.</span></span>

<span data-ttu-id="2a7f6-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosStoreApp](../resources/intune_apps_iosstoreapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-125">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune_apps_iosstoreapp.md).</span></span>

|<span data-ttu-id="2a7f6-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a7f6-126">Property</span></span>|<span data-ttu-id="2a7f6-127">Typ</span><span class="sxs-lookup"><span data-stu-id="2a7f6-127">Type</span></span>|<span data-ttu-id="2a7f6-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a7f6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a7f6-129">id</span><span class="sxs-lookup"><span data-stu-id="2a7f6-129">id</span></span>|<span data-ttu-id="2a7f6-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a7f6-130">String</span></span>|<span data-ttu-id="2a7f6-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2a7f6-131">Key of the entity.</span></span> <span data-ttu-id="2a7f6-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a7f6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2a7f6-133">displayName</span></span>|<span data-ttu-id="2a7f6-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a7f6-134">String</span></span>|<span data-ttu-id="2a7f6-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2a7f6-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a7f6-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a7f6-137">description</span></span>|<span data-ttu-id="2a7f6-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a7f6-138">String</span></span>|<span data-ttu-id="2a7f6-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-139">The description of the app.</span></span> <span data-ttu-id="2a7f6-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a7f6-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="2a7f6-141">publisher</span></span>|<span data-ttu-id="2a7f6-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a7f6-142">String</span></span>|<span data-ttu-id="2a7f6-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-143">The publisher of the app.</span></span> <span data-ttu-id="2a7f6-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a7f6-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2a7f6-145">largeIcon</span></span>|[<span data-ttu-id="2a7f6-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2a7f6-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="2a7f6-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2a7f6-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a7f6-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a7f6-149">createdDateTime</span></span>|<span data-ttu-id="2a7f6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a7f6-150">DateTimeOffset</span></span>|<span data-ttu-id="2a7f6-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-151">The date and time the app was created.</span></span> <span data-ttu-id="2a7f6-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a7f6-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a7f6-153">lastModifiedDateTime</span></span>|<span data-ttu-id="2a7f6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a7f6-154">DateTimeOffset</span></span>|<span data-ttu-id="2a7f6-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-155">The date and time the app was last modified.</span></span> <span data-ttu-id="2a7f6-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a7f6-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2a7f6-157">isFeatured</span></span>|<span data-ttu-id="2a7f6-158">boolesch</span><span class="sxs-lookup"><span data-stu-id="2a7f6-158">Boolean</span></span>|<span data-ttu-id="2a7f6-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a7f6-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2a7f6-160">privacyInformationUrl</span></span>|<span data-ttu-id="2a7f6-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a7f6-161">String</span></span>|<span data-ttu-id="2a7f6-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-162">The privacy statement Url.</span></span> <span data-ttu-id="2a7f6-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a7f6-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2a7f6-164">informationUrl</span></span>|<span data-ttu-id="2a7f6-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a7f6-165">String</span></span>|<span data-ttu-id="2a7f6-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-166">The more information Url.</span></span> <span data-ttu-id="2a7f6-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a7f6-168">Besitzer</span><span class="sxs-lookup"><span data-stu-id="2a7f6-168">owner</span></span>|<span data-ttu-id="2a7f6-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a7f6-169">String</span></span>|<span data-ttu-id="2a7f6-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-170">The owner of the app.</span></span> <span data-ttu-id="2a7f6-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a7f6-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="2a7f6-172">developer</span></span>|<span data-ttu-id="2a7f6-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a7f6-173">String</span></span>|<span data-ttu-id="2a7f6-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-174">The developer of the app.</span></span> <span data-ttu-id="2a7f6-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a7f6-176">Hinweise</span><span class="sxs-lookup"><span data-stu-id="2a7f6-176">notes</span></span>|<span data-ttu-id="2a7f6-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a7f6-177">String</span></span>|<span data-ttu-id="2a7f6-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-178">Notes for the app.</span></span> <span data-ttu-id="2a7f6-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="2a7f6-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="2a7f6-180">publishingState</span></span>|[<span data-ttu-id="2a7f6-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2a7f6-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="2a7f6-182">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-182">The publishing state for the app.</span></span> <span data-ttu-id="2a7f6-183">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2a7f6-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a7f6-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="2a7f6-185">Mögliche Werte sind: `notPublished`, `processing`,`published`.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-185">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="2a7f6-186">bundled</span><span class="sxs-lookup"><span data-stu-id="2a7f6-186">bundleId</span></span>|<span data-ttu-id="2a7f6-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a7f6-187">String</span></span>|<span data-ttu-id="2a7f6-188">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="2a7f6-188">The Identity Name.</span></span>|
|<span data-ttu-id="2a7f6-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2a7f6-189">appStoreUrl</span></span>|<span data-ttu-id="2a7f6-190">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a7f6-190">String</span></span>|<span data-ttu-id="2a7f6-191">URL des Apple-App-Stores</span><span class="sxs-lookup"><span data-stu-id="2a7f6-191">The Apple App Store URL</span></span>|
|<span data-ttu-id="2a7f6-192">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="2a7f6-192">applicableDeviceType</span></span>|[<span data-ttu-id="2a7f6-193">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2a7f6-193">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="2a7f6-194">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-194">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="2a7f6-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2a7f6-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2a7f6-196">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2a7f6-196">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="2a7f6-197">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="2a7f6-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a7f6-198">Response</span></span>
<span data-ttu-id="2a7f6-199">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [iosStoreApp](../resources/intune_apps_iosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-199">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a7f6-200">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a7f6-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a7f6-201">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a7f6-201">Request</span></span>
<span data-ttu-id="2a7f6-202">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1000

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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="2a7f6-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a7f6-203">Response</span></span>
<span data-ttu-id="2a7f6-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a7f6-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1158

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```



