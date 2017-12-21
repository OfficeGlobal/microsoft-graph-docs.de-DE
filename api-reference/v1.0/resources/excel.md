# <a name="working-with-excel-in-microsoft-graph"></a><span data-ttu-id="74036-101">Arbeiten mit Excel in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="74036-101">Working with Excel in Microsoft Graph</span></span>

<span data-ttu-id="74036-p101">Sie können Microsoft Graph verwenden, um es Web- und Mobilanwendungen zu ermöglichen, in OneDrive, SharePoint oder anderen unterstützten Speicherplattformen gespeicherte Excel-Arbeitsmappen zu lesen und zu bearbeiten. Die `Workbook`- (bzw. Excel-Datei-)Ressource enthält alle anderen Excel-Ressourcen über Beziehungen. Sie können über die [Laufwerks-API](drive.md) auf eine Arbeitsmappe zugreifen, indem Sie den Speicherort der Datei in der URL identifizieren. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="74036-p101">You can use Microsoft Graph to allow web and mobile applications to read and modify Excel workbooks stored in OneDrive, SharePoint, or other supported storage platforms. The `Workbook` (or Excel file) resource contains all the other Excel resources through relationships. You can access a workbook through the [Drive API](drive.md) by identifying the location of the file in the URL. For example:</span></span>

`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`  
`https://graph.microsoft.com/{version}/me/drive/root:/{item-path}:/workbook/`  

<span data-ttu-id="74036-p102">Sie können auf eine Reihe von Excel-Objekten (wie Tabelle, Bereich oder Diagramm) mithilfe von standardmäßigen REST-APIs zugreifen, um Vorgänge zum Erstellen, Lesen, Aktualisieren und Löschen in der Abeitsmappe durchzuführen. Beispielsweise gibt `GET https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/worksheets`</span><span class="sxs-lookup"><span data-stu-id="74036-p102">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, `GET https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/worksheets`</span></span>  
<span data-ttu-id="74036-108">eine Sammlung von Arbeitsblattobjekten zurück, die Teil der Arbeitsmappe sind.</span><span class="sxs-lookup"><span data-stu-id="74036-108">returns a collection of worksheet objects that are part of the workbook.</span></span>    


<span data-ttu-id="74036-p103">**Hinweis:** Die Excel-REST-API unterstützt nur Arbeitsmappen im Office Open XML-Dateiformat. Arbeitsmappen mit der Erweiterung `.xls` werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="74036-p103">**Note:** The Excel REST API supports only Office Open XML file formatted workbooks. The `.xls` extension workbooks are not supported.</span></span> 

## <a name="authorization-and-scopes"></a><span data-ttu-id="74036-111">Autorisierung und Bereiche</span><span class="sxs-lookup"><span data-stu-id="74036-111">Authorization and scopes</span></span>

<span data-ttu-id="74036-112">Sie können den [Azure AD v.2-Endpunkt](https://developer.microsoft.com/de-DE/graph/docs/authorization/converged_auth) verwenden, um Excel-APIs zu authentifizieren.</span><span class="sxs-lookup"><span data-stu-id="74036-112">You can use the [Azure AD v.2 endpoint](https://developer.microsoft.com/de-DE/graph/docs/authorization/converged_auth) to authenticate Excel APIs.</span></span> <span data-ttu-id="74036-113">Alle APIs benötigen den `Authorization: Bearer {access-token}`-HTTP-Header.</span><span class="sxs-lookup"><span data-stu-id="74036-113">All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="74036-114">Einer der folgenden [Berechtigungsbereiche](https://developer.microsoft.com/de-DE/graph/docs/authorization/permission_scopes) ist erforderlich, um die Excel-Ressource zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="74036-114">One of the following [permission scopes](https://developer.microsoft.com/de-DE/graph/docs/authorization/permission_scopes) is required to use the Excel resource:</span></span>

* <span data-ttu-id="74036-115">Files.Read (für Leseaktionen)</span><span class="sxs-lookup"><span data-stu-id="74036-115">Files.Read (for read actions)</span></span>
* <span data-ttu-id="74036-116">Files.ReadWrite (für Lese- und Schreibaktionen)</span><span class="sxs-lookup"><span data-stu-id="74036-116">Files.ReadWrite (for read and write actions)</span></span>


## <a name="sessions-and-persistence"></a><span data-ttu-id="74036-117">Sitzungen und Beständigkeit</span><span class="sxs-lookup"><span data-stu-id="74036-117">Sessions and persistence</span></span>

<span data-ttu-id="74036-118">Excel-APIs können in einem der drei folgenden Modi aufgerufen werden:</span><span class="sxs-lookup"><span data-stu-id="74036-118">Excel APIs can be called in one of three modes:</span></span> 

1. <span data-ttu-id="74036-119">Beständige Sitzung: Alle an der Arbeitsmappe vorgenommenen Änderungen werden gespeichert.</span><span class="sxs-lookup"><span data-stu-id="74036-119">Persistent session - All changes made to the workbook are persisted (saved).</span></span> <span data-ttu-id="74036-120">Dies ist die effizienteste und leistungsfähige Modus des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="74036-120">This is the most efficient and performant mode of operation.</span></span> 
2. <span data-ttu-id="74036-p106">Nicht beständige Sitzung: Die von der API vorgenommenen Änderungen werden nicht am Quellspeicherort gespeichert. Stattdessen behält der Excel-Back-End-Server eine temporäre Kopie der Datei  bei, welche die während dieser API-Sitzung vorgenommenen Änderungen enthält. Wenn die Excel-Sitzung abläuft, gehen die Änderungen verloren. Dieser Modus eignet sich für Apps, die Analysen durchführen oder die Ergebnisse einer Berechnung oder eines Diagrammbilds abrufen, aber nicht den Dokumentstatus betreffen.</span><span class="sxs-lookup"><span data-stu-id="74036-p106">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span> 
3. <span data-ttu-id="74036-125">Sitzungslos: Der API-Aufruf erfolgt ohne Sitzungsinformationen.</span><span class="sxs-lookup"><span data-stu-id="74036-125">Sessionless - The API call is made without session information.</span></span> <span data-ttu-id="74036-126">Excel-Server müssen jedes Mal die Arbeitsmappen-Kopie des Servers lokalisieren, um den Vorgang auszuführen. Daher ist dies keine effiziente Methode zum Aufrufen von Excel-APIs.</span><span class="sxs-lookup"><span data-stu-id="74036-126">Excel servers have to locate the server's copy of the workbook each time to perform the operation and hence this is not an efficient way for call Excel APIs.</span></span> <span data-ttu-id="74036-127">Sie eignet sich für die Abfrage von Ausnahmefällen.</span><span class="sxs-lookup"><span data-stu-id="74036-127">It is suitable for making one off requests.</span></span> 

<span data-ttu-id="74036-128">Um die Sitzung in der API darzustellen, verwenden Sie den `workbook-session-id: {session-id}`-Header.</span><span class="sxs-lookup"><span data-stu-id="74036-128">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="74036-p108">**Hinweis:** Der Sitzungsheader ist für das Funktionieren einer Excel-API nicht erforderlich. Die Verwendung des Sitzungsheaders wird jedoch empfohlen, um die Leistung zu verbessern. Wenn Sie keinen Sitzungsheader verwenden, _werden_ die während des API-Aufrufs vorgenommenen Änderungen in der Datei gespeichert.</span><span class="sxs-lookup"><span data-stu-id="74036-p108">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

### <a name="api-call-to-get-a-session"></a><span data-ttu-id="74036-132">API-Aufruf, um eine Sitzung aufzurufen</span><span class="sxs-lookup"><span data-stu-id="74036-132">API call to get a session</span></span> 

#### <a name="request"></a><span data-ttu-id="74036-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-133">Request</span></span> 

<span data-ttu-id="74036-134">Übergeben Sie ein JSON-Objekt durch Festlegen des `persistchanges`-Wert auf `true` oder `false`.</span><span class="sxs-lookup"><span data-stu-id="74036-134">Pass a JSON object by setting the `persistchanges` value to `true` or `false`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/createSession
content-type: Application/Json 
authorization: Bearer {access-token}

{ "persistChanges": true }
```

<span data-ttu-id="74036-135">Wenn der Wert auf `persistChanges` oder `false` festgelegt wird, wird eine nicht beständige Sitzungs-ID zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74036-135">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span>  


#### <a name="response"></a><span data-ttu-id="74036-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-136">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#microsoft.graph.sessionInfo",
  "id": "{session-id}",
  "persistChanges": true
}
```

#### <a name="usage"></a><span data-ttu-id="74036-137">Verwendung</span><span class="sxs-lookup"><span data-stu-id="74036-137">Usage</span></span> 

<span data-ttu-id="74036-138">Die vom vorherigen Aufruf zurückgegebene Sitzungs-ID wird als Header in nachfolgenden API-Anforderungen im</span><span class="sxs-lookup"><span data-stu-id="74036-138">The session ID returned from the previous call is passed as a header on subsequent API requests in</span></span>  
<span data-ttu-id="74036-139">`workbook-session-id`-HTTP-Header dargestellt.</span><span class="sxs-lookup"><span data-stu-id="74036-139">`workbook-session-id` HTTP header.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

><span data-ttu-id="74036-140">Hinweis: Wenn die Sitzungs-ID abgelaufen ist, wird ein `404` HTTP-Fehlercode an die Sitzung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74036-140">Note: If the session id has expired, a `404` HTTP error code is returned on the session.</span></span> <span data-ttu-id="74036-141">In einem solchen Szenario können Sie eine neue Sitzung erstellen und fortfahren.</span><span class="sxs-lookup"><span data-stu-id="74036-141">In such a scenarion, you can choose to create a new session and continue.</span></span> <span data-ttu-id="74036-142">Sie können aber auch die Sitzung regelmäßig aktualisieren, damit die Sitzung erhalten bleibt.</span><span class="sxs-lookup"><span data-stu-id="74036-142">Another approach would be to refresh the session periodically to keep the session alive.</span></span> <span data-ttu-id="74036-143">In der Regel läuft eine beständige Sitzung nach ca. 7 Minuten Inaktivität ab.</span><span class="sxs-lookup"><span data-stu-id="74036-143">Typically the persistent session expires after about 7 minutes of inactivity.</span></span> <span data-ttu-id="74036-144">Eine nicht beständige Sitzung läuft nach ca. 5 Minuten Inaktivität ab.</span><span class="sxs-lookup"><span data-stu-id="74036-144">Non persistent session expires after about 5 minutes of inactivity.</span></span> 

## <a name="common-excel-scenarios"></a><span data-ttu-id="74036-145">Häufige Excel-Szenarien</span><span class="sxs-lookup"><span data-stu-id="74036-145">Common Excel scenarios</span></span>

<span data-ttu-id="74036-146">Dieser Abschnitt enthält Beispiele für häufige Vorgänge,die Sie für Excel-Objekte verwenden können.</span><span class="sxs-lookup"><span data-stu-id="74036-146">This section provides examples of the common operations you can use on Excel objects.</span></span>

### <a name="worksheet-operations"></a><span data-ttu-id="74036-147">Arbeitsblattvorgänge</span><span class="sxs-lookup"><span data-stu-id="74036-147">Worksheet operations</span></span>

#### <a name="list-worksheets-part-of-the-workbook"></a><span data-ttu-id="74036-148">Den Arbeitsblätterteil der Arbeitsmappe auflisten</span><span class="sxs-lookup"><span data-stu-id="74036-148">List worksheets part of the workbook</span></span> 
<span data-ttu-id="74036-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-149">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="74036-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-150">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0000-000000000000}",
      "name": "Sheet1",
      "position": 0,
      "visibility": "Visible"
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0100-000000000000}",
      "name": "Sheet57664",
      "position": 1,
      "visibility": "Visible"
    }
  ]
}
```
#### <a name="add-a-new-worksheet"></a><span data-ttu-id="74036-151">Neues Arbeitsblatt hinzufügen</span><span class="sxs-lookup"><span data-stu-id="74036-151">Add a new worksheet</span></span> 
 
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "Sheet32243" }
```

<span data-ttu-id="74036-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-152">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

#### <a name="get-a-new-worksheet"></a><span data-ttu-id="74036-153">Neues Arbeitsblatt abrufen</span><span class="sxs-lookup"><span data-stu-id="74036-153">Get a new worksheet</span></span> 

<span data-ttu-id="74036-154">Rufen Sie ein Arbeitsblatt basierend auf den Namen ab.</span><span class="sxs-lookup"><span data-stu-id="74036-154">Get a worksheet based on the name.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/Sheet32243
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="74036-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-155">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

<span data-ttu-id="74036-p110">** Hinweis: Arbeitsblätter können auch mit der ID abgerufen werden. Derzeit enthält die ID jedoch die Zeichen `{` und „}“, für die eine URL-Codierung durchgeführt werden muss, damit die API funktioniert. Beispiel: Um ein Arbeitsblatt mit der ID `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}` abzurufen, führen Sie für die ID im Pfad die folgende URL-Codierung durch: `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span><span class="sxs-lookup"><span data-stu-id="74036-p110">** Note: Worksheets can also be retrieved using the ID. However, currently the ID contains `{` and '}' characters, which needs to be URL encoded for the API to work. Example: In order to get a worksheet with ID of `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, URL encode the ID in the path as `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span></span> 

#### <a name="delete-a-worksheet"></a><span data-ttu-id="74036-159">Arbeitsblatt löschen</span><span class="sxs-lookup"><span data-stu-id="74036-159">Delete a worksheet</span></span>

<span data-ttu-id="74036-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-160">Request</span></span>
```
DELETE /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="74036-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-161">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="update-worksheet-properties"></a><span data-ttu-id="74036-162">Arbeitsblatteigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="74036-162">Update worksheet properties</span></span>

<span data-ttu-id="74036-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-163">Request</span></span> 

```
PATCH /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/SheetA
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "SheetA", "position": 3 }
```

<span data-ttu-id="74036-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-164">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
  "id": "{00000000-0001-0000-0100-000000000000}",
  "name": "SheetA",
  "position": 3,
  "visibility": "Visible"
}
```

### <a name="chart-operations"></a><span data-ttu-id="74036-165">Diagrammvorgänge</span><span class="sxs-lookup"><span data-stu-id="74036-165">Chart operations</span></span>

#### <a name="list-charts-that-are-part-of-the-worksheet"></a><span data-ttu-id="74036-166">Diagramme auflisten, die Teil des Arbeitsblatts sind</span><span class="sxs-lookup"><span data-stu-id="74036-166">List charts that are part of the worksheet</span></span> 

<span data-ttu-id="74036-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-167">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="74036-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-168">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B00000000-0008-0000-0100-000003000000%7D%27)",
      "height": 235.5,
      "id": "{00000000-0008-0000-0100-000003000000}",
      "left": 276.0,
      "name": "Chart 2",
      "top": 0.0,
      "width": 401.25
   }
  ]
}
```

<span data-ttu-id="74036-p111">** Hinweis: Die Diagramm-ID enthält die Zeichen `{` und `}` (Beispiel: `{00000000-0008-0000-0100-000003000000}`), für die eine URL-Codierung durchgeführt werden muss, damit die API funktioniert. Beispiel: Um ein Diagrammobjekt abzurufen, führen Sie für die ID im Pfad die folgende URL-Codierung durch: `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span><span class="sxs-lookup"><span data-stu-id="74036-p111">** Note: Chart ID contains `{` and `}` characters (example: `{00000000-0008-0000-0100-000003000000}`), which needs to be URL encoded for the API to work. Example: In order to get a chart object, URL encode the ID in the path as `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span></span> 

#### <a name="get-chart-image"></a><span data-ttu-id="74036-171">Diagrammbild abrufen</span><span class="sxs-lookup"><span data-stu-id="74036-171">Get chart image</span></span>

<span data-ttu-id="74036-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-172">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B00000000-0008-0000-0100-000003000000%7D')/Image(width=0,height=0,fittingMode='fit')
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="74036-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-173">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#Edm.String",
  "value": "{base-64-string}"
}
```

#### <a name="add-a-chart"></a><span data-ttu-id="74036-174">Diagramm hinzufügen</span><span class="sxs-lookup"><span data-stu-id="74036-174">Add a chart</span></span>  

<span data-ttu-id="74036-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-175">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/Add
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 

{ "type": "ColumnClustered", "sourcedata": "A1:C4", "seriesby": "Auto" }
```

<span data-ttu-id="74036-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-176">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#chart",
  "@odata.type": "#microsoft.graph.chart",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "Chart 2",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-a-chart"></a><span data-ttu-id="74036-177">Diagramm aktualisieren</span><span class="sxs-lookup"><span data-stu-id="74036-177">Update a chart</span></span>

<!-- { "blockType": "ignored" } -->
```http 
PATCH /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "height": 216.0, "left": 0, "name": "NewName", "top": 0, "width": 360.0 }

```
<span data-ttu-id="74036-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-178">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "NewName",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-chart-source-data"></a><span data-ttu-id="74036-179">Quelldaten des Diagramms aktualisieren</span><span class="sxs-lookup"><span data-stu-id="74036-179">Update chart source data</span></span> 

<span data-ttu-id="74036-180">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-180">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')/setData
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "sourceData": "A1:C4", "seriesBy": "Auto" }
```

<span data-ttu-id="74036-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-181">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="table-operations"></a><span data-ttu-id="74036-182">Tabellenvorgänge</span><span class="sxs-lookup"><span data-stu-id="74036-182">Table operations</span></span> 

#### <a name="get-list-of-tables"></a><span data-ttu-id="74036-183">Liste der Tabellen abrufen</span><span class="sxs-lookup"><span data-stu-id="74036-183">Get list of tables</span></span> 

<span data-ttu-id="74036-184">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-184">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/tables
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="74036-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-185">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 
```

#### <a name="create-table"></a><span data-ttu-id="74036-186">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="74036-186">Create Table</span></span>

<span data-ttu-id="74036-187">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-187">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http 
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables/$/add
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "hasHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="74036-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-188">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)",
  "id": "2",
  "name": "NewTableName",
  "showHeaders": true,
  "showTotals": false,
  "style": "TableStyleMedium4"
}
```

#### <a name="update-table"></a><span data-ttu-id="74036-189">Tabelle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="74036-189">Update table</span></span>

<span data-ttu-id="74036-190">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-190">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http 
PATCH /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "showHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="74036-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-191">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)",
  "id": "2",
  "name": "NewTableName",
  "showHeaders": true,
  "showTotals": false,
  "style": "TableStyleMedium4"
}
```

#### <a name="get-list-of-table-rows"></a><span data-ttu-id="74036-192">Liste der Tabellenzeilen abrufen</span><span class="sxs-lookup"><span data-stu-id="74036-192">Get list of table rows</span></span>
<span data-ttu-id="74036-193">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-193">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="74036-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-194">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(0)",
      "index": 0,
      "values": [
        [
          42019,
          53,
          34
       ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(1)",
      "index": 1,
      "values": [
        [
          42020,
          45,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(2)",
      "index": 2,
      "values": [
        [
          42021,
          50,
          31
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(3)",
      "index": 3,
      "values": [
        [
          42022,
          43,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(4)",
      "index": 4,
      "values": [
        [
          42023,
          45,
          41
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(5)",
      "index": 5,
      "values": [
        [
          42024,
          52,
          40
        ]
      ]
    }
  ]
}
```

#### <a name="get-list-of-table-columns"></a><span data-ttu-id="74036-195">Liste der Tabellenspalten abrufen</span><span class="sxs-lookup"><span data-stu-id="74036-195">Get list of table columns</span></span>

<span data-ttu-id="74036-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-196">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Columns
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="74036-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-197">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/columns",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%271%27)",
      "id": "1",
      "index": 0,
      "name": "Date",
      "values": [
        [
          "Date"
        ],
        [
          42019
       ],
        [
          42020
        ],
        [
          42021
        ],
        [
          42022
        ],
        [
          42023
        ],
        [
          42024
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%272%27)",
      "id": "2",
      "index": 1,
      "name": "High (F)",
      "values": [
        [
          "High (F)"
        ],
        [
          53
        ],
        [
          45
        ],
        [
          50
        ],
        [
          43
        ],
        [
          45
        ],
        [
          52
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%273%27)",
      "id": "3",
      "index": 2,
      "name": "Low (F)",
      "values": [
        [
          "Low (F)"
        ],
        [
          34
        ],
        [
          39
        ],
        [
          31
        ],
        [
          39
        ],
        [
          41
        ],
        [
          40
        ]
      ]
    }
  ]
}
```


#### <a name="add-a-table-row"></a><span data-ttu-id="74036-198">Tabellenzeile hinzufügen</span><span class="sxs-lookup"><span data-stu-id="74036-198">Add a table row</span></span>

<span data-ttu-id="74036-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-199">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Jan-15-2016", "49", "37" ] ], "index": null }
```

<span data-ttu-id="74036-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-200">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows(null)",
  "index": 6,
  "values": [
    [
      "Jan-15-2016",
      49,
      37
    ]
  ]
}
```

#### <a name="add-a-table-column"></a><span data-ttu-id="74036-201">Tabellenspalte hinzufügen</span><span class="sxs-lookup"><span data-stu-id="74036-201">Add a table column</span></span> 

<span data-ttu-id="74036-202">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-202">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http 
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')/Columns
content-type: Application/Json 
accept: application/Json 


{ "values": [ [ "Status" ], [ "Open" ], [ "Closed" ] ], "index": 2 }
```

<span data-ttu-id="74036-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-203">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('2')/columns/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)/columns(%274%27)",
  "id": "4",
  "index": 2,
  "name": "Status",
  "values": [
    [
      "Status"
    ],
    [
      "Open"
    ],
    [
      "Closed"
    ]
  ]
}
```

#### <a name="delete-table-row"></a><span data-ttu-id="74036-204">Tabellenzeile löschen</span><span class="sxs-lookup"><span data-stu-id="74036-204">Delete table row</span></span>

<span data-ttu-id="74036-205">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-205">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http  
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows/$/ItemAt(index=6)
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="74036-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-206">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="delete-table-column"></a><span data-ttu-id="74036-207">Tabellenspalte löschen</span><span class="sxs-lookup"><span data-stu-id="74036-207">Delete table column</span></span> 
<span data-ttu-id="74036-208">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-208">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Columns('3')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="74036-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-209">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="convert-table-to-range"></a><span data-ttu-id="74036-210">Tabelle in Bereich konvertieren</span><span class="sxs-lookup"><span data-stu-id="74036-210">Convert table to range</span></span> 
<span data-ttu-id="74036-211">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-211">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('1')/convertToRange
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="74036-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-212">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 
```

#### <a name="table-sort"></a><span data-ttu-id="74036-213">Tabelle sortieren</span><span class="sxs-lookup"><span data-stu-id="74036-213">Table sort</span></span>
<span data-ttu-id="74036-214">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-214">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```


<span data-ttu-id="74036-215">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-215">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="table-filter"></a><span data-ttu-id="74036-216">Tabelle filtern</span><span class="sxs-lookup"><span data-stu-id="74036-216">Table filter</span></span>
<span data-ttu-id="74036-217">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-217">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"criteria" : 
  { "filterOn": "custom",
   "criterion1": ">15",
   "operator": "and",
   "criterion2": "<50"
   
  }
}
```

<span data-ttu-id="74036-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-218">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="clear-filter"></a><span data-ttu-id="74036-219">Filter löschen</span><span class="sxs-lookup"><span data-stu-id="74036-219">Clear filter</span></span>
<span data-ttu-id="74036-220">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-220">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/clear
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="74036-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-221">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="range-operations"></a><span data-ttu-id="74036-222">Bereichsvorgänge</span><span class="sxs-lookup"><span data-stu-id="74036-222">Range operations</span></span>

#### <a name="get-range"></a><span data-ttu-id="74036-223">Bereich abrufen</span><span class="sxs-lookup"><span data-stu-id="74036-223">Get Range</span></span> 

<span data-ttu-id="74036-224">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-224">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/worksheets('test')/range(address='A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="74036-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-225">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#range",
  "@odata.type": "#microsoft.graph.range",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasLocal": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasR1C1": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "values": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "valueTypes": [
    [
      "Empty",
      "Empty"
    ],
    [
      "Empty",
      "Empty"
    ]
  ]
}
```

#### <a name="range-update"></a><span data-ttu-id="74036-226">Bereich aktualisieren</span><span class="sxs-lookup"><span data-stu-id="74036-226">Range update</span></span> 

<!-- { "blockType": "ignored" } -->
```http
PATCH /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/worksheets('test')/range(address='test!A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Test", "Value" ], [ "For", "Update" ] ] }
```

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#range",
  "@odata.type": "#microsoft.graph.range",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27test!A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasLocal": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasR1C1": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "values": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "valueTypes": [
    [
      "String",
      "String"
    ],
    [
      "String",
      "String"
    ]
  ]
}
```

#### <a name="range-sort"></a><span data-ttu-id="74036-227">Bereich sortieren</span><span class="sxs-lookup"><span data-stu-id="74036-227">Range sort</span></span>
<span data-ttu-id="74036-228">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-228">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/usedRange/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```

<span data-ttu-id="74036-229">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-229">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


### <a name="named-items"></a><span data-ttu-id="74036-230">Benannte Elemente</span><span class="sxs-lookup"><span data-stu-id="74036-230">Named items</span></span>
<span data-ttu-id="74036-231">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-231">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/names
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="74036-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-232">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27data%27)",
      "name": "data",
      "type": "Range",
      "value": "Range!$A$1:$D$3",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27myrange%27)",
      "name": "myrange",
      "type": "Range",
      "value": "Range!$E$1:$F$7",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27range1%27)",
      "name": "range1",
      "type": "Range",
      "value": "Range!$I$1:$M$11",
      "visible": true
    }
  ]
}
```

### <a name="work-with-nulls"></a><span data-ttu-id="74036-233">Verwenden von Daten</span><span class="sxs-lookup"><span data-stu-id="74036-233">Work with nulls</span></span>

#### <a name="null-input-in-2-d-array"></a><span data-ttu-id="74036-234">NULL-Eingabe im 2D-Array</span><span class="sxs-lookup"><span data-stu-id="74036-234">null input in 2-D array</span></span>

<span data-ttu-id="74036-p112">Die `null`-Eingabe in einem zweidimensionalen Array (für Werte, Zahlenformate, Formeln) wird in den Bereichs- und Tabellenressourcen ignoriert. Am beabsichtigten Ziel (Zelle) findet keine Aktualisierung statt, wenn die `null`-Eingabe in Werten, im Zahlenformat oder Formelraster von Werten gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="74036-p112">`null` input inside a two-dimensional array (for values, number-format, formula) is ignored in the Range and Table resources. No update will take place to the intended target (cell) when `null` input is sent in values or number-format or formula grid of values.</span></span>

<span data-ttu-id="74036-237">Um nur bestimmte Teile des Bereichs zu aktualisieren, wie z. B. das Zahlenformat einer Zelle, und das vorhandene Zahlenformat in anderen Teilen des Bereichs beizubehalten, legen Sie das gewünschte Zahlenformat an entsprechender Stelle fest und senden Sie `null` für die anderen Zellen.</span><span class="sxs-lookup"><span data-stu-id="74036-237">For example, to only update specific parts of the Range, such as a cell's Number Format, and to retain the existing number-format on other parts of the Range, set the Number Format where needed and send `null` for the other cells.</span></span>

<span data-ttu-id="74036-238">In der folgenden Set-Anforderung werden nur einige Teile des Bereichszahlenformats festgelegt, dabei wird das vorhandene Zahlenformat im verbleibenden Teil beibehalten (durch NULL-Übergabe).</span><span class="sxs-lookup"><span data-stu-id="74036-238">In the following set request, only some parts of the Range Number Format are set while the existing Number Format on the remaining part is retained (by passing nulls).</span></span>

```json
{
  "values" : [["Eurasia", "29.96", "0.25", "15-Feb" ]],
  "numberFormat" : [[null, null, null, "m/d/yyyy;@"]]
}
```

#### <a name="null-input-for-a-property"></a><span data-ttu-id="74036-239">NULL-Eingabe für eine Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="74036-239">null input for a property</span></span>

<span data-ttu-id="74036-p113">`null` ist keine gültige einzelne Eingabe für die gesamte Eigenschaft. Folgende Eingabe ist beispielsweise ungültig, da die gesamten Werte nicht auf NULL festgelegt oder ignoriert werden können.</span><span class="sxs-lookup"><span data-stu-id="74036-p113">`null` is not a valid single input for the entire property. For example, the following is not valid because the entire values cannot be set to null or ignored.</span></span>

```json
{
"values":  null
}

```

<span data-ttu-id="74036-242">Folgendes ist ebenfalls nicht gültig, da NULL kein gültiger Farbwert ist.</span><span class="sxs-lookup"><span data-stu-id="74036-242">The following is not valid either as null is not a valid color value.</span></span>

```json
{
"color" :  null
}
```

#### <a name="null-response"></a><span data-ttu-id="74036-243">NULL-Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-243">Null-Response</span></span>

<span data-ttu-id="74036-244">Darstellungen der Formatierungseigenschaften, die aus ungleichmäßigen Werten bestehen, ergeben einen NULL-Wert in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="74036-244">Representation of formatting properties that consists of non-uniform values results in the return of a null value in the response.</span></span>

<span data-ttu-id="74036-p114">So kann z. B. ein Bereich aus einer oder mehreren Zellen bestehen. In Fällen, in denen die im angegebenen Bereich enthaltenen einzelnen Zellen keine gleichmäßigen Formatierungswerte enthalten, wird die Bereichsebenendarstellung undefiniert.</span><span class="sxs-lookup"><span data-stu-id="74036-p114">For example, a Range can consist of one or more cells. In cases where the individual cells contained in the Range specified don't have uniform formatting values, the range level representation will be undefined.</span></span>

```json
{
  "size: : null,
  "color" : null
}
```


### <a name="blank-input-and-output"></a><span data-ttu-id="74036-247">Leere Eingabe und Ausgabe</span><span class="sxs-lookup"><span data-stu-id="74036-247">Blank input and output</span></span>

<span data-ttu-id="74036-p115">Leere Werte in Aktualisierungsanforderungen werden als Anweisung behandelt, um die entsprechende Eigenschaft zu löschen oder zurückzusetzen. Ein leerer Wert wird durch zwei doppelte Anführungszeichen ohne Leerzeichen dazwischen dargestellt: `""`</span><span class="sxs-lookup"><span data-stu-id="74036-p115">Blank values in update requests are treated as an instruction to clear or reset the respective property. A blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

<span data-ttu-id="74036-250">Beispiele:</span><span class="sxs-lookup"><span data-stu-id="74036-250">Examples:</span></span>

* <span data-ttu-id="74036-251">Für `values` wird der Bereichswert gelöscht. Das ist genauso wie das Löschen des Inhalts in der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="74036-251">For `values`, the range value is cleared out. This is the same as clearing the contents in the application.</span></span>

* <span data-ttu-id="74036-252">Für `numberFormat` wird das Zahlenformat auf `General` festgelegt.</span><span class="sxs-lookup"><span data-stu-id="74036-252">For `numberFormat`, the number format is set to `General`.</span></span>

* <span data-ttu-id="74036-253">Für `formula` und `formulaLocale` werden die Formelwerte gelöscht.</span><span class="sxs-lookup"><span data-stu-id="74036-253">For `formula` and `formulaLocale`, the formula values are cleared.</span></span>


<span data-ttu-id="74036-p116">Für Lesevorgänge können Sie leere Werte erwarten, wenn der Inhalt der Zellen leer ist. Wenn die Zelle keine Daten oder keinen Wert enthält, gibt die API einen leeren Wert zurück. Ein leerer Wert wird durch zwei doppelte Anführungszeichen ohne Leerzeichen dazwischen dargestellt: `""`</span><span class="sxs-lookup"><span data-stu-id="74036-p116">For read operations, expect to receive blank values if the contents of the cells are blanks. If the cell contains no data or value, the API returns a blank value. Blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

```json
{
  "values" : [["", "some", "data", "in", "other", "cells", ""]]
}
```

```json
{
  "formula" : [["", "", "=Rand()"]]
}
```


### <a name="unbounded-range"></a><span data-ttu-id="74036-257">Ungebundener Bereich</span><span class="sxs-lookup"><span data-stu-id="74036-257">Unbounded Range</span></span>

#### <a name="read"></a><span data-ttu-id="74036-258">Lesen</span><span class="sxs-lookup"><span data-stu-id="74036-258">Read</span></span>

<span data-ttu-id="74036-259">Die Adresse eines ungebundenen Bereichs enthält nur Bezeichner für die Spalte oder Zeile und nicht angegebene Zeilenbezeichner oder Spaltenbezeichner, wie etwa:</span><span class="sxs-lookup"><span data-stu-id="74036-259">Unbounded Range address contains only column or row identifiers and unspecified row identifier or column identifiers (respectively), such as:</span></span>

* <span data-ttu-id="74036-260">`C:C`, `A:F`, `A:XFD` (enthält nicht angegebene Zeilen)</span><span class="sxs-lookup"><span data-stu-id="74036-260">`C:C`, `A:F`, `A:XFD` (contains unspecified rows)</span></span>
* <span data-ttu-id="74036-261">`2:2`, `1:4`, `1:1048546` (enthält nicht angegebene Spalten)</span><span class="sxs-lookup"><span data-stu-id="74036-261">`2:2`, `1:4`, `1:1048546` (contains unspecified columns)</span></span>

<span data-ttu-id="74036-p117">Wenn die API eine Anforderung zum Abrufen eines ungebundenen Bereichs (`getRange('C:C')`) ausführt, enthält die zurückgegebene Antwort `null` für Zellenebeneneigenschaften wie `values`, `text`, `numberFormat` oder `formula`. Andere Bereichseigenschaften wie `address` oder `cellCount` spiegeln den ungebundenen Bereich wider.</span><span class="sxs-lookup"><span data-stu-id="74036-p117">When the API makes a request to retrieve an unbounded Range (`getRange('C:C')`), the response returned contains `null` for cell-level properties such as `values`, `text`, `numberFormat`, or `formula`. Other Range properties such as `address` or `cellCount` will reflect the unbounded range.</span></span>

#### <a name="write"></a><span data-ttu-id="74036-264">Schreiben</span><span class="sxs-lookup"><span data-stu-id="74036-264">Write</span></span>

<span data-ttu-id="74036-265">Das Festlegen von Eigenschaften auf Zellebene (z. B. values, numberFormat usw.) für einen ungebundenen Bereich ist **nicht zulässig**, da die Eingabeanforderung möglicherweise zu groß zum Verarbeiten ist.</span><span class="sxs-lookup"><span data-stu-id="74036-265">Setting cell level properties (such as values, numberFormat, etc.) on unbounded Range is **not allowed** because the input request might be too large to handle.</span></span>

<span data-ttu-id="74036-266">Beispiel: Folgendes ist keine gültige Aktualisierungsanforderung, da der angeforderte Bereich ungebunden ist.</span><span class="sxs-lookup"><span data-stu-id="74036-266">For example, the following is not a valid update request because the requested range is unbounded.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets('Sheet1')/range(address="A:B")

{
  "values" : "Due Date"
}
```

<span data-ttu-id="74036-267">Wenn ein Aktualisierungsvorgang für so einen Bereich ausgeführt wird, gibt die API einen Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="74036-267">When an update operation is attempted on such a Range, the API will return an error.</span></span>


### <a name="large-range"></a><span data-ttu-id="74036-268">Großer Bereich</span><span class="sxs-lookup"><span data-stu-id="74036-268">Large Range</span></span>

<span data-ttu-id="74036-p118">Ein großer Bereich impliziert einen Bereich, dessen Größe für einen einzelnen API-Aufruf zu groß ist. Viele Faktoren wie z. B. die Anzahl der Zellen, Werte, numberFormat und Formeln, die im Bereich enthalten sind, können die Antwort so groß werden lassen, dass sie zur API-Interaktion ungeeignet werden kann. Die API ermöglicht einen optimalen Versuch zum Zurückgeben oder Schreiben der angeforderten Daten. Allerdings kann die Größe aufgrund der hohen Ressourcenverwendung zu einem API-Fehlerzustand führen.</span><span class="sxs-lookup"><span data-stu-id="74036-p118">Large Range implies a Range of a size that is too large for a single API call. Many factors such as number of cells, values, numberFormat, and formulas contained in the range can make the response so large that it becomes unsuitable for API interaction. The API makes a best attempt to return or write to the requested data. However, the large size involved might result in an API error condition because of the large resource utilization.</span></span>

<span data-ttu-id="74036-273">Um dies zu vermeiden, wird empfohlen, das Lesen oder Schreiben für einen großen Bereich in mehreren kleineren Bereichsgrößen zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="74036-273">To avoid this, we recommend that you read or write for large Range in multiple smaller range sizes.</span></span>


### <a name="single-input-copy"></a><span data-ttu-id="74036-274">Einzelne Eingabekopie</span><span class="sxs-lookup"><span data-stu-id="74036-274">Single input copy</span></span>

<span data-ttu-id="74036-p119">Zur Unterstützung der Aktualisierung eines Bereichs mit denselben Werten oder demselben Zahlenformat oder des Anwendens derselben Formel für einen kompletten Bereich, wird in der Set-API folgende Konvention verwendet. In Excel ähnelt dieses Verhalten dem Eingeben von Werten oder Formeln in einen Bereich im Modus STRG + EINGABETASTE.</span><span class="sxs-lookup"><span data-stu-id="74036-p119">To support updating a range with the same values or number-format or applying same formula across a range, the following convention is used in the set API. In Excel, this behavior is similar to inputting values or formulas to a range in the CTRL+Enter mode.</span></span>

<span data-ttu-id="74036-277">Die API sucht nach einem *einzelnen Zellenwert* und wenn die Ziel-Bereichsdimension nicht mit der Eingabebereichsdimension übereinstimmt, wendet sie die Aktualisierung im STRG + EINGABE-Modell mit dem in der Anforderung bereitgestellten Wert oder der Formel auf den gesamten Bereich an.</span><span class="sxs-lookup"><span data-stu-id="74036-277">The API will look for a *single cell value* and, if the target range dimension doesn't match the input range dimension, it will apply the update to the entire range in the CTRL+Enter model with the value or formula provided in the request.</span></span>

#### <a name="examples"></a><span data-ttu-id="74036-278">Beispiele</span><span class="sxs-lookup"><span data-stu-id="74036-278">Examples</span></span>

<span data-ttu-id="74036-p120">Die folgende Anforderung aktualisiert den ausgewählten Bereich mit dem Text „Beispieltext“. Beachten Sie, dass der Bereich 200 Zellen aufweist, während die angegebene Eingabe nur einen Zellwert besitzt.</span><span class="sxs-lookup"><span data-stu-id="74036-p120">The following request updates the selected range with the text of "Sample text". Note that Range has 200 cells, whereas the provided input only has 1 cell value.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets('Sheet1')/range(address="A1:B00")

{
  "values" : "Sample text"
}
```

### <a name="workbook-functions"></a><span data-ttu-id="74036-281">Arbeitsmappenfunktionen</span><span class="sxs-lookup"><span data-stu-id="74036-281">Workbook functions</span></span> 
<span data-ttu-id="74036-282">Sie können auf die Arbeitsmappenfunktionen über eine Sammlung von Funktionen zugreifen, die in der /Functions-Ressource enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="74036-282">You can access the workbook functions through a collection of functions included in the /Functions resource.</span></span> 

<!-- LG: Where is the Functions resource? We should link to this.
-->
##### <a name="request"></a><span data-ttu-id="74036-283">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74036-283">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
https://graph.microsoft.com/v1.0/me/drive/root:/book1.xlsx:/workbook/functions/pmt
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
    "rate": 4.5,
    "nper": 12,
    "pv": -1250
}
```


##### <a name="response"></a><span data-ttu-id="74036-284">Antwort</span><span class="sxs-lookup"><span data-stu-id="74036-284">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/pmt()",
    "error": null,
    "value": 5625.00000734125
}
```

## <a name="error-information"></a><span data-ttu-id="74036-285">Informationen zu Fehlern</span><span class="sxs-lookup"><span data-stu-id="74036-285">Error information</span></span> 

<span data-ttu-id="74036-p121">Fehler werden mit einem HTTP-Fehlercode und einem Fehlerobjekt zurückgegeben. Die Fehler `code` und `message` erläutern die Ursache des Fehlers.</span><span class="sxs-lookup"><span data-stu-id="74036-p121">Errors are returned with an HTTP error code and an error object. An error `code` and `message` explain the reason for the error.</span></span>
 
<span data-ttu-id="74036-288">Es folgt ein Beispiel.</span><span class="sxs-lookup"><span data-stu-id="74036-288">The following is an example.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 400 Bad Request
Content-Type: application/json

{
  "error": {
    "code": "ItemAlreadyExists",
    "message": "A resource with the same name or identifier already exists.",
    "innerError": {
      "request-id": "214ca7ea-9ea4-442e-9c67-71fdda0a559c",
      "date": "2016-07-28T03:56:09"
    }
  }
}
```

