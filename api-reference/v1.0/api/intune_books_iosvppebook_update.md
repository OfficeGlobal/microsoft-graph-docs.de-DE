# <a name="update-iosvppebook"></a><span data-ttu-id="3cf12-101">Aktualisieren von „iosVppEBook“</span><span class="sxs-lookup"><span data-stu-id="3cf12-101">Update iosVppEBook</span></span>

> <span data-ttu-id="3cf12-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3cf12-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cf12-103">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="3cf12-103">Update the properties of a [calendar](../resources/intune_books_iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3cf12-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3cf12-104">Prerequisites</span></span>
<span data-ttu-id="3cf12-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3cf12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3cf12-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3cf12-107">Permission type</span></span>|<span data-ttu-id="3cf12-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3cf12-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cf12-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3cf12-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3cf12-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cf12-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3cf12-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3cf12-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cf12-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3cf12-112">Not supported.</span></span>|
|<span data-ttu-id="3cf12-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3cf12-113">Application</span></span>|<span data-ttu-id="3cf12-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3cf12-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cf12-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3cf12-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="3cf12-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3cf12-116">Request headers</span></span>
|<span data-ttu-id="3cf12-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3cf12-117">Header</span></span>|<span data-ttu-id="3cf12-118">Wert</span><span class="sxs-lookup"><span data-stu-id="3cf12-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cf12-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cf12-119">Authorization</span></span>|<span data-ttu-id="3cf12-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3cf12-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3cf12-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3cf12-121">Accept</span></span>|<span data-ttu-id="3cf12-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3cf12-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cf12-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3cf12-123">Request body</span></span>
<span data-ttu-id="3cf12-124">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md) an.</span><span class="sxs-lookup"><span data-stu-id="3cf12-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_books_iosvppebook.md) object.</span></span>

<span data-ttu-id="3cf12-125">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3cf12-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="3cf12-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3cf12-126">Property</span></span>|<span data-ttu-id="3cf12-127">Typ</span><span class="sxs-lookup"><span data-stu-id="3cf12-127">Type</span></span>|<span data-ttu-id="3cf12-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3cf12-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cf12-129">id</span><span class="sxs-lookup"><span data-stu-id="3cf12-129">id</span></span>|<span data-ttu-id="3cf12-130">String</span><span class="sxs-lookup"><span data-stu-id="3cf12-130">String</span></span>|<span data-ttu-id="3cf12-131">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="3cf12-131">Key of the setting.</span></span> <span data-ttu-id="3cf12-132">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3cf12-132">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="3cf12-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3cf12-133">displayName</span></span>|<span data-ttu-id="3cf12-134">String</span><span class="sxs-lookup"><span data-stu-id="3cf12-134">String</span></span>|<span data-ttu-id="3cf12-135">Name des E-Books.</span><span class="sxs-lookup"><span data-stu-id="3cf12-135">Name of the folder.</span></span> <span data-ttu-id="3cf12-136">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3cf12-136">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="3cf12-137">description</span><span class="sxs-lookup"><span data-stu-id="3cf12-137">description</span></span>|<span data-ttu-id="3cf12-138">String</span><span class="sxs-lookup"><span data-stu-id="3cf12-138">String</span></span>|<span data-ttu-id="3cf12-139">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="3cf12-139">Description.</span></span> <span data-ttu-id="3cf12-140">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3cf12-140">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="3cf12-141">publisher</span><span class="sxs-lookup"><span data-stu-id="3cf12-141">Publisher</span></span>|<span data-ttu-id="3cf12-142">String</span><span class="sxs-lookup"><span data-stu-id="3cf12-142">String</span></span>|<span data-ttu-id="3cf12-143">Herausgeber.</span><span class="sxs-lookup"><span data-stu-id="3cf12-143">Publisher</span></span> <span data-ttu-id="3cf12-144">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3cf12-144">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="3cf12-145">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cf12-145">publishedDateTime</span></span>|<span data-ttu-id="3cf12-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cf12-146">DateTimeOffset</span></span>|<span data-ttu-id="3cf12-147">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="3cf12-147">The date and time when the page was created.</span></span> <span data-ttu-id="3cf12-148">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3cf12-148">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="3cf12-149">largeCover</span><span class="sxs-lookup"><span data-stu-id="3cf12-149">largeCover</span></span>|[<span data-ttu-id="3cf12-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3cf12-150">mimeContent</span></span>](../resources/intune_books_mimecontent.md)|<span data-ttu-id="3cf12-151">Umschlagbild des Buchs.</span><span class="sxs-lookup"><span data-stu-id="3cf12-151">Book cover</span></span> <span data-ttu-id="3cf12-152">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3cf12-152">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="3cf12-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3cf12-153">createdDateTime</span></span>|<span data-ttu-id="3cf12-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cf12-154">DateTimeOffset</span></span>|<span data-ttu-id="3cf12-155">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="3cf12-155">The date and time when the page was created.</span></span> <span data-ttu-id="3cf12-156">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3cf12-156">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="3cf12-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cf12-157">lastModifiedDateTime</span></span>|<span data-ttu-id="3cf12-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cf12-158">DateTimeOffset</span></span>|<span data-ttu-id="3cf12-159">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="3cf12-159">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="3cf12-160">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3cf12-160">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="3cf12-161">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3cf12-161">informationUrl</span></span>|<span data-ttu-id="3cf12-162">String</span><span class="sxs-lookup"><span data-stu-id="3cf12-162">String</span></span>|<span data-ttu-id="3cf12-163">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="3cf12-163">The more information Url.</span></span> <span data-ttu-id="3cf12-164">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3cf12-164">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="3cf12-165">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3cf12-165">privacyInformationUrl</span></span>|<span data-ttu-id="3cf12-166">String</span><span class="sxs-lookup"><span data-stu-id="3cf12-166">String</span></span>|<span data-ttu-id="3cf12-167">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="3cf12-167">The privacy statement Url.</span></span> <span data-ttu-id="3cf12-168">Geerbt von [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3cf12-168">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="3cf12-169">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="3cf12-169">vppTokenId</span></span>|<span data-ttu-id="3cf12-170">Guid</span><span class="sxs-lookup"><span data-stu-id="3cf12-170">Guid</span></span>|<span data-ttu-id="3cf12-171">ID des VPP-Tokens</span><span class="sxs-lookup"><span data-stu-id="3cf12-171">The Vpp token ID.</span></span>|
|<span data-ttu-id="3cf12-172">appleId</span><span class="sxs-lookup"><span data-stu-id="3cf12-172">appleId</span></span>|<span data-ttu-id="3cf12-173">String</span><span class="sxs-lookup"><span data-stu-id="3cf12-173">String</span></span>|<span data-ttu-id="3cf12-174">Apple-ID, die dem VPP-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="3cf12-174">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="3cf12-175">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="3cf12-175">vppOrganizationName</span></span>|<span data-ttu-id="3cf12-176">String</span><span class="sxs-lookup"><span data-stu-id="3cf12-176">String</span></span>|<span data-ttu-id="3cf12-177">Zum VPP-Token gehörender Organisationsname</span><span class="sxs-lookup"><span data-stu-id="3cf12-177">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="3cf12-178">genres</span><span class="sxs-lookup"><span data-stu-id="3cf12-178">genres</span></span>|<span data-ttu-id="3cf12-179">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="3cf12-179">String collection</span></span>|<span data-ttu-id="3cf12-180">Genres</span><span class="sxs-lookup"><span data-stu-id="3cf12-180">Genres.</span></span>|
|<span data-ttu-id="3cf12-181">language</span><span class="sxs-lookup"><span data-stu-id="3cf12-181">language</span></span>|<span data-ttu-id="3cf12-182">String</span><span class="sxs-lookup"><span data-stu-id="3cf12-182">String</span></span>|<span data-ttu-id="3cf12-183">Sprache</span><span class="sxs-lookup"><span data-stu-id="3cf12-183">language</span></span>|
|<span data-ttu-id="3cf12-184">seller</span><span class="sxs-lookup"><span data-stu-id="3cf12-184">seller</span></span>|<span data-ttu-id="3cf12-185">String</span><span class="sxs-lookup"><span data-stu-id="3cf12-185">String</span></span>|<span data-ttu-id="3cf12-186">Verkäufer</span><span class="sxs-lookup"><span data-stu-id="3cf12-186">Seller Dashboard</span></span>|
|<span data-ttu-id="3cf12-187">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3cf12-187">totalLicenseCount</span></span>|<span data-ttu-id="3cf12-188">Int32</span><span class="sxs-lookup"><span data-stu-id="3cf12-188">Int32</span></span>|<span data-ttu-id="3cf12-189">Gesamtanzahl von Lizenzen</span><span class="sxs-lookup"><span data-stu-id="3cf12-189">Total license count.</span></span>|
|<span data-ttu-id="3cf12-190">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3cf12-190">usedLicenseCount</span></span>|<span data-ttu-id="3cf12-191">Int32</span><span class="sxs-lookup"><span data-stu-id="3cf12-191">Int32</span></span>|<span data-ttu-id="3cf12-192">Gesamtanzahl von genutzten Lizenzen</span><span class="sxs-lookup"><span data-stu-id="3cf12-192">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="3cf12-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="3cf12-193">Response</span></span>
<span data-ttu-id="3cf12-194">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3cf12-194">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_books_iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cf12-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3cf12-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="3cf12-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3cf12-196">Request</span></span>
<span data-ttu-id="3cf12-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3cf12-197">Here is an example of the request.</span></span>
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
  "vppTokenId": "<Unknown Primitive Type Edm.Guid>",
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

### <a name="response"></a><span data-ttu-id="3cf12-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="3cf12-198">Response</span></span>
<span data-ttu-id="3cf12-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3cf12-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "vppTokenId": "<Unknown Primitive Type Edm.Guid>",
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



