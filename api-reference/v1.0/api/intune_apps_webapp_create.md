# <a name="create-webapp"></a><span data-ttu-id="ce82b-101">webApp erstellen</span><span class="sxs-lookup"><span data-stu-id="ce82b-101">Create webApp</span></span>

> <span data-ttu-id="ce82b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ce82b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce82b-103">Erstellen eines neuen [webApp](../resources/intune_apps_webapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ce82b-103">Create a new [plannerBucket](../resources/intune_apps_webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce82b-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ce82b-104">Prerequisites</span></span>
<span data-ttu-id="ce82b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce82b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ce82b-107">Permission type</span></span>|<span data-ttu-id="ce82b-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ce82b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce82b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ce82b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ce82b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce82b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce82b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ce82b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce82b-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce82b-112">Not supported.</span></span>|
|<span data-ttu-id="ce82b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ce82b-113">Application</span></span>|<span data-ttu-id="ce82b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce82b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce82b-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce82b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ce82b-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ce82b-116">Request headers</span></span>
|<span data-ttu-id="ce82b-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ce82b-117">Header</span></span>|<span data-ttu-id="ce82b-118">Wert</span><span class="sxs-lookup"><span data-stu-id="ce82b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce82b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce82b-119">Authorization</span></span>|<span data-ttu-id="ce82b-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ce82b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ce82b-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ce82b-121">Accept</span></span>|<span data-ttu-id="ce82b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ce82b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce82b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ce82b-123">Request body</span></span>
<span data-ttu-id="ce82b-124">Geben Sie im Anforderungstext eine JSON-Darstellung des webApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ce82b-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="ce82b-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der webApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ce82b-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="ce82b-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ce82b-126">Property</span></span>|<span data-ttu-id="ce82b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="ce82b-127">Type</span></span>|<span data-ttu-id="ce82b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce82b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce82b-129">id</span><span class="sxs-lookup"><span data-stu-id="ce82b-129">id</span></span>|<span data-ttu-id="ce82b-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce82b-130">String</span></span>|<span data-ttu-id="ce82b-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="ce82b-131">Key of the setting.</span></span> <span data-ttu-id="ce82b-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce82b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ce82b-133">displayName</span></span>|<span data-ttu-id="ce82b-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce82b-134">String</span></span>|<span data-ttu-id="ce82b-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="ce82b-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ce82b-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce82b-137">description</span><span class="sxs-lookup"><span data-stu-id="ce82b-137">description</span></span>|<span data-ttu-id="ce82b-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce82b-138">String</span></span>|<span data-ttu-id="ce82b-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="ce82b-139">The description of the app.</span></span> <span data-ttu-id="ce82b-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce82b-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="ce82b-141">Publisher</span></span>|<span data-ttu-id="ce82b-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce82b-142">String</span></span>|<span data-ttu-id="ce82b-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="ce82b-143">The name of the app.</span></span> <span data-ttu-id="ce82b-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce82b-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ce82b-145">largeIcon</span></span>|[<span data-ttu-id="ce82b-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ce82b-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="ce82b-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="ce82b-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ce82b-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce82b-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce82b-149">createdDateTime</span></span>|<span data-ttu-id="ce82b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce82b-150">DateTimeOffset</span></span>|<span data-ttu-id="ce82b-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="ce82b-151">The date and time the group was created.</span></span> <span data-ttu-id="ce82b-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce82b-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce82b-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ce82b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce82b-154">DateTimeOffset</span></span>|<span data-ttu-id="ce82b-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="ce82b-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="ce82b-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce82b-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ce82b-157">isFeatured</span></span>|<span data-ttu-id="ce82b-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce82b-158">Boolean</span></span>|<span data-ttu-id="ce82b-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce82b-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ce82b-160">privacyInformationUrl</span></span>|<span data-ttu-id="ce82b-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce82b-161">String</span></span>|<span data-ttu-id="ce82b-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="ce82b-162">The privacy statement Url.</span></span> <span data-ttu-id="ce82b-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce82b-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ce82b-164">informationUrl</span></span>|<span data-ttu-id="ce82b-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce82b-165">String</span></span>|<span data-ttu-id="ce82b-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="ce82b-166">The more information Url.</span></span> <span data-ttu-id="ce82b-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce82b-168">owner</span><span class="sxs-lookup"><span data-stu-id="ce82b-168">owner</span></span>|<span data-ttu-id="ce82b-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce82b-169">String</span></span>|<span data-ttu-id="ce82b-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="ce82b-170">The owner of the app.</span></span> <span data-ttu-id="ce82b-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce82b-172">developer</span><span class="sxs-lookup"><span data-stu-id="ce82b-172">developer</span></span>|<span data-ttu-id="ce82b-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce82b-173">String</span></span>|<span data-ttu-id="ce82b-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="ce82b-174">The name of the app.</span></span> <span data-ttu-id="ce82b-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce82b-176">notes</span><span class="sxs-lookup"><span data-stu-id="ce82b-176">notes</span></span>|<span data-ttu-id="ce82b-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce82b-177">String</span></span>|<span data-ttu-id="ce82b-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="ce82b-178">Notes for the app.</span></span> <span data-ttu-id="ce82b-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce82b-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce82b-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="ce82b-180">publishingState</span></span>|<span data-ttu-id="ce82b-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce82b-181">String</span></span>|<span data-ttu-id="ce82b-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="ce82b-182">The publishing state for the app.</span></span> <span data-ttu-id="ce82b-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="ce82b-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ce82b-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="ce82b-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ce82b-185">appUrl</span><span class="sxs-lookup"><span data-stu-id="ce82b-185">appUrl</span></span>|<span data-ttu-id="ce82b-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce82b-186">String</span></span>|<span data-ttu-id="ce82b-187">Die URL der Web-App.</span><span class="sxs-lookup"><span data-stu-id="ce82b-187">The web app URL.</span></span>|
|<span data-ttu-id="ce82b-188">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="ce82b-188">useManagedBrowser</span></span>|<span data-ttu-id="ce82b-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce82b-189">Boolean</span></span>|<span data-ttu-id="ce82b-190">Gibt an, ob ein verwalteter Browser verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="ce82b-190">Whether or not to use managed browser.</span></span> <span data-ttu-id="ce82b-191">Diese Eigenschaft ist nur für Android und IOS möglich.</span><span class="sxs-lookup"><span data-stu-id="ce82b-191">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="ce82b-192">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce82b-192">Response</span></span>
<span data-ttu-id="ce82b-193">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [webApp](../resources/intune_apps_webapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce82b-193">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_apps_webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce82b-194">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ce82b-194">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce82b-195">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce82b-195">Request</span></span>
<span data-ttu-id="ce82b-196">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ce82b-196">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 709

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="ce82b-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce82b-197">Response</span></span>
<span data-ttu-id="ce82b-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce82b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 817

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```



