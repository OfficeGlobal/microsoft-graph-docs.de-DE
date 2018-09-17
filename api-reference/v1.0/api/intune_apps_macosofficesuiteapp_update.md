# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="c9aa7-101">Aktualisieren von „macOSOfficeSuiteApp“</span><span class="sxs-lookup"><span data-stu-id="c9aa7-101">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="c9aa7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9aa7-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-103">Update the properties of a [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9aa7-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c9aa7-104">Prerequisites</span></span>
<span data-ttu-id="c9aa7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c9aa7-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c9aa7-107">Permission type</span></span>|<span data-ttu-id="c9aa7-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c9aa7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9aa7-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c9aa7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c9aa7-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9aa7-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c9aa7-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c9aa7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9aa7-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9aa7-112">Not supported.</span></span>|
|<span data-ttu-id="c9aa7-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c9aa7-113">Application</span></span>|<span data-ttu-id="c9aa7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9aa7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9aa7-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9aa7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="c9aa7-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9aa7-116">Request headers</span></span>
|<span data-ttu-id="c9aa7-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c9aa7-117">Header</span></span>|<span data-ttu-id="c9aa7-118">Wert</span><span class="sxs-lookup"><span data-stu-id="c9aa7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9aa7-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c9aa7-119">Authorization</span></span>|<span data-ttu-id="c9aa7-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c9aa7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9aa7-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="c9aa7-121">Accept</span></span>|<span data-ttu-id="c9aa7-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="c9aa7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9aa7-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9aa7-123">Request body</span></span>
<span data-ttu-id="c9aa7-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-124">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="c9aa7-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-125">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="c9aa7-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9aa7-126">Property</span></span>|<span data-ttu-id="c9aa7-127">Typ</span><span class="sxs-lookup"><span data-stu-id="c9aa7-127">Type</span></span>|<span data-ttu-id="c9aa7-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9aa7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9aa7-129">ID</span><span class="sxs-lookup"><span data-stu-id="c9aa7-129">id</span></span>|<span data-ttu-id="c9aa7-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9aa7-130">String</span></span>|<span data-ttu-id="c9aa7-131">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c9aa7-131">Key of the entity.</span></span> <span data-ttu-id="c9aa7-132">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c9aa7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c9aa7-133">displayName</span></span>|<span data-ttu-id="c9aa7-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9aa7-134">String</span></span>|<span data-ttu-id="c9aa7-135">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c9aa7-136">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c9aa7-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9aa7-137">description</span></span>|<span data-ttu-id="c9aa7-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9aa7-138">String</span></span>|<span data-ttu-id="c9aa7-139">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-139">The description of the app.</span></span> <span data-ttu-id="c9aa7-140">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c9aa7-141">Verleger</span><span class="sxs-lookup"><span data-stu-id="c9aa7-141">publisher</span></span>|<span data-ttu-id="c9aa7-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9aa7-142">String</span></span>|<span data-ttu-id="c9aa7-143">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-143">The publisher of the app.</span></span> <span data-ttu-id="c9aa7-144">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c9aa7-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c9aa7-145">largeIcon</span></span>|[<span data-ttu-id="c9aa7-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c9aa7-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="c9aa7-147">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c9aa7-148">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c9aa7-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9aa7-149">createdDateTime</span></span>|<span data-ttu-id="c9aa7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9aa7-150">DateTimeOffset</span></span>|<span data-ttu-id="c9aa7-151">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-151">The date and time the app was created.</span></span> <span data-ttu-id="c9aa7-152">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c9aa7-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9aa7-153">lastModifiedDateTime</span></span>|<span data-ttu-id="c9aa7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9aa7-154">DateTimeOffset</span></span>|<span data-ttu-id="c9aa7-155">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-155">The date and time the app was last modified.</span></span> <span data-ttu-id="c9aa7-156">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c9aa7-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c9aa7-157">isFeatured</span></span>|<span data-ttu-id="c9aa7-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="c9aa7-158">Boolean</span></span>|<span data-ttu-id="c9aa7-159">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c9aa7-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c9aa7-160">privacyInformationUrl</span></span>|<span data-ttu-id="c9aa7-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9aa7-161">String</span></span>|<span data-ttu-id="c9aa7-162">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-162">The privacy statement Url.</span></span> <span data-ttu-id="c9aa7-163">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c9aa7-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c9aa7-164">informationUrl</span></span>|<span data-ttu-id="c9aa7-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9aa7-165">String</span></span>|<span data-ttu-id="c9aa7-166">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-166">The more information Url.</span></span> <span data-ttu-id="c9aa7-167">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c9aa7-168">Besitzer</span><span class="sxs-lookup"><span data-stu-id="c9aa7-168">owner</span></span>|<span data-ttu-id="c9aa7-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9aa7-169">String</span></span>|<span data-ttu-id="c9aa7-170">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-170">The owner of the app.</span></span> <span data-ttu-id="c9aa7-171">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c9aa7-172">Entwickler</span><span class="sxs-lookup"><span data-stu-id="c9aa7-172">developer</span></span>|<span data-ttu-id="c9aa7-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9aa7-173">String</span></span>|<span data-ttu-id="c9aa7-174">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-174">The developer of the app.</span></span> <span data-ttu-id="c9aa7-175">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c9aa7-176">Hinweise</span><span class="sxs-lookup"><span data-stu-id="c9aa7-176">notes</span></span>|<span data-ttu-id="c9aa7-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9aa7-177">String</span></span>|<span data-ttu-id="c9aa7-178">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-178">Notes for the app.</span></span> <span data-ttu-id="c9aa7-179">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c9aa7-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="c9aa7-180">publishingState</span></span>|[<span data-ttu-id="c9aa7-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c9aa7-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="c9aa7-182">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-182">The publishing state for the app.</span></span> <span data-ttu-id="c9aa7-183">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c9aa7-184">Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9aa7-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="c9aa7-185">Mögliche Werte: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="c9aa7-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9aa7-186">Response</span></span>
<span data-ttu-id="c9aa7-187">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-187">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9aa7-188">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9aa7-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9aa7-189">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9aa7-189">Request</span></span>
<span data-ttu-id="c9aa7-190">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 590

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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="c9aa7-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9aa7-191">Response</span></span>
<span data-ttu-id="c9aa7-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9aa7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








