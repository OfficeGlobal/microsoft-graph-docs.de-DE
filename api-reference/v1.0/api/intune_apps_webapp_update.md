# <a name="update-webapp"></a><span data-ttu-id="f9e85-101">webApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f9e85-101">Update webApp</span></span>

> <span data-ttu-id="f9e85-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f9e85-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9e85-103">Aktualisieren der Eigenschaften eines [webApp](../resources/intune_apps_webapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f9e85-103">Update the properties of a [calendar](../resources/intune_apps_webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9e85-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f9e85-104">Prerequisites</span></span>
<span data-ttu-id="f9e85-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f9e85-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f9e85-107">Permission type</span></span>|<span data-ttu-id="f9e85-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f9e85-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9e85-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f9e85-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f9e85-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9e85-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9e85-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f9e85-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9e85-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9e85-112">Not supported.</span></span>|
|<span data-ttu-id="f9e85-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f9e85-113">Application</span></span>|<span data-ttu-id="f9e85-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9e85-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9e85-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9e85-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f9e85-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f9e85-116">Request headers</span></span>
|<span data-ttu-id="f9e85-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f9e85-117">Header</span></span>|<span data-ttu-id="f9e85-118">Wert</span><span class="sxs-lookup"><span data-stu-id="f9e85-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9e85-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9e85-119">Authorization</span></span>|<span data-ttu-id="f9e85-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f9e85-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f9e85-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f9e85-121">Accept</span></span>|<span data-ttu-id="f9e85-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f9e85-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9e85-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f9e85-123">Request body</span></span>
<span data-ttu-id="f9e85-124">Geben Sie im Anforderungstext eine JSON-Darstellung des [webApp](../resources/intune_apps_webapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f9e85-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_webapp.md) object.</span></span>

<span data-ttu-id="f9e85-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [webApp](../resources/intune_apps_webapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f9e85-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="f9e85-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f9e85-126">Property</span></span>|<span data-ttu-id="f9e85-127">Typ</span><span class="sxs-lookup"><span data-stu-id="f9e85-127">Type</span></span>|<span data-ttu-id="f9e85-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9e85-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9e85-129">id</span><span class="sxs-lookup"><span data-stu-id="f9e85-129">id</span></span>|<span data-ttu-id="f9e85-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e85-130">String</span></span>|<span data-ttu-id="f9e85-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="f9e85-131">Key of the setting.</span></span> <span data-ttu-id="f9e85-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f9e85-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f9e85-133">displayName</span></span>|<span data-ttu-id="f9e85-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e85-134">String</span></span>|<span data-ttu-id="f9e85-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="f9e85-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f9e85-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f9e85-137">description</span><span class="sxs-lookup"><span data-stu-id="f9e85-137">description</span></span>|<span data-ttu-id="f9e85-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e85-138">String</span></span>|<span data-ttu-id="f9e85-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="f9e85-139">The description of the app.</span></span> <span data-ttu-id="f9e85-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f9e85-141">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="f9e85-141">Publisher</span></span>|<span data-ttu-id="f9e85-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e85-142">String</span></span>|<span data-ttu-id="f9e85-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="f9e85-143">The name of the app.</span></span> <span data-ttu-id="f9e85-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f9e85-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f9e85-145">largeIcon</span></span>|[<span data-ttu-id="f9e85-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f9e85-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="f9e85-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f9e85-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f9e85-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f9e85-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9e85-149">createdDateTime</span></span>|<span data-ttu-id="f9e85-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9e85-150">DateTimeOffset</span></span>|<span data-ttu-id="f9e85-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="f9e85-151">The date and time the group was created.</span></span> <span data-ttu-id="f9e85-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f9e85-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9e85-153">lastModifiedDateTime</span></span>|<span data-ttu-id="f9e85-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9e85-154">DateTimeOffset</span></span>|<span data-ttu-id="f9e85-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="f9e85-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="f9e85-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f9e85-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f9e85-157">isFeatured</span></span>|<span data-ttu-id="f9e85-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9e85-158">Boolean</span></span>|<span data-ttu-id="f9e85-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f9e85-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f9e85-160">privacyInformationUrl</span></span>|<span data-ttu-id="f9e85-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e85-161">String</span></span>|<span data-ttu-id="f9e85-162">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="f9e85-162">The privacy statement Url.</span></span> <span data-ttu-id="f9e85-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f9e85-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f9e85-164">informationUrl</span></span>|<span data-ttu-id="f9e85-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e85-165">String</span></span>|<span data-ttu-id="f9e85-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="f9e85-166">The more information Url.</span></span> <span data-ttu-id="f9e85-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f9e85-168">owner</span><span class="sxs-lookup"><span data-stu-id="f9e85-168">owner</span></span>|<span data-ttu-id="f9e85-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e85-169">String</span></span>|<span data-ttu-id="f9e85-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="f9e85-170">The owner of the app.</span></span> <span data-ttu-id="f9e85-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f9e85-172">developer</span><span class="sxs-lookup"><span data-stu-id="f9e85-172">developer</span></span>|<span data-ttu-id="f9e85-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e85-173">String</span></span>|<span data-ttu-id="f9e85-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="f9e85-174">The name of the app.</span></span> <span data-ttu-id="f9e85-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f9e85-176">notes</span><span class="sxs-lookup"><span data-stu-id="f9e85-176">notes</span></span>|<span data-ttu-id="f9e85-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e85-177">String</span></span>|<span data-ttu-id="f9e85-178">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="f9e85-178">Notes for the app.</span></span> <span data-ttu-id="f9e85-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9e85-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="f9e85-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="f9e85-180">publishingState</span></span>|<span data-ttu-id="f9e85-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e85-181">String</span></span>|<span data-ttu-id="f9e85-182">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="f9e85-182">The publishing state for the app.</span></span> <span data-ttu-id="f9e85-183">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="f9e85-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f9e85-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="f9e85-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f9e85-185">appUrl</span><span class="sxs-lookup"><span data-stu-id="f9e85-185">appUrl</span></span>|<span data-ttu-id="f9e85-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f9e85-186">String</span></span>|<span data-ttu-id="f9e85-187">Die URL der Web-App.</span><span class="sxs-lookup"><span data-stu-id="f9e85-187">The web app URL.</span></span>|
|<span data-ttu-id="f9e85-188">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="f9e85-188">useManagedBrowser</span></span>|<span data-ttu-id="f9e85-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f9e85-189">Boolean</span></span>|<span data-ttu-id="f9e85-190">Gibt an, ob ein verwalteter Browser verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f9e85-190">Whether or not to use managed browser.</span></span> <span data-ttu-id="f9e85-191">Diese Eigenschaft ist nur für Android und IOS möglich.</span><span class="sxs-lookup"><span data-stu-id="f9e85-191">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="f9e85-192">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9e85-192">Response</span></span>
<span data-ttu-id="f9e85-193">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [webApp](../resources/intune_apps_webapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9e85-193">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9e85-194">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f9e85-194">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9e85-195">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9e85-195">Request</span></span>
<span data-ttu-id="f9e85-196">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f9e85-196">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 664

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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="f9e85-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9e85-197">Response</span></span>
<span data-ttu-id="f9e85-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9e85-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



