<span data-ttu-id="f3d3a-p101">Obwohl das [**SharedDriveItem**](../resources/shareddriveitem.md)-Element nützliche Informationen enthält, möchten die meisten Apps direkt auf das freigegebene [DriveItem](../resources/driveitem.md)-Element zugreifen. Die **SharedDriveItem**-Ressource umfasst **root**- und **items**-Beziehungen, die innerhalb des Bereichs des freigegebenen Elements auf die Inhalte zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="f3d3a-p101">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

Obwohl das [**SharedDriveItem**](../resources/shareddriveitem.md)-Element nützliche Informationen enthält, möchten die meisten Apps direkt auf das freigegebene [DriveItem](../resources/driveitem.md)-Element zugreifen. Die **SharedDriveItem**-Ressource umfasst **root**- und **items**-Beziehungen, die innerhalb des Bereichs des freigegebenen Elements auf die Inhalte zugreifen können.

### <span data-ttu-id="f3d3a-122">Beispiel (einzelne Datei)</span><span class="sxs-lookup"><span data-stu-id="f3d3a-122">Example (single file)</span></span>
<a id="example-single-file" class="xliff"></a>

##### <span data-ttu-id="f3d3a-123">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3d3a-123">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="f3d3a-124">Durch das Anfordern der **root**-Beziehung wird das **DriveItem**-Element zurückgegeben, das freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="f3d3a-124">By requesting the **root** relationship, the **DriveItem** that was shared will be returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root
```

##### <span data-ttu-id="f3d3a-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3d3a-125">Response</span></span>
<a id="response" class="xliff"></a>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

### <span data-ttu-id="f3d3a-126">Beispiel (freigegebener Ordner)</span><span class="sxs-lookup"><span data-stu-id="f3d3a-126">Example (shared folder)</span></span>
<a id="example-shared-folder" class="xliff"></a>

##### <span data-ttu-id="f3d3a-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3d3a-127">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="f3d3a-128">Durch das Anfordern der **root**-Beziehung und das Erweitern der **children**-Sammlung wird das freigegebene **DriveItem**-Element mit Dateien im freigegebenen Ordner zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3d3a-128">By requesting the **root** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root?$expand=children
```

##### <span data-ttu-id="f3d3a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3d3a-129">Response</span></span>
<a id="response" class="xliff"></a>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {}
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <span data-ttu-id="f3d3a-130">Konvertieren einer Freigabe-URL</span><span class="sxs-lookup"><span data-stu-id="f3d3a-130">Transform a sharing URL</span></span>
<a id="transform-a-sharing-url" class="xliff"></a>

<span data-ttu-id="f3d3a-131">Um auf eine Freigabe-URL unter Verwendung der **shares**-API zuzugreifen, muss die URL in ein Freigabetoken umgewandelt werden.</span><span class="sxs-lookup"><span data-stu-id="f3d3a-131">To access a sharing URL using the **shares** API, the URL needs to be transformed into a sharing token.</span></span>

<span data-ttu-id="f3d3a-132">So wandeln Sie eine URL in ein Freigabetoken um:</span><span class="sxs-lookup"><span data-stu-id="f3d3a-132">To transform a URL into a sharing token:</span></span>

1. <span data-ttu-id="f3d3a-133">Codieren Sie die URL-Freigabe mithilfe von Base64.</span><span class="sxs-lookup"><span data-stu-id="f3d3a-133">Base64 encode the sharing URL.</span></span>
2. <span data-ttu-id="f3d3a-134">Konvertieren Sie die Base64-codierten Daten in das [base64url-Format ohne Füllzeichen](https://en.wikipedia.org/wiki/Base64), indem Sie folgende Aktionen durchführen:</span><span class="sxs-lookup"><span data-stu-id="f3d3a-134">Convert the base64 encoded data to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by:</span></span>
  1. <span data-ttu-id="f3d3a-135">Kürzen Sie nachgestellte `=`-Zeichen in der Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f3d3a-135">Trim trailing `=` characters from the string</span></span>
  2. <span data-ttu-id="f3d3a-136">Ersetzen Sie unsichere URL-Zeichen mit einem entsprechenden Zeichen; ersetzen Sie `/` mit `_` und `+` mit `-`.</span><span class="sxs-lookup"><span data-stu-id="f3d3a-136">Replace unsafe URL characters with an equivalent character; replace `/` with `_` and `+` with `-`.</span></span>
3. <span data-ttu-id="f3d3a-137">Fügen Sie `u!` an den Anfang der Zeichenfolge an.</span><span class="sxs-lookup"><span data-stu-id="f3d3a-137">Append `u!` to the beginning of the string.</span></span>

<span data-ttu-id="f3d3a-138">Mit der folgenden C#-Methode wird beispielsweise eine Eingabezeichenfolge in eine Freigabetoken konvertiert:</span><span class="sxs-lookup"><span data-stu-id="f3d3a-138">For example, the following C# method transforms an input string into a sharing token:</span></span>

```csharp
string UrlToSharingToken(string inputUrl) {
  var base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(inputUrl));
  return "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
