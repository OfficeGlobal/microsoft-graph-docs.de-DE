# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="648a1-101">microsoftStoreForBusinessApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="648a1-101">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="648a1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="648a1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="648a1-103">Aktualisieren der Eigenschaften eines [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="648a1-103">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="648a1-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="648a1-104">Prerequisites</span></span>
<span data-ttu-id="648a1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="648a1-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="648a1-107">Permission type</span></span>|<span data-ttu-id="648a1-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="648a1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="648a1-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="648a1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="648a1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="648a1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="648a1-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="648a1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="648a1-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="648a1-112">Not supported.</span></span>|
|<span data-ttu-id="648a1-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="648a1-113">Application</span></span>|<span data-ttu-id="648a1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="648a1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="648a1-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="648a1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="648a1-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="648a1-116">Request headers</span></span>
|<span data-ttu-id="648a1-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="648a1-117">Header</span></span>|<span data-ttu-id="648a1-118">Wert</span><span class="sxs-lookup"><span data-stu-id="648a1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="648a1-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="648a1-119">Authorization</span></span>|<span data-ttu-id="648a1-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="648a1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="648a1-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="648a1-121">Accept</span></span>|<span data-ttu-id="648a1-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="648a1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="648a1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="648a1-123">Request body</span></span>
<span data-ttu-id="648a1-124">Geben Sie im Anforderungstext eine JSON-Darstellung für das [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="648a1-124">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="648a1-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="648a1-125">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="648a1-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="648a1-126">Property</span></span>|<span data-ttu-id="648a1-127">Typ</span><span class="sxs-lookup"><span data-stu-id="648a1-127">Type</span></span>|<span data-ttu-id="648a1-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="648a1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="648a1-129">ID</span><span class="sxs-lookup"><span data-stu-id="648a1-129">id</span></span>|<span data-ttu-id="648a1-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="648a1-130">String</span></span>|<span data-ttu-id="648a1-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="648a1-131">Key of the entity.</span></span> <span data-ttu-id="648a1-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="648a1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="648a1-133">displayName</span></span>|<span data-ttu-id="648a1-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="648a1-134">String</span></span>|<span data-ttu-id="648a1-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="648a1-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="648a1-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="648a1-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="648a1-137">description</span></span>|<span data-ttu-id="648a1-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="648a1-138">String</span></span>|<span data-ttu-id="648a1-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="648a1-139">The description of the app.</span></span> <span data-ttu-id="648a1-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="648a1-141">Verleger</span><span class="sxs-lookup"><span data-stu-id="648a1-141">publisher</span></span>|<span data-ttu-id="648a1-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="648a1-142">String</span></span>|<span data-ttu-id="648a1-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="648a1-143">The publisher of the app.</span></span> <span data-ttu-id="648a1-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="648a1-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="648a1-145">largeIcon</span></span>|[<span data-ttu-id="648a1-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="648a1-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="648a1-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="648a1-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="648a1-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="648a1-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="648a1-149">createdDateTime</span></span>|<span data-ttu-id="648a1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="648a1-150">DateTimeOffset</span></span>|<span data-ttu-id="648a1-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="648a1-151">The date and time the app was created.</span></span> <span data-ttu-id="648a1-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="648a1-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="648a1-153">lastModifiedDateTime</span></span>|<span data-ttu-id="648a1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="648a1-154">DateTimeOffset</span></span>|<span data-ttu-id="648a1-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="648a1-155">The date and time the app was last modified.</span></span> <span data-ttu-id="648a1-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="648a1-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="648a1-157">isFeatured</span></span>|<span data-ttu-id="648a1-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="648a1-158">Boolean</span></span>|<span data-ttu-id="648a1-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="648a1-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="648a1-160">privacyInformationUrl</span></span>|<span data-ttu-id="648a1-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="648a1-161">String</span></span>|<span data-ttu-id="648a1-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="648a1-162">The privacy statement Url.</span></span> <span data-ttu-id="648a1-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="648a1-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="648a1-164">informationUrl</span></span>|<span data-ttu-id="648a1-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="648a1-165">String</span></span>|<span data-ttu-id="648a1-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="648a1-166">The more information Url.</span></span> <span data-ttu-id="648a1-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="648a1-168">owner</span><span class="sxs-lookup"><span data-stu-id="648a1-168">owner</span></span>|<span data-ttu-id="648a1-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="648a1-169">String</span></span>|<span data-ttu-id="648a1-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="648a1-170">The owner of the app.</span></span> <span data-ttu-id="648a1-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="648a1-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="648a1-172">developer</span></span>|<span data-ttu-id="648a1-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="648a1-173">String</span></span>|<span data-ttu-id="648a1-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="648a1-174">The developer of the app.</span></span> <span data-ttu-id="648a1-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="648a1-176">Hinweise</span><span class="sxs-lookup"><span data-stu-id="648a1-176">notes</span></span>|<span data-ttu-id="648a1-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="648a1-177">String</span></span>|<span data-ttu-id="648a1-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="648a1-178">Notes for the app.</span></span> <span data-ttu-id="648a1-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="648a1-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="648a1-180">publishingState</span></span>|[<span data-ttu-id="648a1-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="648a1-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="648a1-182">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="648a1-182">The publishing state for the app.</span></span> <span data-ttu-id="648a1-183">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="648a1-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="648a1-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="648a1-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="648a1-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="648a1-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="648a1-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="648a1-186">usedLicenseCount</span></span>|<span data-ttu-id="648a1-187">Int32</span><span class="sxs-lookup"><span data-stu-id="648a1-187">Int32</span></span>|<span data-ttu-id="648a1-188">Die Anzahl von verwendeten Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="648a1-188">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="648a1-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="648a1-189">totalLicenseCount</span></span>|<span data-ttu-id="648a1-190">Int32</span><span class="sxs-lookup"><span data-stu-id="648a1-190">Int32</span></span>|<span data-ttu-id="648a1-191">Die Gesamtzahl der Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="648a1-191">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="648a1-192">productKey</span><span class="sxs-lookup"><span data-stu-id="648a1-192">productKey</span></span>|<span data-ttu-id="648a1-193">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="648a1-193">String</span></span>|<span data-ttu-id="648a1-194">Der Product Key der App</span><span class="sxs-lookup"><span data-stu-id="648a1-194">The app product key</span></span>|
|<span data-ttu-id="648a1-195">licenseType</span><span class="sxs-lookup"><span data-stu-id="648a1-195">licenseType</span></span>|[<span data-ttu-id="648a1-196">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="648a1-196">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune_apps_microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="648a1-197">Die Art der App-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="648a1-197">The app license type Possible values are: , .</span></span> <span data-ttu-id="648a1-198">Mögliche Werte sind: `offline` und `online`.</span><span class="sxs-lookup"><span data-stu-id="648a1-198">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="648a1-199">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="648a1-199">packageIdentityName</span></span>|<span data-ttu-id="648a1-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="648a1-200">String</span></span>|<span data-ttu-id="648a1-201">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="648a1-201">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="648a1-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="648a1-202">Response</span></span>
<span data-ttu-id="648a1-203">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="648a1-203">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="648a1-204">Beispiel</span><span class="sxs-lookup"><span data-stu-id="648a1-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="648a1-205">Anforderung</span><span class="sxs-lookup"><span data-stu-id="648a1-205">Request</span></span>
<span data-ttu-id="648a1-206">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="648a1-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 766

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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="648a1-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="648a1-207">Response</span></span>
<span data-ttu-id="648a1-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="648a1-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```








