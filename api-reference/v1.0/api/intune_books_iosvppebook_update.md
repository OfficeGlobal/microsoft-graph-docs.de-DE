# <a name="update-iosvppebook"></a><span data-ttu-id="7e3c1-101">Aktualisieren von „iosVppEBook“</span><span class="sxs-lookup"><span data-stu-id="7e3c1-101">Update iosVppEBook</span></span>

> <span data-ttu-id="7e3c1-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e3c1-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="7e3c1-103">Update the properties of a [iosVppEBook](../resources/intune_books_iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e3c1-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7e3c1-104">Prerequisites</span></span>
<span data-ttu-id="7e3c1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7e3c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7e3c1-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7e3c1-107">Permission type</span></span>|<span data-ttu-id="7e3c1-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7e3c1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e3c1-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7e3c1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7e3c1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e3c1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7e3c1-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7e3c1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e3c1-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e3c1-112">Not supported.</span></span>|
|<span data-ttu-id="7e3c1-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7e3c1-113">Application</span></span>|<span data-ttu-id="7e3c1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e3c1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e3c1-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e3c1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="7e3c1-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7e3c1-116">Request headers</span></span>
|<span data-ttu-id="7e3c1-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7e3c1-117">Header</span></span>|<span data-ttu-id="7e3c1-118">Wert</span><span class="sxs-lookup"><span data-stu-id="7e3c1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e3c1-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7e3c1-119">Authorization</span></span>|<span data-ttu-id="7e3c1-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7e3c1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e3c1-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="7e3c1-121">Accept</span></span>|<span data-ttu-id="7e3c1-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="7e3c1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e3c1-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7e3c1-123">Request body</span></span>
<span data-ttu-id="7e3c1-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md) an.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-124">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune_books_iosvppebook.md) object.</span></span>

<span data-ttu-id="7e3c1-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-125">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune_books_iosvppebook.md).</span></span>

|<span data-ttu-id="7e3c1-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e3c1-126">Property</span></span>|<span data-ttu-id="7e3c1-127">Typ</span><span class="sxs-lookup"><span data-stu-id="7e3c1-127">Type</span></span>|<span data-ttu-id="7e3c1-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e3c1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e3c1-129">id</span><span class="sxs-lookup"><span data-stu-id="7e3c1-129">id</span></span>|<span data-ttu-id="7e3c1-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e3c1-130">String</span></span>|<span data-ttu-id="7e3c1-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-131">Key of the entity.</span></span> <span data-ttu-id="7e3c1-132">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7e3c1-132">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="7e3c1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7e3c1-133">displayName</span></span>|<span data-ttu-id="7e3c1-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e3c1-134">String</span></span>|<span data-ttu-id="7e3c1-135">Name des E-Books.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-135">Name of the eBook.</span></span> <span data-ttu-id="7e3c1-136">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7e3c1-136">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="7e3c1-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e3c1-137">description</span></span>|<span data-ttu-id="7e3c1-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e3c1-138">String</span></span>|<span data-ttu-id="7e3c1-139">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-139">Description.</span></span> <span data-ttu-id="7e3c1-140">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7e3c1-140">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="7e3c1-141">Verleger</span><span class="sxs-lookup"><span data-stu-id="7e3c1-141">publisher</span></span>|<span data-ttu-id="7e3c1-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e3c1-142">String</span></span>|<span data-ttu-id="7e3c1-143">Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-143">Publisher.</span></span> <span data-ttu-id="7e3c1-144">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7e3c1-144">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="7e3c1-145">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e3c1-145">publishedDateTime</span></span>|<span data-ttu-id="7e3c1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e3c1-146">DateTimeOffset</span></span>|<span data-ttu-id="7e3c1-147">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-147">The date and time when the eBook was published.</span></span> <span data-ttu-id="7e3c1-148">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7e3c1-148">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="7e3c1-149">largeCover</span><span class="sxs-lookup"><span data-stu-id="7e3c1-149">largeCover</span></span>|[<span data-ttu-id="7e3c1-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7e3c1-150">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="7e3c1-151">Umschlagbild des Buchs.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-151">Book cover.</span></span> <span data-ttu-id="7e3c1-152">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7e3c1-152">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="7e3c1-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e3c1-153">createdDateTime</span></span>|<span data-ttu-id="7e3c1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e3c1-154">DateTimeOffset</span></span>|<span data-ttu-id="7e3c1-155">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-155">The date and time when the eBook file was created.</span></span> <span data-ttu-id="7e3c1-156">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7e3c1-156">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="7e3c1-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e3c1-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7e3c1-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e3c1-158">DateTimeOffset</span></span>|<span data-ttu-id="7e3c1-159">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-159">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="7e3c1-160">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7e3c1-160">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="7e3c1-161">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7e3c1-161">informationUrl</span></span>|<span data-ttu-id="7e3c1-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e3c1-162">String</span></span>|<span data-ttu-id="7e3c1-163">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-163">The more information Url.</span></span> <span data-ttu-id="7e3c1-164">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7e3c1-164">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="7e3c1-165">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7e3c1-165">privacyInformationUrl</span></span>|<span data-ttu-id="7e3c1-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e3c1-166">String</span></span>|<span data-ttu-id="7e3c1-167">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-167">The privacy statement Url.</span></span> <span data-ttu-id="7e3c1-168">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7e3c1-168">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="7e3c1-169">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="7e3c1-169">vppTokenId</span></span>|<span data-ttu-id="7e3c1-170">Guid</span><span class="sxs-lookup"><span data-stu-id="7e3c1-170">Guid</span></span>|<span data-ttu-id="7e3c1-171">ID des VPP-Tokens</span><span class="sxs-lookup"><span data-stu-id="7e3c1-171">The Vpp token ID.</span></span>|
|<span data-ttu-id="7e3c1-172">appleId</span><span class="sxs-lookup"><span data-stu-id="7e3c1-172">appleId</span></span>|<span data-ttu-id="7e3c1-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e3c1-173">String</span></span>|<span data-ttu-id="7e3c1-174">Apple-ID, die dem VPP-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="7e3c1-174">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="7e3c1-175">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="7e3c1-175">vppOrganizationName</span></span>|<span data-ttu-id="7e3c1-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e3c1-176">String</span></span>|<span data-ttu-id="7e3c1-177">Zum VPP-Token gehörender Organisationsname</span><span class="sxs-lookup"><span data-stu-id="7e3c1-177">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="7e3c1-178">Genre</span><span class="sxs-lookup"><span data-stu-id="7e3c1-178">genres</span></span>|<span data-ttu-id="7e3c1-179">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="7e3c1-179">String collection</span></span>|<span data-ttu-id="7e3c1-180">Genres</span><span class="sxs-lookup"><span data-stu-id="7e3c1-180">Genres.</span></span>|
|<span data-ttu-id="7e3c1-181">Sprache</span><span class="sxs-lookup"><span data-stu-id="7e3c1-181">language</span></span>|<span data-ttu-id="7e3c1-182">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e3c1-182">String</span></span>|<span data-ttu-id="7e3c1-183">Sprache</span><span class="sxs-lookup"><span data-stu-id="7e3c1-183">Language.</span></span>|
|<span data-ttu-id="7e3c1-184">Verkäufer</span><span class="sxs-lookup"><span data-stu-id="7e3c1-184">seller</span></span>|<span data-ttu-id="7e3c1-185">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e3c1-185">String</span></span>|<span data-ttu-id="7e3c1-186">Verkäufer</span><span class="sxs-lookup"><span data-stu-id="7e3c1-186">Seller.</span></span>|
|<span data-ttu-id="7e3c1-187">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7e3c1-187">totalLicenseCount</span></span>|<span data-ttu-id="7e3c1-188">Int32</span><span class="sxs-lookup"><span data-stu-id="7e3c1-188">Int32</span></span>|<span data-ttu-id="7e3c1-189">Gesamtanzahl von Lizenzen</span><span class="sxs-lookup"><span data-stu-id="7e3c1-189">Total license count.</span></span>|
|<span data-ttu-id="7e3c1-190">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7e3c1-190">usedLicenseCount</span></span>|<span data-ttu-id="7e3c1-191">Int32</span><span class="sxs-lookup"><span data-stu-id="7e3c1-191">Int32</span></span>|<span data-ttu-id="7e3c1-192">Gesamtanzahl von genutzten Lizenzen</span><span class="sxs-lookup"><span data-stu-id="7e3c1-192">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="7e3c1-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e3c1-193">Response</span></span>
<span data-ttu-id="7e3c1-194">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-194">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune_books_iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e3c1-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7e3c1-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="7e3c1-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e3c1-196">Request</span></span>
<span data-ttu-id="7e3c1-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
Content-type: application/json
Content-length: 803

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "79199ed9-e50b-4257-8de4-70b9c8685061",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```

### <a name="response"></a><span data-ttu-id="7e3c1-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e3c1-198">Response</span></span>
<span data-ttu-id="7e3c1-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e3c1-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 961

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "79199ed9-e50b-4257-8de4-70b9c8685061",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```



