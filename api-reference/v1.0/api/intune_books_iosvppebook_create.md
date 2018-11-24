# <a name="create-iosvppebook"></a><span data-ttu-id="24078-101">iosVppEBook erstellen</span><span class="sxs-lookup"><span data-stu-id="24078-101">Create iosVppEBook</span></span>

> <span data-ttu-id="24078-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="24078-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24078-103">Erstellt neue Objekte des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="24078-103">Create a new [iosVppEBook](../resources/intune_books_iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24078-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="24078-104">Prerequisites</span></span>
<span data-ttu-id="24078-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="24078-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="24078-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="24078-107">Permission type</span></span>|<span data-ttu-id="24078-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="24078-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24078-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="24078-109">Delegated (work or school account)</span></span>|<span data-ttu-id="24078-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24078-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="24078-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="24078-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24078-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24078-112">Not supported.</span></span>|
|<span data-ttu-id="24078-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="24078-113">Application</span></span>|<span data-ttu-id="24078-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24078-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24078-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="24078-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="24078-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="24078-116">Request headers</span></span>
|<span data-ttu-id="24078-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="24078-117">Header</span></span>|<span data-ttu-id="24078-118">Wert</span><span class="sxs-lookup"><span data-stu-id="24078-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24078-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="24078-119">Authorization</span></span>|<span data-ttu-id="24078-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="24078-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24078-121">Accept</span><span class="sxs-lookup"><span data-stu-id="24078-121">Accept</span></span>|<span data-ttu-id="24078-122">application/json</span><span class="sxs-lookup"><span data-stu-id="24078-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24078-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="24078-123">Request body</span></span>
<span data-ttu-id="24078-124">Geben Sie im Anforderungstext eine JSON-Darstellung des iosVppEBook-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="24078-124">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="24078-125">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des iosVppEBook erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="24078-125">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="24078-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="24078-126">Property</span></span>|<span data-ttu-id="24078-127">Typ</span><span class="sxs-lookup"><span data-stu-id="24078-127">Type</span></span>|<span data-ttu-id="24078-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24078-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24078-129">id</span><span class="sxs-lookup"><span data-stu-id="24078-129">id</span></span>|<span data-ttu-id="24078-130">String</span><span class="sxs-lookup"><span data-stu-id="24078-130">String</span></span>|<span data-ttu-id="24078-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="24078-131">Key of the entity.</span></span> <span data-ttu-id="24078-132">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="24078-132">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="24078-133">displayName</span><span class="sxs-lookup"><span data-stu-id="24078-133">displayName</span></span>|<span data-ttu-id="24078-134">String</span><span class="sxs-lookup"><span data-stu-id="24078-134">String</span></span>|<span data-ttu-id="24078-135">Name des E-Books.</span><span class="sxs-lookup"><span data-stu-id="24078-135">Name of the eBook.</span></span> <span data-ttu-id="24078-136">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="24078-136">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="24078-137">description</span><span class="sxs-lookup"><span data-stu-id="24078-137">description</span></span>|<span data-ttu-id="24078-138">String</span><span class="sxs-lookup"><span data-stu-id="24078-138">String</span></span>|<span data-ttu-id="24078-139">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="24078-139">Description.</span></span> <span data-ttu-id="24078-140">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="24078-140">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="24078-141">publisher</span><span class="sxs-lookup"><span data-stu-id="24078-141">publisher</span></span>|<span data-ttu-id="24078-142">String</span><span class="sxs-lookup"><span data-stu-id="24078-142">String</span></span>|<span data-ttu-id="24078-143">Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="24078-143">Publisher.</span></span> <span data-ttu-id="24078-144">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="24078-144">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="24078-145">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="24078-145">publishedDateTime</span></span>|<span data-ttu-id="24078-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24078-146">DateTimeOffset</span></span>|<span data-ttu-id="24078-147">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="24078-147">The date and time when the eBook was published.</span></span> <span data-ttu-id="24078-148">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="24078-148">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="24078-149">largeCover</span><span class="sxs-lookup"><span data-stu-id="24078-149">largeCover</span></span>|[<span data-ttu-id="24078-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="24078-150">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="24078-151">Umschlagbild des Buchs.</span><span class="sxs-lookup"><span data-stu-id="24078-151">Book cover.</span></span> <span data-ttu-id="24078-152">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="24078-152">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="24078-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24078-153">createdDateTime</span></span>|<span data-ttu-id="24078-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24078-154">DateTimeOffset</span></span>|<span data-ttu-id="24078-155">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="24078-155">The date and time when the eBook file was created.</span></span> <span data-ttu-id="24078-156">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="24078-156">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="24078-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24078-157">lastModifiedDateTime</span></span>|<span data-ttu-id="24078-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24078-158">DateTimeOffset</span></span>|<span data-ttu-id="24078-159">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="24078-159">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="24078-160">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="24078-160">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="24078-161">informationUrl</span><span class="sxs-lookup"><span data-stu-id="24078-161">informationUrl</span></span>|<span data-ttu-id="24078-162">String</span><span class="sxs-lookup"><span data-stu-id="24078-162">String</span></span>|<span data-ttu-id="24078-163">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="24078-163">The more information Url.</span></span> <span data-ttu-id="24078-164">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="24078-164">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="24078-165">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="24078-165">privacyInformationUrl</span></span>|<span data-ttu-id="24078-166">String</span><span class="sxs-lookup"><span data-stu-id="24078-166">String</span></span>|<span data-ttu-id="24078-167">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="24078-167">The privacy statement Url.</span></span> <span data-ttu-id="24078-168">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="24078-168">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="24078-169">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="24078-169">vppTokenId</span></span>|<span data-ttu-id="24078-170">Guid</span><span class="sxs-lookup"><span data-stu-id="24078-170">Guid</span></span>|<span data-ttu-id="24078-171">ID des VPP-Tokens</span><span class="sxs-lookup"><span data-stu-id="24078-171">The Vpp token ID.</span></span>|
|<span data-ttu-id="24078-172">appleId</span><span class="sxs-lookup"><span data-stu-id="24078-172">appleId</span></span>|<span data-ttu-id="24078-173">String</span><span class="sxs-lookup"><span data-stu-id="24078-173">String</span></span>|<span data-ttu-id="24078-174">Apple-ID, die dem VPP-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="24078-174">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="24078-175">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="24078-175">vppOrganizationName</span></span>|<span data-ttu-id="24078-176">String</span><span class="sxs-lookup"><span data-stu-id="24078-176">String</span></span>|<span data-ttu-id="24078-177">Zum VPP-Token gehörender Organisationsname</span><span class="sxs-lookup"><span data-stu-id="24078-177">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="24078-178">genres</span><span class="sxs-lookup"><span data-stu-id="24078-178">genres</span></span>|<span data-ttu-id="24078-179">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="24078-179">String collection</span></span>|<span data-ttu-id="24078-180">Genres</span><span class="sxs-lookup"><span data-stu-id="24078-180">Genres.</span></span>|
|<span data-ttu-id="24078-181">language</span><span class="sxs-lookup"><span data-stu-id="24078-181">language</span></span>|<span data-ttu-id="24078-182">String</span><span class="sxs-lookup"><span data-stu-id="24078-182">String</span></span>|<span data-ttu-id="24078-183">Sprache</span><span class="sxs-lookup"><span data-stu-id="24078-183">Language.</span></span>|
|<span data-ttu-id="24078-184">seller</span><span class="sxs-lookup"><span data-stu-id="24078-184">seller</span></span>|<span data-ttu-id="24078-185">String</span><span class="sxs-lookup"><span data-stu-id="24078-185">String</span></span>|<span data-ttu-id="24078-186">Verkäufer</span><span class="sxs-lookup"><span data-stu-id="24078-186">Seller.</span></span>|
|<span data-ttu-id="24078-187">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="24078-187">totalLicenseCount</span></span>|<span data-ttu-id="24078-188">Int32</span><span class="sxs-lookup"><span data-stu-id="24078-188">Int32</span></span>|<span data-ttu-id="24078-189">Gesamtanzahl von Lizenzen</span><span class="sxs-lookup"><span data-stu-id="24078-189">Total license count.</span></span>|
|<span data-ttu-id="24078-190">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="24078-190">usedLicenseCount</span></span>|<span data-ttu-id="24078-191">Int32</span><span class="sxs-lookup"><span data-stu-id="24078-191">Int32</span></span>|<span data-ttu-id="24078-192">Gesamtanzahl von genutzten Lizenzen</span><span class="sxs-lookup"><span data-stu-id="24078-192">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="24078-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="24078-193">Response</span></span>
<span data-ttu-id="24078-194">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosVppEBook](../resources/intune_books_iosvppebook.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24078-194">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune_books_iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24078-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="24078-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="24078-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24078-196">Request</span></span>
<span data-ttu-id="24078-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="24078-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 792

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
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

### <a name="response"></a><span data-ttu-id="24078-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="24078-198">Response</span></span>
<span data-ttu-id="24078-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24078-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 964

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
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
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



