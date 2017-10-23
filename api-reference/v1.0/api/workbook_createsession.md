# <a name="create-session"></a><span data-ttu-id="c2031-101">Sitzung erstellen</span><span class="sxs-lookup"><span data-stu-id="c2031-101">Create Upload Session</span></span>

<span data-ttu-id="c2031-102">Verwenden Sie diese API zum Erstellen einer neuen Arbeitsmappensitzung.</span><span class="sxs-lookup"><span data-stu-id="c2031-102">Use this API to create a new plannerPlan.</span></span> 

<span data-ttu-id="c2031-103">Excel-APIs können in einem der beiden folgenden Modi aufgerufen werden:</span><span class="sxs-lookup"><span data-stu-id="c2031-103">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="c2031-p101">Beständige Sitzung: Alle an der Arbeitsmappe vorgenommenen Änderungen werden gespeichert. Dies ist die übliche Vorgehensweise.</span><span class="sxs-lookup"><span data-stu-id="c2031-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="c2031-p102">Nicht beständige Sitzung: Die von der API vorgenommenen Änderungen werden nicht am Quellspeicherort gespeichert. Stattdessen behält der Excel-Back-End-Server eine temporäre Kopie der Datei  bei, welche die während dieser API-Sitzung vorgenommenen Änderungen enthält. Wenn die Excel-Sitzung abläuft, gehen die Änderungen verloren. Dieser Modus eignet sich für Apps, die Analysen durchführen oder die Ergebnisse einer Berechnung oder eines Diagrammbilds abrufen, aber nicht den Dokumentstatus betreffen.</span><span class="sxs-lookup"><span data-stu-id="c2031-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="c2031-110">Um die Sitzung in der API darzustellen, verwenden Sie den `workbook-session-id: {session-id}`-Header.</span><span class="sxs-lookup"><span data-stu-id="c2031-110">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="c2031-p103">**Hinweis:** Der Sitzungsheader ist für das Funktionieren einer Excel-API nicht erforderlich. Die Verwendung des Sitzungsheaders wird jedoch empfohlen, um die Leistung zu verbessern. Wenn Sie keinen Sitzungsheader verwenden, _werden_ die während des API-Aufrufs vorgenommenen Änderungen in der Datei gespeichert.</span><span class="sxs-lookup"><span data-stu-id="c2031-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="permissions"></a><span data-ttu-id="c2031-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c2031-114">Permissions</span></span>
<span data-ttu-id="c2031-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c2031-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c2031-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c2031-117">Permission type</span></span>      | <span data-ttu-id="c2031-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c2031-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2031-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c2031-119">Delegated (work or school account)</span></span> | <span data-ttu-id="c2031-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2031-120">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c2031-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c2031-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2031-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2031-122">Not supported.</span></span>    |
|<span data-ttu-id="c2031-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c2031-123">Application</span></span> | <span data-ttu-id="c2031-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2031-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2031-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2031-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession

```
## <a name="request-headers"></a><span data-ttu-id="c2031-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c2031-126">Request headers</span></span>
| <span data-ttu-id="c2031-127">Name</span><span class="sxs-lookup"><span data-stu-id="c2031-127">Name</span></span>       | <span data-ttu-id="c2031-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2031-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c2031-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2031-129">Authorization</span></span>  | <span data-ttu-id="c2031-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c2031-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2031-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c2031-132">Request body</span></span>
<span data-ttu-id="c2031-133">Geben Sie im Anforderungstext eine JSON-Darstellung des [WorkbookSessionInfo](../resources/workbooksessioninfo.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c2031-133">In the request body, supply a JSON representation of [calendar](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c2031-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2031-134">Response</span></span>

<span data-ttu-id="c2031-135">Wenn die Methode erfolgreich verläuft, werden der `201, Created` Antwortcode und ein [WorkbookSessionInfo](../resources/workbooksessioninfo.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c2031-135">If successful, this method returns `201, Created` response code and the new [page](../resources/workbooksessioninfo.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2031-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c2031-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2031-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2031-137">Request</span></span>
<span data-ttu-id="c2031-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c2031-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistSession": true
}
```
<span data-ttu-id="c2031-139">Geben Sie im Anforderungstext eine JSON-Darstellung des [WorkbookSessionInfo](../resources/workbooksessioninfo.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c2031-139">In the request body, supply a JSON representation of [calendar](../resources/workbooksessioninfo.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="c2031-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2031-140">Response</span></span>
<span data-ttu-id="c2031-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c2031-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistSession": true
}
```

