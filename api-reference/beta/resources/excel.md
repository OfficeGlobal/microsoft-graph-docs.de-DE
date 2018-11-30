---
title: Arbeiten mit Excel in Microsoft Graph
description: 'Sie können Microsoft Graph verwenden, um es Web- und Mobilanwendungen zu ermöglichen, in OneDrive, SharePoint oder anderen unterstützten Speicherplattformen gespeicherte Excel-Arbeitsmappen zu lesen und zu bearbeiten. Die `Workbook`- (bzw. Excel-Datei-)Ressource enthält alle anderen Excel-Ressourcen über Beziehungen. Sie können über die Laufwerks-API auf eine Arbeitsmappe zugreifen, indem Sie den Speicherort der Datei in der URL identifizieren. Beispiel:'
ms.openlocfilehash: c5dae7620989adf4f02a8b8518a334255607b591
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063285"
---
# <a name="working-with-excel-in-microsoft-graph"></a><span data-ttu-id="23999-106">Arbeiten mit Excel in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="23999-106">Working with Excel in Microsoft Graph</span></span>

> <span data-ttu-id="23999-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23999-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23999-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23999-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23999-p103">Sie können Microsoft Graph verwenden, um es Web- und Mobilanwendungen zu ermöglichen, in OneDrive, SharePoint oder anderen unterstützten Speicherplattformen gespeicherte Excel-Arbeitsmappen zu lesen und zu bearbeiten. Die `Workbook`- (bzw. Excel-Datei-)Ressource enthält alle anderen Excel-Ressourcen über Beziehungen. Sie können über die [Laufwerks-API](drive.md) auf eine Arbeitsmappe zugreifen, indem Sie den Speicherort der Datei in der URL identifizieren. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="23999-p103">You can use Microsoft Graph to allow web and mobile applications to read and modify Excel workbooks stored in OneDrive, SharePoint, or other supported storage platforms. The `Workbook` (or Excel file) resource contains all the other Excel resources through relationships. You can access a workbook through the [Drive API](drive.md) by identifying the location of the file in the URL. For example:</span></span>

`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`  
`https://graph.microsoft.com/{version}/me/drive/root:/{item-path}:/workbook/`  

<span data-ttu-id="23999-p104">Sie können auf eine Reihe von Excel-Objekten (wie Tabelle, Bereich oder Diagramm) mithilfe von standardmäßigen REST-APIs zugreifen, um Vorgänge zum Erstellen, Lesen, Aktualisieren und Löschen in der Abeitsmappe durchzuführen. Beispielsweise gibt `https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`</span><span class="sxs-lookup"><span data-stu-id="23999-p104">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, `https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`</span></span>  
<span data-ttu-id="23999-115">eine Sammlung von Arbeitsblattobjekten zurück, die Teil der Arbeitsmappe sind.</span><span class="sxs-lookup"><span data-stu-id="23999-115">returns a collection of worksheet objects that are part of the workbook.</span></span>    


<span data-ttu-id="23999-p105">**Hinweis:** Die Excel-REST-API unterstützt nur Arbeitsmappen im Office Open XML-Dateiformat. Arbeitsmappen mit der Erweiterung `.xls` werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23999-p105">**Note:** The Excel REST API supports only Office Open XML file formatted workbooks. The `.xls` extension workbooks are not supported.</span></span> 

## <a name="authorization-and-scopes"></a><span data-ttu-id="23999-118">Autorisierung und Bereiche</span><span class="sxs-lookup"><span data-stu-id="23999-118">Authorization and scopes</span></span>

<span data-ttu-id="23999-p106">Sie können den [Azure AD v.20-Endpunkt](https://developer.microsoft.com/graph/docs/authorization/converged_auth) verwenden, um Excel-APIs zu authentifizieren. Alle APIs benötigen den `Authorization: Bearer {access-token}`-HTTP-Header.</span><span class="sxs-lookup"><span data-stu-id="23999-p106">You can use the [Azure AD v.20 endpoint](https://developer.microsoft.com/graph/docs/authorization/converged_auth) to authenticate Excel APIs. All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="23999-121">Einer der folgenden [Berechtigungsbereiche](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) ist erforderlich, um die Excel-Ressource verwenden:</span><span class="sxs-lookup"><span data-stu-id="23999-121">One of the following [permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to use the Excel resource:</span></span>

* <span data-ttu-id="23999-122">Files.Read</span><span class="sxs-lookup"><span data-stu-id="23999-122">Files.Read</span></span> 
* <span data-ttu-id="23999-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23999-123">Files.ReadWrite</span></span>


## <a name="sessions-and-persistence"></a><span data-ttu-id="23999-124">Sitzungen und Beständigkeit</span><span class="sxs-lookup"><span data-stu-id="23999-124">Sessions and persistence</span></span>

<span data-ttu-id="23999-125">Excel-APIs können in einem der beiden folgenden Modi aufgerufen werden:</span><span class="sxs-lookup"><span data-stu-id="23999-125">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="23999-p107">Beständige Sitzung: Alle an der Arbeitsmappe vorgenommenen Änderungen werden gespeichert. Dies ist die übliche Vorgehensweise.</span><span class="sxs-lookup"><span data-stu-id="23999-p107">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="23999-p108">Nicht beständige Sitzung: Die von der API vorgenommenen Änderungen werden nicht am Quellspeicherort gespeichert. Stattdessen behält der Excel-Back-End-Server eine temporäre Kopie der Datei  bei, welche die während dieser API-Sitzung vorgenommenen Änderungen enthält. Wenn die Excel-Sitzung abläuft, gehen die Änderungen verloren. Dieser Modus eignet sich für Apps, die Analysen durchführen oder die Ergebnisse einer Berechnung oder eines Diagrammbilds abrufen, aber nicht den Dokumentstatus betreffen.</span><span class="sxs-lookup"><span data-stu-id="23999-p108">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="23999-132">Um die Sitzung in der API darzustellen, verwenden Sie den `workbook-session-id: {session-id}`-Header.</span><span class="sxs-lookup"><span data-stu-id="23999-132">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="23999-p109">**Hinweis:** Der Sitzungsheader ist für das Funktionieren einer Excel-API nicht erforderlich. Die Verwendung des Sitzungsheaders wird jedoch empfohlen, um die Leistung zu verbessern. Wenn Sie keinen Sitzungsheader verwenden, _werden_ die während des API-Aufrufs vorgenommenen Änderungen in der Datei gespeichert.</span><span class="sxs-lookup"><span data-stu-id="23999-p109">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

### <a name="api-call-to-get-a-session"></a><span data-ttu-id="23999-136">API-Aufruf, um eine Sitzung aufzurufen</span><span class="sxs-lookup"><span data-stu-id="23999-136">API call to get a session</span></span> 

#### <a name="request"></a><span data-ttu-id="23999-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23999-137">Request</span></span> 

<span data-ttu-id="23999-138">Übergeben Sie ein JSON-Objekt durch Festlegen des `persistchanges`-Wert auf `true` oder `false`.</span><span class="sxs-lookup"><span data-stu-id="23999-138">Pass a JSON object by setting the `persistchanges` value to `true` or `false`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/createSession
content-type: Application/Json 
authorization: Bearer {access-token}

{ "persistChanges": true }
```

<span data-ttu-id="23999-139">Wenn der Wert auf `persistChanges` oder `false` festgelegt wird, wird eine nicht beständige Sitzungs-ID zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23999-139">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span>  


#### <a name="response"></a><span data-ttu-id="23999-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="23999-140">Response</span></span>

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

#### <a name="usage"></a><span data-ttu-id="23999-141">Verwendung</span><span class="sxs-lookup"><span data-stu-id="23999-141">Usage</span></span> 

<span data-ttu-id="23999-142">Die vom vorherigen Aufruf zurückgegebene Sitzungs-ID wird als Header in nachfolgenden API-Anforderungen im</span><span class="sxs-lookup"><span data-stu-id="23999-142">The session ID returned from the previous call is passed as a header on subsequent API requests in</span></span>  
<span data-ttu-id="23999-143">`workbook-session-id`-HTTP-Header dargestellt.</span><span class="sxs-lookup"><span data-stu-id="23999-143">`workbook-session-id` HTTP header.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

><span data-ttu-id="23999-144">Hinweis: Wenn die Sitzungs-ID abgelaufen ist, wird ein `404` HTTP-Fehlercode an die Sitzung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23999-144">Note: If the session id has expired, a `404` HTTP error code is returned on the session.</span></span> <span data-ttu-id="23999-145">In einem solchen Szenario können Sie eine neue Sitzung erstellen und fortfahren.</span><span class="sxs-lookup"><span data-stu-id="23999-145">In such a scenarion, you can choose to create a new session and continue.</span></span> <span data-ttu-id="23999-146">Sie können aber auch die Sitzung regelmäßig aktualisieren, damit die Sitzung erhalten bleibt.</span><span class="sxs-lookup"><span data-stu-id="23999-146">Another approach would be to refresh the session periodically to keep the session alive.</span></span> <span data-ttu-id="23999-147">In der Regel läuft eine beständige Sitzung nach ca. 7 Minuten Inaktivität ab.</span><span class="sxs-lookup"><span data-stu-id="23999-147">Typically the persistent session expires after about 7 minutes of inactivity.</span></span> <span data-ttu-id="23999-148">Eine nicht beständige Sitzung läuft nach ca. 5 Minuten Inaktivität ab.</span><span class="sxs-lookup"><span data-stu-id="23999-148">Non persistent session expires after about 5 minutes of inactivity.</span></span> 

## <a name="common-excel-scenarios"></a><span data-ttu-id="23999-149">Häufige Excel-Szenarien</span><span class="sxs-lookup"><span data-stu-id="23999-149">Common Excel scenarios</span></span>

<span data-ttu-id="23999-150">Dieser Abschnitt enthält Beispiele für häufige Vorgänge,die Sie für Excel-Objekte verwenden können.</span><span class="sxs-lookup"><span data-stu-id="23999-150">This section provides examples of the common operations you can use on Excel objects.</span></span>

### <a name="worksheet-operations"></a><span data-ttu-id="23999-151">Arbeitsblattvorgänge</span><span class="sxs-lookup"><span data-stu-id="23999-151">Worksheet operations</span></span>

#### <a name="list-worksheets-part-of-the-workbook"></a><span data-ttu-id="23999-152">Den Arbeitsblätterteil der Arbeitsmappe auflisten</span><span class="sxs-lookup"><span data-stu-id="23999-152">List worksheets part of the workbook</span></span> 
<span data-ttu-id="23999-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23999-153">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="23999-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="23999-154">Response</span></span>

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
#### <a name="add-a-new-worksheet"></a><span data-ttu-id="23999-155">Neues Arbeitsblatt hinzufügen</span><span class="sxs-lookup"><span data-stu-id="23999-155">Add a new worksheet</span></span> 
 
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "Sheet32243" }
```

<span data-ttu-id="23999-156">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-156">Response <!-- { "blockType": "ignored" } --></span></span>
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

#### <a name="get-a-new-worksheet"></a><span data-ttu-id="23999-157">Neues Arbeitsblatt abrufen</span><span class="sxs-lookup"><span data-stu-id="23999-157">Get a new worksheet</span></span> 
 
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/Sheet32243
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="23999-158">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-158">Response <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="23999-p111">\*\* Hinweis: Arbeitsblätter können auch mit der ID abgerufen werden. Derzeit enthält die ID jedoch die Zeichen `{` und „}“, für die eine URL-Codierung durchgeführt werden muss, damit die API funktioniert. Beispiel: Um ein Arbeitsblatt mit der ID `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}` abzurufen, führen Sie für die ID im Pfad die folgende URL-Codierung durch: `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span><span class="sxs-lookup"><span data-stu-id="23999-p111">\*\* Note: Worksheets can also be retrieved using the ID. However, currently the ID contains `{` and '}' characters, which needs to be URL encoded for the API to work. Example: In order to get a worksheet with ID of `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, URL encode the ID in the path as `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span></span> 

#### <a name="delete-a-worksheet"></a><span data-ttu-id="23999-162">Arbeitsblatt löschen</span><span class="sxs-lookup"><span data-stu-id="23999-162">Delete a worksheet</span></span>

<span data-ttu-id="23999-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23999-163">Request</span></span>
```
DELETE /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="23999-164">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-164">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```


#### <a name="update-worksheet-properties"></a><span data-ttu-id="23999-165">Arbeitsblatteigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="23999-165">Update worksheet properties</span></span>

<span data-ttu-id="23999-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23999-166">Request</span></span> 

```
PATCH /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/SheetA
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "SheetA", "position": 3 }
```

<span data-ttu-id="23999-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="23999-167">Response</span></span>

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

### <a name="chart-operations"></a><span data-ttu-id="23999-168">Diagrammvorgänge</span><span class="sxs-lookup"><span data-stu-id="23999-168">Chart operations</span></span>

#### <a name="list-charts-that-are-part-of-the-worksheet"></a><span data-ttu-id="23999-169">Diagramme auflisten, die Teil des Arbeitsblatts sind</span><span class="sxs-lookup"><span data-stu-id="23999-169">List charts that are part of the worksheet</span></span> 

<span data-ttu-id="23999-170">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-170">Request <!-- { "blockType": "ignored" } --></span></span>
```http 
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="23999-171">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-171">Response <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="23999-p112">\*\* Hinweis: Die Diagramm-ID enthält die Zeichen `{` und `}` (Beispiel: `{00000000-0008-0000-0100-000003000000}`), für die eine URL-Codierung durchgeführt werden muss, damit die API funktioniert. Beispiel: Um ein Diagrammobjekt abzurufen, führen Sie für die ID im Pfad die folgende URL-Codierung durch: `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span><span class="sxs-lookup"><span data-stu-id="23999-p112">\*\* Note: Chart ID contains `{` and `}` characters (example: `{00000000-0008-0000-0100-000003000000}`), which needs to be URL encoded for the API to work. Example: In order to get a chart object, URL encode the ID in the path as `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span></span> 

#### <a name="get-chart-image"></a><span data-ttu-id="23999-174">Diagrammbild abrufen</span><span class="sxs-lookup"><span data-stu-id="23999-174">Get chart image</span></span>

<span data-ttu-id="23999-175">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-175">Request <!-- { "blockType": "ignored" } --></span></span>
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B00000000-0008-0000-0100-000003000000%7D')/Image(width=0,height=0,fittingMode='fit')
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="23999-176">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-176">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#Edm.String",
  "value": "{base-64-string}"
}
```

#### <a name="add-a-chart"></a><span data-ttu-id="23999-177">Diagramm hinzufügen</span><span class="sxs-lookup"><span data-stu-id="23999-177">Add a chart</span></span>  

<span data-ttu-id="23999-178">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23999-178">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/Add
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 

{ "type": "ColumnClustered", "sourcedata": "A1:C4", "seriesby": "Auto" }
```

<span data-ttu-id="23999-179">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-179">Response <!-- { "blockType": "ignored" } --></span></span>
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

#### <a name="update-a-chart"></a><span data-ttu-id="23999-180">Diagramm aktualisieren</span><span class="sxs-lookup"><span data-stu-id="23999-180">Update a chart</span></span>

<!-- { "blockType": "ignored" } -->
```http 
PATCH /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "height": 216.0, "left": 0, "name": "NewName", "top": 0, "width": 360.0 }

```
<span data-ttu-id="23999-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="23999-181">Response</span></span> 

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

#### <a name="update-chart-source-data"></a><span data-ttu-id="23999-182">Quelldaten des Diagramms aktualisieren</span><span class="sxs-lookup"><span data-stu-id="23999-182">Update chart source data</span></span> 

<span data-ttu-id="23999-183">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-183">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')/setData
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "sourceData": "A1:C4", "seriesBy": "Auto" }
```

<span data-ttu-id="23999-184">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-184">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

### <a name="table-operations"></a><span data-ttu-id="23999-185">Tabellenvorgänge</span><span class="sxs-lookup"><span data-stu-id="23999-185">Table operations</span></span> 

#### <a name="get-list-of-tables"></a><span data-ttu-id="23999-186">Liste der Tabellen abrufen</span><span class="sxs-lookup"><span data-stu-id="23999-186">Get list of tables</span></span> 

<span data-ttu-id="23999-187">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-187">Request <!-- { "blockType": "ignored" } --></span></span>
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/tables
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="23999-188">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-188">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 
```

#### <a name="create-table"></a><span data-ttu-id="23999-189">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="23999-189">Create table</span></span>

<span data-ttu-id="23999-190">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-190">Request <!-- { "blockType": "ignored" } --></span></span>
```http 
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables/$/add
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "hasHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="23999-191">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-191">Response <!-- { "blockType": "ignored" } --></span></span>
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

#### <a name="update-table"></a><span data-ttu-id="23999-192">Tabelle aktualisieren</span><span class="sxs-lookup"><span data-stu-id="23999-192">Update table</span></span>

<span data-ttu-id="23999-193">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-193">Request <!-- { "blockType": "ignored" } --></span></span>
```http 
PATCH /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "showHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="23999-194">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-194">Response <!-- { "blockType": "ignored" } --></span></span>
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

#### <a name="get-list-of-table-rows"></a><span data-ttu-id="23999-195">Liste der Tabellenzeilen abrufen</span><span class="sxs-lookup"><span data-stu-id="23999-195">Get list of table rows</span></span>
<span data-ttu-id="23999-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23999-196">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="23999-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="23999-197">Response</span></span>

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

#### <a name="get-list-of-table-columns"></a><span data-ttu-id="23999-198">Liste der Tabellenspalten abrufen</span><span class="sxs-lookup"><span data-stu-id="23999-198">Get list of table columns</span></span>

<span data-ttu-id="23999-199">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-199">Request <!-- { "blockType": "ignored" } --></span></span>
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Columns
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="23999-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="23999-200">Response</span></span> 

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


#### <a name="add-a-table-row"></a><span data-ttu-id="23999-201">Tabellenzeile hinzufügen</span><span class="sxs-lookup"><span data-stu-id="23999-201">Add a table row</span></span>

<span data-ttu-id="23999-202">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-202">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Jan-15-2016", "49", "37" ] ], "index": null }
```

<span data-ttu-id="23999-203">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-203">Response <!-- { "blockType": "ignored" } --></span></span>
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

#### <a name="add-a-table-column"></a><span data-ttu-id="23999-204">Tabellenspalte hinzufügen</span><span class="sxs-lookup"><span data-stu-id="23999-204">Add a table column</span></span> 

<span data-ttu-id="23999-205">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-205">Request <!-- { "blockType": "ignored" } --></span></span>
```http 
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')/Columns
content-type: Application/Json 
accept: application/Json 


{ "values": [ [ "Status" ], [ "Open" ], [ "Closed" ] ], "index": 2 }
```

<span data-ttu-id="23999-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="23999-206">Response</span></span> 

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

#### <a name="delete-table-row"></a><span data-ttu-id="23999-207">Tabellenzeile löschen</span><span class="sxs-lookup"><span data-stu-id="23999-207">Delete table row</span></span>

<span data-ttu-id="23999-208">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-208">Request <!-- { "blockType": "ignored" } --></span></span>
```http  
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows/$/ItemAt(index=6)
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="23999-209">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-209">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

#### <a name="delete-table-column"></a><span data-ttu-id="23999-210">Tabellenspalte löschen</span><span class="sxs-lookup"><span data-stu-id="23999-210">Delete table column</span></span> 
<span data-ttu-id="23999-211">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-211">Request <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Columns('3')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="23999-212">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-212">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

#### <a name="convert-table-to-range"></a><span data-ttu-id="23999-213">Tabelle in Bereich konvertieren</span><span class="sxs-lookup"><span data-stu-id="23999-213">Convert table to range</span></span> 
<span data-ttu-id="23999-214">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-214">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('1')/convertToRange
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="23999-215">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-215">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 
```

#### <a name="table-sort"></a><span data-ttu-id="23999-216">Tabelle sortieren</span><span class="sxs-lookup"><span data-stu-id="23999-216">Table sort</span></span>
<span data-ttu-id="23999-217">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-217">Request <!-- { "blockType": "ignored" } --></span></span>
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


<span data-ttu-id="23999-218">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-218">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

#### <a name="table-filter"></a><span data-ttu-id="23999-219">Tabelle filtern</span><span class="sxs-lookup"><span data-stu-id="23999-219">Table filter</span></span>
<span data-ttu-id="23999-220">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-220">Request <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="23999-221">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-221">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```


#### <a name="clear-filter"></a><span data-ttu-id="23999-222">Filter löschen</span><span class="sxs-lookup"><span data-stu-id="23999-222">Clear filter</span></span>
<span data-ttu-id="23999-223">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-223">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/clear
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="23999-224">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-224">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

### <a name="range-operations"></a><span data-ttu-id="23999-225">Bereichsvorgänge</span><span class="sxs-lookup"><span data-stu-id="23999-225">Range operations</span></span>

#### <a name="get-range"></a><span data-ttu-id="23999-226">Bereich abrufen</span><span class="sxs-lookup"><span data-stu-id="23999-226">Get Range</span></span> 

<span data-ttu-id="23999-227">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-227">Request <!-- { "blockType": "ignored" } --></span></span>
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/worksheets('test')/range(address='A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="23999-228">Antwort</span><span class="sxs-lookup"><span data-stu-id="23999-228">Response</span></span> 

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

#### <a name="range-update"></a><span data-ttu-id="23999-229">Bereich aktualisieren</span><span class="sxs-lookup"><span data-stu-id="23999-229">Range update</span></span> 

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

#### <a name="range-sort"></a><span data-ttu-id="23999-230">Bereich sortieren</span><span class="sxs-lookup"><span data-stu-id="23999-230">Range sort</span></span>
<span data-ttu-id="23999-231">Anforderung<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-231">Request <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="23999-232">Antwort<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="23999-232">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```


### <a name="named-items"></a><span data-ttu-id="23999-233">Benannte Elemente</span><span class="sxs-lookup"><span data-stu-id="23999-233">Named items</span></span>
<span data-ttu-id="23999-234">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23999-234">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/names
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="23999-235">Antwort</span><span class="sxs-lookup"><span data-stu-id="23999-235">Response</span></span> 

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

### <a name="work-with-nulls"></a><span data-ttu-id="23999-236">Verwenden von Daten</span><span class="sxs-lookup"><span data-stu-id="23999-236">Work with nulls</span></span>

#### <a name="null-input-in-2-d-array"></a><span data-ttu-id="23999-237">NULL-Eingabe im 2D-Array</span><span class="sxs-lookup"><span data-stu-id="23999-237">null input in 2-D array</span></span>

<span data-ttu-id="23999-p113">Die `null`-Eingabe in einem zweidimensionalen Array (für Werte, Zahlenformate, Formeln) wird in den Bereichs- und Tabellenressourcen ignoriert. Am beabsichtigten Ziel (Zelle) findet keine Aktualisierung statt, wenn die `null`-Eingabe in Werten, im Zahlenformat oder Formelraster von Werten gesendet wird.</span><span class="sxs-lookup"><span data-stu-id="23999-p113">`null` input inside a two-dimensional array (for values, number-format, formula) is ignored in the Range and Table resources. No update will take place to the intended target (cell) when `null` input is sent in values or number-format or formula grid of values.</span></span>

<span data-ttu-id="23999-240">Um nur bestimmte Teile des Bereichs zu aktualisieren, wie z. B. das Zahlenformat einer Zelle, und das vorhandene Zahlenformat in anderen Teilen des Bereichs beizubehalten, legen Sie das gewünschte Zahlenformat an entsprechender Stelle fest und senden Sie `null` für die anderen Zellen.</span><span class="sxs-lookup"><span data-stu-id="23999-240">For example, to only update specific parts of the Range, such as a cell's Number Format, and to retain the existing number-format on other parts of the Range, set the Number Format where needed and send `null` for the other cells.</span></span>

<span data-ttu-id="23999-241">In der folgenden Set-Anforderung werden nur einige Teile des Bereichszahlenformats festgelegt, dabei wird das vorhandene Zahlenformat im verbleibenden Teil beibehalten (durch NULL-Übergabe).</span><span class="sxs-lookup"><span data-stu-id="23999-241">In the following set request, only some parts of the Range Number Format are set while the existing Number Format on the remaining part is retained (by passing nulls).</span></span>

```json
{
  "values" : [["Eurasia", "29.96", "0.25", "15-Feb" ]],
  "numberFormat" : [[null, null, null, "m/d/yyyy;@"]]
}
```

#### <a name="null-input-for-a-property"></a><span data-ttu-id="23999-242">NULL-Eingabe für eine Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23999-242">null input for a property</span></span>

<span data-ttu-id="23999-p114">`null` ist keine gültige einzelne Eingabe für die gesamte Eigenschaft. Folgende Eingabe ist beispielsweise ungültig, da die gesamten Werte nicht auf NULL festgelegt oder ignoriert werden können.</span><span class="sxs-lookup"><span data-stu-id="23999-p114">`null` is not a valid single input for the entire property. For example, the following is not valid because the entire values cannot be set to null or ignored.</span></span>

```json
{
"values":  null
}

```

<span data-ttu-id="23999-245">Folgendes ist ebenfalls nicht gültig, da NULL kein gültiger Farbwert ist.</span><span class="sxs-lookup"><span data-stu-id="23999-245">The following is not valid either as null is not a valid color value.</span></span>

```json
{
"color" :  null
}
```

#### <a name="null-response"></a><span data-ttu-id="23999-246">NULL-Antwort</span><span class="sxs-lookup"><span data-stu-id="23999-246">Null-Response</span></span>

<span data-ttu-id="23999-247">Darstellungen der Formatierungseigenschaften, die aus ungleichmäßigen Werten bestehen, ergeben einen NULL-Wert in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="23999-247">Representation of formatting properties that consists of non-uniform values results in the return of a null value in the response.</span></span>

<span data-ttu-id="23999-p115">So kann z. B. ein Bereich aus einer oder mehreren Zellen bestehen. In Fällen, in denen die im angegebenen Bereich enthaltenen einzelnen Zellen keine gleichmäßigen Formatierungswerte enthalten, wird die Bereichsebenendarstellung undefiniert.</span><span class="sxs-lookup"><span data-stu-id="23999-p115">For example, a Range can consist of one or more cells. In cases where the individual cells contained in the Range specified don't have uniform formatting values, the range level representation will be undefined.</span></span>

```json
{
  "size: : null,
  "color" : null
}
```


### <a name="blank-input-and-output"></a><span data-ttu-id="23999-250">Leere Eingabe und Ausgabe</span><span class="sxs-lookup"><span data-stu-id="23999-250">Blank input and output</span></span>

<span data-ttu-id="23999-p116">Leere Werte in Aktualisierungsanforderungen werden als Anweisung behandelt, um die entsprechende Eigenschaft zu löschen oder zurückzusetzen. Ein leerer Wert wird durch zwei doppelte Anführungszeichen ohne Leerzeichen dazwischen dargestellt: `""`</span><span class="sxs-lookup"><span data-stu-id="23999-p116">Blank values in update requests are treated as an instruction to clear or reset the respective property. A blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

<span data-ttu-id="23999-253">Beispiele:</span><span class="sxs-lookup"><span data-stu-id="23999-253">Examples:</span></span>

* <span data-ttu-id="23999-254">Für `values` wird der Bereichswert gelöscht. Das ist genauso wie das Löschen des Inhalts in der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="23999-254">For `values`, the range value is cleared out. This is the same as clearing the contents in the application.</span></span>

* <span data-ttu-id="23999-255">Für `numberFormat` wird das Zahlenformat auf `General` festgelegt.</span><span class="sxs-lookup"><span data-stu-id="23999-255">For `numberFormat`, the number format is set to `General`.</span></span>

* <span data-ttu-id="23999-256">Für `formula` und `formulaLocale` werden die Formelwerte gelöscht.</span><span class="sxs-lookup"><span data-stu-id="23999-256">For `formula` and `formulaLocale`, the formula values are cleared.</span></span>


<span data-ttu-id="23999-p117">Für Lesevorgänge können Sie leere Werte erwarten, wenn der Inhalt der Zellen leer ist. Wenn die Zelle keine Daten oder keinen Wert enthält, gibt die API einen leeren Wert zurück. Ein leerer Wert wird durch zwei doppelte Anführungszeichen ohne Leerzeichen dazwischen dargestellt: `""`</span><span class="sxs-lookup"><span data-stu-id="23999-p117">For read operations, expect to receive blank values if the contents of the cells are blanks. If the cell contains no data or value, the API returns a blank value. Blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

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


### <a name="unbounded-range"></a><span data-ttu-id="23999-260">Ungebundener Bereich</span><span class="sxs-lookup"><span data-stu-id="23999-260">Unbounded Range</span></span>

#### <a name="read"></a><span data-ttu-id="23999-261">Lesen</span><span class="sxs-lookup"><span data-stu-id="23999-261">Read</span></span>

<span data-ttu-id="23999-262">Die Adresse eines ungebundenen Bereichs enthält nur Bezeichner für die Spalte oder Zeile und nicht angegebene Zeilenbezeichner oder Spaltenbezeichner, wie etwa:</span><span class="sxs-lookup"><span data-stu-id="23999-262">Unbounded Range address contains only column or row identifiers and unspecified row identifier or column identifiers (respectively), such as:</span></span>

* <span data-ttu-id="23999-263">`C:C`, `A:F`, `A:XFD` (enthält nicht angegebene Zeilen)</span><span class="sxs-lookup"><span data-stu-id="23999-263">`C:C`, `A:F`, `A:XFD` (contains unspecified rows)</span></span>
* <span data-ttu-id="23999-264">`2:2`, `1:4`, `1:1048546` (enthält nicht angegebene Spalten)</span><span class="sxs-lookup"><span data-stu-id="23999-264">`2:2`, `1:4`, `1:1048546` (contains unspecified columns)</span></span>

<span data-ttu-id="23999-p118">Wenn die API eine Anforderung zum Abrufen eines ungebundenen Bereichs (`getRange('C:C')`) ausführt, enthält die zurückgegebene Antwort `null` für Zellenebeneneigenschaften wie `values`, `text`, `numberFormat` oder `formula`. Andere Bereichseigenschaften wie `address` oder `cellCount` spiegeln den ungebundenen Bereich wider.</span><span class="sxs-lookup"><span data-stu-id="23999-p118">When the API makes a request to retrieve an unbounded Range (`getRange('C:C')`), the response returned contains `null` for cell-level properties such as `values`, `text`, `numberFormat`, or `formula`. Other Range properties such as `address` or `cellCount` will reflect the unbounded range.</span></span>

#### <a name="write"></a><span data-ttu-id="23999-267">Schreiben</span><span class="sxs-lookup"><span data-stu-id="23999-267">Write</span></span>

<span data-ttu-id="23999-268">Das Festlegen von Eigenschaften auf Zellebene (z. B. values, numberFormat usw.) für einen ungebundenen Bereich ist **nicht zulässig**, da die Eingabeanforderung möglicherweise zu groß zum Verarbeiten ist.</span><span class="sxs-lookup"><span data-stu-id="23999-268">Setting cell level properties (such as values, numberFormat, etc.) on unbounded Range is **not allowed** because the input request might be too large to handle.</span></span>

<span data-ttu-id="23999-269">Beispiel: Folgendes ist keine gültige Aktualisierungsanforderung, da der angeforderte Bereich ungebunden ist.</span><span class="sxs-lookup"><span data-stu-id="23999-269">For example, the following is not a valid update request because the requested range is unbounded.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets('Sheet1')/range(address="A:B")

{
  "values" : "Due Date"
}
```

<span data-ttu-id="23999-270">Wenn ein Aktualisierungsvorgang für so einen Bereich ausgeführt wird, gibt die API einen Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="23999-270">When an update operation is attempted on such a Range, the API will return an error.</span></span>


### <a name="large-range"></a><span data-ttu-id="23999-271">Großer Bereich</span><span class="sxs-lookup"><span data-stu-id="23999-271">Large Range</span></span>

<span data-ttu-id="23999-p119">Ein großer Bereich impliziert einen Bereich, dessen Größe für einen einzelnen API-Aufruf zu groß ist. Viele Faktoren wie z. B. die Anzahl der Zellen, Werte, numberFormat und Formeln, die im Bereich enthalten sind, können die Antwort so groß werden lassen, dass sie zur API-Interaktion ungeeignet werden kann. Die API ermöglicht einen optimalen Versuch zum Zurückgeben oder Schreiben der angeforderten Daten. Allerdings kann die Größe aufgrund der hohen Ressourcenverwendung zu einem API-Fehlerzustand führen.</span><span class="sxs-lookup"><span data-stu-id="23999-p119">Large Range implies a Range of a size that is too large for a single API call. Many factors such as number of cells, values, numberFormat, and formulas contained in the range can make the response so large that it becomes unsuitable for API interaction. The API makes a best attempt to return or write to the requested data. However, the large size involved might result in an API error condition because of the large resource utilization.</span></span>

<span data-ttu-id="23999-276">Um dies zu vermeiden, wird empfohlen, das Lesen oder Schreiben für einen großen Bereich in mehreren kleineren Bereichsgrößen zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="23999-276">To avoid this, we recommend that you read or write for large Range in multiple smaller range sizes.</span></span>


### <a name="single-input-copy"></a><span data-ttu-id="23999-277">Einzelne Eingabekopie</span><span class="sxs-lookup"><span data-stu-id="23999-277">Single input copy</span></span>

<span data-ttu-id="23999-p120">Zur Unterstützung der Aktualisierung eines Bereichs mit denselben Werten oder demselben Zahlenformat oder des Anwendens derselben Formel für einen kompletten Bereich, wird in der Set-API folgende Konvention verwendet. In Excel ähnelt dieses Verhalten dem Eingeben von Werten oder Formeln in einen Bereich im Modus STRG + EINGABETASTE.</span><span class="sxs-lookup"><span data-stu-id="23999-p120">To support updating a range with the same values or number-format or applying same formula across a range, the following convention is used in the set API. In Excel, this behavior is similar to inputting values or formulas to a range in the CTRL+Enter mode.</span></span>

<span data-ttu-id="23999-280">Die API sucht nach einem *einzelnen Zellenwert* und wenn die Ziel-Bereichsdimension nicht mit der Eingabebereichsdimension übereinstimmt, wendet sie die Aktualisierung im STRG + EINGABE-Modell mit dem in der Anforderung bereitgestellten Wert oder der Formel auf den gesamten Bereich an.</span><span class="sxs-lookup"><span data-stu-id="23999-280">The API will look for a *single cell value* and, if the target range dimension doesn't match the input range dimension, it will apply the update to the entire range in the CTRL+Enter model with the value or formula provided in the request.</span></span>

#### <a name="examples"></a><span data-ttu-id="23999-281">Beispiele</span><span class="sxs-lookup"><span data-stu-id="23999-281">Examples</span></span>

<span data-ttu-id="23999-p121">Die folgende Anforderung aktualisiert den ausgewählten Bereich mit dem Text „Beispieltext“. Beachten Sie, dass der Bereich 200 Zellen aufweist, während die angegebene Eingabe nur einen Zellwert besitzt.</span><span class="sxs-lookup"><span data-stu-id="23999-p121">The following request updates the selected range with the text of "Sample text". Note that Range has 200 cells, whereas the provided input only has 1 cell value.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets('Sheet1')/range(address="A1:B00")

{
  "values" : "Sample text"
}
```

### <a name="workbook-functions"></a><span data-ttu-id="23999-284">Arbeitsmappenfunktionen</span><span class="sxs-lookup"><span data-stu-id="23999-284">Workbook functions</span></span> 
<span data-ttu-id="23999-285">Sie können auf die Arbeitsmappenfunktionen über eine Sammlung von Funktionen zugreifen, die in der /Functions-Ressource enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="23999-285">You can access the workbook functions through a collection of functions included in the /Functions resource.</span></span> 

<!-- LG: Where is the Functions resource? We should link to this.
-->
##### <a name="request"></a><span data-ttu-id="23999-286">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23999-286">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/pmt
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
    "rate": 4.5,
    "nper": 12,
    "pv": -1250
}
```


##### <a name="response"></a><span data-ttu-id="23999-287">Antwort</span><span class="sxs-lookup"><span data-stu-id="23999-287">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/pmt()",
    "error": null,
    "value": 5625.00000734125
}
```

## <a name="error-information"></a><span data-ttu-id="23999-288">Informationen zu Fehlern</span><span class="sxs-lookup"><span data-stu-id="23999-288">Error information</span></span> 

<span data-ttu-id="23999-p122">Fehler werden mit einem HTTP-Fehlercode und einem Fehlerobjekt zurückgegeben. Die Fehler `code` und `message` erläutern die Ursache des Fehlers.</span><span class="sxs-lookup"><span data-stu-id="23999-p122">Errors are returned with an HTTP error code and an error object. An error `code` and `message` explain the reason for the error.</span></span>
 
<span data-ttu-id="23999-291">Es folgt ein Beispiel.</span><span class="sxs-lookup"><span data-stu-id="23999-291">The following is an example.</span></span>

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

