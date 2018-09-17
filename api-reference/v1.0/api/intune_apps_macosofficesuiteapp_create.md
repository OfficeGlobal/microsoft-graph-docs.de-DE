# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="9ce25-101">Erstellen von „macOSOfficeSuiteApp“</span><span class="sxs-lookup"><span data-stu-id="9ce25-101">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="9ce25-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9ce25-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ce25-103">Diese Methode erstellt ein neues Objekt des Typs [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-103">Create a new [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9ce25-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9ce25-104">Prerequisites</span></span>
<span data-ttu-id="9ce25-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9ce25-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ce25-107">Permission type</span></span>|<span data-ttu-id="9ce25-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ce25-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ce25-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ce25-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9ce25-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ce25-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9ce25-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ce25-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ce25-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ce25-112">Not supported.</span></span>|
|<span data-ttu-id="9ce25-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ce25-113">Application</span></span>|<span data-ttu-id="9ce25-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ce25-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ce25-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ce25-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9ce25-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ce25-116">Request headers</span></span>
|<span data-ttu-id="9ce25-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9ce25-117">Header</span></span>|<span data-ttu-id="9ce25-118">Wert</span><span class="sxs-lookup"><span data-stu-id="9ce25-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ce25-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9ce25-119">Authorization</span></span>|<span data-ttu-id="9ce25-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9ce25-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ce25-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="9ce25-121">Accept</span></span>|<span data-ttu-id="9ce25-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="9ce25-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ce25-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ce25-123">Request body</span></span>
<span data-ttu-id="9ce25-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs „macOSOfficeSuiteApp“ an.</span><span class="sxs-lookup"><span data-stu-id="9ce25-124">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="9ce25-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSOfficeSuiteApp“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="9ce25-125">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="9ce25-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ce25-126">Property</span></span>|<span data-ttu-id="9ce25-127">Typ</span><span class="sxs-lookup"><span data-stu-id="9ce25-127">Type</span></span>|<span data-ttu-id="9ce25-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ce25-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ce25-129">ID</span><span class="sxs-lookup"><span data-stu-id="9ce25-129">id</span></span>|<span data-ttu-id="9ce25-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ce25-130">String</span></span>|<span data-ttu-id="9ce25-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9ce25-131">Key of the entity.</span></span> <span data-ttu-id="9ce25-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9ce25-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9ce25-133">displayName</span></span>|<span data-ttu-id="9ce25-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ce25-134">String</span></span>|<span data-ttu-id="9ce25-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="9ce25-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9ce25-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9ce25-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ce25-137">description</span></span>|<span data-ttu-id="9ce25-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ce25-138">String</span></span>|<span data-ttu-id="9ce25-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="9ce25-139">The description of the app.</span></span> <span data-ttu-id="9ce25-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9ce25-141">Verleger</span><span class="sxs-lookup"><span data-stu-id="9ce25-141">publisher</span></span>|<span data-ttu-id="9ce25-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ce25-142">String</span></span>|<span data-ttu-id="9ce25-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="9ce25-143">The publisher of the app.</span></span> <span data-ttu-id="9ce25-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9ce25-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9ce25-145">largeIcon</span></span>|[<span data-ttu-id="9ce25-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9ce25-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="9ce25-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="9ce25-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9ce25-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9ce25-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ce25-149">createdDateTime</span></span>|<span data-ttu-id="9ce25-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ce25-150">DateTimeOffset</span></span>|<span data-ttu-id="9ce25-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="9ce25-151">The date and time the app was created.</span></span> <span data-ttu-id="9ce25-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9ce25-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ce25-153">lastModifiedDateTime</span></span>|<span data-ttu-id="9ce25-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ce25-154">DateTimeOffset</span></span>|<span data-ttu-id="9ce25-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="9ce25-155">The date and time the app was last modified.</span></span> <span data-ttu-id="9ce25-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9ce25-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9ce25-157">isFeatured</span></span>|<span data-ttu-id="9ce25-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="9ce25-158">Boolean</span></span>|<span data-ttu-id="9ce25-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9ce25-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9ce25-160">privacyInformationUrl</span></span>|<span data-ttu-id="9ce25-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ce25-161">String</span></span>|<span data-ttu-id="9ce25-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="9ce25-162">The privacy statement Url.</span></span> <span data-ttu-id="9ce25-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9ce25-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9ce25-164">informationUrl</span></span>|<span data-ttu-id="9ce25-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ce25-165">String</span></span>|<span data-ttu-id="9ce25-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="9ce25-166">The more information Url.</span></span> <span data-ttu-id="9ce25-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9ce25-168">Besitzer</span><span class="sxs-lookup"><span data-stu-id="9ce25-168">owner</span></span>|<span data-ttu-id="9ce25-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ce25-169">String</span></span>|<span data-ttu-id="9ce25-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="9ce25-170">The owner of the app.</span></span> <span data-ttu-id="9ce25-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9ce25-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="9ce25-172">developer</span></span>|<span data-ttu-id="9ce25-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ce25-173">String</span></span>|<span data-ttu-id="9ce25-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="9ce25-174">The developer of the app.</span></span> <span data-ttu-id="9ce25-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9ce25-176">Hinweise</span><span class="sxs-lookup"><span data-stu-id="9ce25-176">notes</span></span>|<span data-ttu-id="9ce25-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ce25-177">String</span></span>|<span data-ttu-id="9ce25-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="9ce25-178">Notes for the app.</span></span> <span data-ttu-id="9ce25-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9ce25-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="9ce25-180">publishingState</span></span>|[<span data-ttu-id="9ce25-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9ce25-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="9ce25-182">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="9ce25-182">The publishing state for the app.</span></span> <span data-ttu-id="9ce25-183">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="9ce25-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9ce25-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ce25-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="9ce25-185">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="9ce25-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="9ce25-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ce25-186">Response</span></span>
<span data-ttu-id="9ce25-187">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9ce25-187">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ce25-188">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ce25-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="9ce25-189">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ce25-189">Request</span></span>
<span data-ttu-id="9ce25-190">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9ce25-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 648

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="9ce25-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ce25-191">Response</span></span>
<span data-ttu-id="9ce25-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ce25-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 756

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "publishingState": "processing"
}
```








