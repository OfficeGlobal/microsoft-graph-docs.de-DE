# <a name="create-webapp"></a><span data-ttu-id="140f1-101">webApp erstellen</span><span class="sxs-lookup"><span data-stu-id="140f1-101">Create webApp</span></span>

> <span data-ttu-id="140f1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="140f1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="140f1-103">Erstellen eines neuen [webApp](../resources/intune_apps_webapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="140f1-103">Create a new [webApp](../resources/intune_apps_webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="140f1-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="140f1-104">Prerequisites</span></span>
<span data-ttu-id="140f1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="140f1-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="140f1-107">Permission type</span></span>|<span data-ttu-id="140f1-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="140f1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="140f1-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="140f1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="140f1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="140f1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="140f1-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="140f1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="140f1-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="140f1-112">Not supported.</span></span>|
|<span data-ttu-id="140f1-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="140f1-113">Application</span></span>|<span data-ttu-id="140f1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="140f1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="140f1-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="140f1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="140f1-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="140f1-116">Request headers</span></span>
|<span data-ttu-id="140f1-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="140f1-117">Header</span></span>|<span data-ttu-id="140f1-118">Wert</span><span class="sxs-lookup"><span data-stu-id="140f1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="140f1-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="140f1-119">Authorization</span></span>|<span data-ttu-id="140f1-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="140f1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="140f1-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="140f1-121">Accept</span></span>|<span data-ttu-id="140f1-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="140f1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="140f1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="140f1-123">Request body</span></span>
<span data-ttu-id="140f1-124">Geben Sie im Anforderungstext eine JSON-Darstellung des webApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="140f1-124">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="140f1-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der webApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="140f1-125">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="140f1-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="140f1-126">Property</span></span>|<span data-ttu-id="140f1-127">Typ</span><span class="sxs-lookup"><span data-stu-id="140f1-127">Type</span></span>|<span data-ttu-id="140f1-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="140f1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="140f1-129">id</span><span class="sxs-lookup"><span data-stu-id="140f1-129">id</span></span>|<span data-ttu-id="140f1-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="140f1-130">String</span></span>|<span data-ttu-id="140f1-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="140f1-131">Key of the entity.</span></span> <span data-ttu-id="140f1-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="140f1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="140f1-133">displayName</span></span>|<span data-ttu-id="140f1-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="140f1-134">String</span></span>|<span data-ttu-id="140f1-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="140f1-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="140f1-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="140f1-137">description</span><span class="sxs-lookup"><span data-stu-id="140f1-137">description</span></span>|<span data-ttu-id="140f1-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="140f1-138">String</span></span>|<span data-ttu-id="140f1-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="140f1-139">The description of the app.</span></span> <span data-ttu-id="140f1-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="140f1-141">publisher</span><span class="sxs-lookup"><span data-stu-id="140f1-141">publisher</span></span>|<span data-ttu-id="140f1-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="140f1-142">String</span></span>|<span data-ttu-id="140f1-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="140f1-143">The publisher of the app.</span></span> <span data-ttu-id="140f1-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="140f1-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="140f1-145">largeIcon</span></span>|[<span data-ttu-id="140f1-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="140f1-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="140f1-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="140f1-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="140f1-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="140f1-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="140f1-149">createdDateTime</span></span>|<span data-ttu-id="140f1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="140f1-150">DateTimeOffset</span></span>|<span data-ttu-id="140f1-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="140f1-151">The date and time the app was created.</span></span> <span data-ttu-id="140f1-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="140f1-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="140f1-153">lastModifiedDateTime</span></span>|<span data-ttu-id="140f1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="140f1-154">DateTimeOffset</span></span>|<span data-ttu-id="140f1-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="140f1-155">The date and time the app was last modified.</span></span> <span data-ttu-id="140f1-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="140f1-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="140f1-157">isFeatured</span></span>|<span data-ttu-id="140f1-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="140f1-158">Boolean</span></span>|<span data-ttu-id="140f1-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="140f1-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="140f1-160">privacyInformationUrl</span></span>|<span data-ttu-id="140f1-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="140f1-161">String</span></span>|<span data-ttu-id="140f1-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="140f1-162">The privacy statement Url.</span></span> <span data-ttu-id="140f1-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="140f1-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="140f1-164">informationUrl</span></span>|<span data-ttu-id="140f1-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="140f1-165">String</span></span>|<span data-ttu-id="140f1-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="140f1-166">The more information Url.</span></span> <span data-ttu-id="140f1-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="140f1-168">owner</span><span class="sxs-lookup"><span data-stu-id="140f1-168">owner</span></span>|<span data-ttu-id="140f1-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="140f1-169">String</span></span>|<span data-ttu-id="140f1-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="140f1-170">The owner of the app.</span></span> <span data-ttu-id="140f1-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="140f1-172">developer</span><span class="sxs-lookup"><span data-stu-id="140f1-172">developer</span></span>|<span data-ttu-id="140f1-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="140f1-173">String</span></span>|<span data-ttu-id="140f1-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="140f1-174">The developer of the app.</span></span> <span data-ttu-id="140f1-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="140f1-176">notes</span><span class="sxs-lookup"><span data-stu-id="140f1-176">notes</span></span>|<span data-ttu-id="140f1-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="140f1-177">String</span></span>|<span data-ttu-id="140f1-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="140f1-178">Notes for the app.</span></span> <span data-ttu-id="140f1-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="140f1-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="140f1-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="140f1-180">publishingState</span></span>|[<span data-ttu-id="140f1-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="140f1-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="140f1-p114">Der Veröffentlichungsstand der App. Die App kann nur dann zugewiesen werden, wenn die App veröffentlicht wird. Vererbt von [mobileApp](../resources/intune_apps_mobileapp.md). Die möglichen Werte sind: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="140f1-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="140f1-186">appUrl</span><span class="sxs-lookup"><span data-stu-id="140f1-186">appUrl</span></span>|<span data-ttu-id="140f1-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="140f1-187">String</span></span>|<span data-ttu-id="140f1-188">Die URL der Web-App.</span><span class="sxs-lookup"><span data-stu-id="140f1-188">The web app URL.</span></span>|
|<span data-ttu-id="140f1-189">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="140f1-189">useManagedBrowser</span></span>|<span data-ttu-id="140f1-190">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="140f1-190">Boolean</span></span>|<span data-ttu-id="140f1-191">Gibt an, ob ein verwalteter Browser verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="140f1-191">Whether or not to use managed browser.</span></span> <span data-ttu-id="140f1-192">Diese Eigenschaft ist nur für Android und IOS möglich.</span><span class="sxs-lookup"><span data-stu-id="140f1-192">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="140f1-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="140f1-193">Response</span></span>
<span data-ttu-id="140f1-194">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [webApp](../resources/intune_apps_webapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="140f1-194">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune_apps_webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="140f1-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="140f1-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="140f1-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="140f1-196">Request</span></span>
<span data-ttu-id="140f1-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="140f1-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="140f1-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="140f1-198">Response</span></span>
<span data-ttu-id="140f1-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="140f1-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








