# <a name="upload-large-files-with-an-upload-session"></a><span data-ttu-id="de2bd-101">Hochladen großer Dateien mit einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="de2bd-101">Upload large files with an upload session</span></span>

<span data-ttu-id="de2bd-p101">Wenn Sie eine Uploadsitzung erstellen, kann Ihre App Dateien bis zur maximal zulässigen Dateigröße hochladen. Eine Uploadsitzung erlaubt es der App, Bereiche einer Datei in sequenziellen API-Anfragen hochzuladen. Bricht die Verbindung während des Uploads ab, kann die Übertragung so anschließend fortgesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p101">Create an upload session to allow your app to upload files up to the maximum file size. An upload session allows your app to upload ranges of the file in sequental API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="de2bd-104">Sie müssen zwei Schritte durchführen, um eine Datei mit einer Uploadsitzung hochzuladen:</span><span class="sxs-lookup"><span data-stu-id="de2bd-104">To upload a file using an upload session, there are two steps:</span></span>

1. [<span data-ttu-id="de2bd-105">Erstellen einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="de2bd-105">Create an upload session</span></span>](#create-an-upload-session)
2. [<span data-ttu-id="de2bd-106">Hochladen von Bytes in die Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="de2bd-106">Upload bytes to the upload session</span></span>](#upload-bytes-to-the-upload-session)

## <a name="permissions"></a><span data-ttu-id="de2bd-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="de2bd-107">Permissions</span></span>
<span data-ttu-id="de2bd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="de2bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="de2bd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="de2bd-110">Permission type</span></span>      | <span data-ttu-id="de2bd-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="de2bd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de2bd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="de2bd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="de2bd-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de2bd-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="de2bd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="de2bd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de2bd-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de2bd-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="de2bd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="de2bd-116">Application</span></span> | <span data-ttu-id="de2bd-117">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de2bd-117">Sites.ReadWrite.All</span></span> |

> <span data-ttu-id="de2bd-p103">**Hinweis**: Die Anwendungsberechtigung „Files.ReadWrite.All“ wird für diese API noch nicht unterstützt. Vollständige Unterstützung soll in Kürze folgen.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p103">**Note**: The Files.ReadWrite.All application permission is not yet supported on this API. Full support is planned soon.</span></span> 

## <a name="create-an-upload-session"></a><span data-ttu-id="de2bd-120">Erstellen einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="de2bd-120">Create an upload session</span></span>

<span data-ttu-id="de2bd-p104">Um eine große Datei hochladen zu können, muss die App zuerst eine neue Uploadsitzung anfordern. Es wird dann ein temporärer Speicherort erstellt, an dem die Bytes der Datei gespeichert werden, bis sie vollständig hochgeladen ist. Sobald das letzte Byte der Datei hochgeladen wurde, ist die Uploadsitzung abgeschlossen, und die endgültige Datei wird im Zielordner angezeigt.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p104">To begin a large file upload, your app must first request a new upload session. This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded. Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>

### <a name="http-request"></a><span data-ttu-id="de2bd-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="de2bd-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root:/{path-to-item}:/createUploadSession
POST /me/drive/items/{parent-item-id}:/{filename}:/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="de2bd-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="de2bd-125">Request body</span></span>
<span data-ttu-id="de2bd-p105">Es ist kein Anforderungstexts erforderlich. Allerdings können Sie einen Anforderungstext definieren, um zusätzliche Daten zu der hochzuladenden Datei anzugeben.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p105">No request body is required. However, you can specify a request body to provide additional data about the file being uploaded.</span></span>

<span data-ttu-id="de2bd-128">Beispielsweise können Sie im Anforderungstext die Eigenschaft „conflictBehavior“ definieren, um festzulegen, wie vorgegangen werden soll, wenn der Dateiname bereits anderweitig in Verwendung ist.</span><span class="sxs-lookup"><span data-stu-id="de2bd-128">For example, to control the behavior if the filename is already taken, you can specify the conflict behavior property in the body of the request.</span></span>

```json
{
    "item": {
        "@microsoft.graph.conflictBehavior": "rename"
    }
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="de2bd-129">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="de2bd-129">Optional request headers</span></span>

| <span data-ttu-id="de2bd-130">Name</span><span class="sxs-lookup"><span data-stu-id="de2bd-130">Name</span></span>       | <span data-ttu-id="de2bd-131">Wert</span><span class="sxs-lookup"><span data-stu-id="de2bd-131">Value</span></span> | <span data-ttu-id="de2bd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de2bd-132">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="de2bd-133">*if-match*</span><span class="sxs-lookup"><span data-stu-id="de2bd-133">*if-match*</span></span> | <span data-ttu-id="de2bd-134">etag</span><span class="sxs-lookup"><span data-stu-id="de2bd-134">etag</span></span>  | <span data-ttu-id="de2bd-135">Wenn dieser Anforderungsheader enthalten ist und das angegebene Etag (oder CTag) nicht mit dem aktuellen Etag des Elements übereinstimmt, wird der Fehler `412 Precondition Failed` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de2bd-135">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` errr response is returned.</span></span> |

### <a name="response"></a><span data-ttu-id="de2bd-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="de2bd-136">Response</span></span>
<span data-ttu-id="de2bd-137">Die Antwort auf diese Anforderung enthält die Details der neu erstellten Ressource des Typs [uploadSession](../resources/uploadsession.md), einschließlich der zum Upload der Dateiteile verwendeten URL.</span><span class="sxs-lookup"><span data-stu-id="de2bd-137">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

### <a name="example"></a><span data-ttu-id="de2bd-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de2bd-138">Example</span></span>

<!-- {
  "blockType": "request",
  "name": "driveItem_createUploadSession"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createUploadSession
```

##### <a name="response"></a><span data-ttu-id="de2bd-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="de2bd-139">Response</span></span> 

<span data-ttu-id="de2bd-140">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="de2bd-140">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://tenant-my.sharepoint.com/alkjl1kjklna",
  "expirationDateTime": "2020-08-24T10:58:00Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="de2bd-141">Hochladen von Bytes in die Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="de2bd-141">Upload bytes to the upload session</span></span>

<span data-ttu-id="de2bd-p106">Zum Hochladen der Datei oder eines Teils der Datei sendet die App eine PUT-Anfrage an den Wert **uploadUrl**, der ihr in der **createUploadSession**-Antwort übermittelt wurde. Sie können die gesamte Datei hochladen oder die Datei in Fragmente aufteilen, vorausgesetzt, die maximale Bytezahl pro Anforderung bleibt unter 60 MiB. Die Dateifragmente müssen sequenziell in der richtigen Reihenfolge hochgeladen werden. Werden die Fragmente in der falschen Reihenfolge hochgeladen, tritt ein Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p106">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response. You can upload the entire file, or split the file into fragments, as long as the maximum bytes in any given request is less than 60 MiB. The fragments of the file must be uploaded sequentally in order. Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="de2bd-p107">**Hinweis:** Wenn die App eine Datei in mehrere Fragmente aufteilt, **MUSS** die Größe jedes Fragments ein Vielfaches von 320 KiB sein. Bei Fragmentgrößen, die sich nicht ohne Rest durch 320 teilen lassen, treten beim Commit einiger Dateien Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p107">**Note:** If your app splits a file into multiple fragments, the size of each fragment **MUST** be a multiple of 320 KiB. Using a fragment size that does not divide evenly by 320 will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="de2bd-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de2bd-148">Example</span></span>

<span data-ttu-id="de2bd-p108">In diesem Beispiel werden die ersten 26 Byte einer 128-Byte-Datei hochgeladen. Der Header **Content-Length** definiert die Größe der aktuellen Anforderung. Der Header **Content-Range** gibt den Bytebereich in der Gesamtdatei an, den diese Anforderung repräsentiert. Die Gesamtlänge der Datei muss bekannt sein, bevor Sie das erste Fragment der Datei hochladen können.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p108">This example is uploading the first 26 bytes of a 128 byte file. The **Content-Length** header specifies the size of the current request. The **Content-Range** header indicates the range of bytes in the overall file that this request represents. The total length of the file must be known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="de2bd-p109">**Wichtig:** Die App muss sicherstellen, dass die im Header **Content-Range** angegebene Gesamtdateigröße bei allen Anforderungen identisch ist. Wird für ein Fragment eine andere Dateigröße deklariert, schlägt die betreffende Anforderung fehl.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p109">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests. If a fragment declares a different file size, the request will fail.</span></span>

##### <a name="response"></a><span data-ttu-id="de2bd-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="de2bd-155">Response</span></span>

<span data-ttu-id="de2bd-156">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="de2bd-156">The following example shows the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="de2bd-p110">Die App kann mithilfe des Werts **nextExpectedRanges** bestimmen, wo das nächste Fragment beginnen soll. Eventuell werden mehrere Bereichen angegeben. Sie stehen für Teile der Datei, die der Server noch nicht empfangen hat. Dies ist nützlich, wenn eine Übertragung nach einer Unterbrechung fortgesetzt werden soll und der Client den Dienststatus nicht kennt.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p110">Your app can use the **nextExpectedRanges** value to determine where to start the next fragment. You may see multiple ranges specified, indicating parts of the file that the server has not yet received. This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="de2bd-p111">Halten Sie sich bei der Festlegung der Fragmentgröße immer an die unten beschriebenen bewährten Methoden. Gehen Sie nicht davon aus, dass **nextExpectedRanges** richtig dimensionierte Bereiche für ein Uploadfragment zurückgeben wird. Die Eigenschaft **nextExpectedRanges** gibt Dateibereiche an, die noch nicht empfangen wurden. Sie ist nicht als Muster für den Dateiupload zu verstehen.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p111">You should always determine the fragment size according to the best practices below. Do not assume that **nextExpectedRanges** will return reanges of proper size for an upload fragment. The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how you should upload the file.</span></span>

<span data-ttu-id="de2bd-163">**Hinweise:**</span><span class="sxs-lookup"><span data-stu-id="de2bd-163">**Notes:**</span></span>

* <span data-ttu-id="de2bd-164">Die Eigenschaft `nextExpectedRanges` listet nicht immer alle fehlenden Bereiche auf.</span><span class="sxs-lookup"><span data-stu-id="de2bd-164">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="de2bd-p112">Wird ein Segment geschrieben, gibt sie den nächsten Bereich zurück, ab dem begonnen wird (z. B. „523-“).</span><span class="sxs-lookup"><span data-stu-id="de2bd-p112">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="de2bd-p113">Schlägt der Schreibvorgang fehl, weil der Client ein Fragment gesendet hat, das der Server bereits empfangen hat, antwortet der Server mit `HTTP 416 Requested Range Not Satisfiable`. Sie können den [Uploadstatus anfordern](#resuming-an-in-progress-upload), um eine detailliertere Liste der fehlenden Bereiche zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p113">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="de2bd-p114">Wenn Sie den Autorisierungsheader in den `PUT`-Aufruf einschließen, wird möglicherweise eine Antwort des Typs `HTTP 401 Unauthorized` zurückgegeben. Der Autorisierungsheader und das Bearertoken sollten nur mit dem `POST`-Aufruf im Rahmen von Schritt 1 gesendet werden. Der Autorisierungsheader sollte nicht in den `PUT`-Aufruf eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p114">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthorized` response. The Authorization header and bearer token should only be sent when issuing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>   


## <a name="completing-a-file"></a><span data-ttu-id="de2bd-172">Vervollständigen einer Datei</span><span class="sxs-lookup"><span data-stu-id="de2bd-172">Completing a file</span></span>

<span data-ttu-id="de2bd-p115">Sobald der Server das letzte Fragment einer Datei empfängt, antwortet er mit `HTTP 201 Created` oder `HTTP 200 OK`. Der Antworttext enthält auch die Standardeigenschaft, die für das **DriveItem** festgelegt wurde, das die vervollständigte Datei repräsentiert.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p115">When the last fragment of a file is received the server will response with an `HTTP 201 Created` or `HTTP 200 OK`. The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-final", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
Content-Length: 21
Content-Range: bytes 101-127/128

<final bytes of the file>
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```
<span data-ttu-id="de2bd-175">**Hinweis:** Die Elementantwort ist aus Gründen der Dokumentationsübersichtlichkeit abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="de2bd-175">**Note:** The item response is truncated for documentation clarity.</span></span>

## <a name="cancel-an-upload-session"></a><span data-ttu-id="de2bd-176">Abbrechen einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="de2bd-176">Cancel an upload session</span></span>

<span data-ttu-id="de2bd-p116">Wenn Sie eine Uploadsitzung abbrechen möchten, senden Sie eine DELETE-Anforderung an die Upload-URL. Das bereinigt die temporäre Datei, in der die bisher hochgeladenen Daten gespeichert sind. Verwenden Sie diese Vorgehensweise in Szenarios, in denen der Upload abgebrochen wird, beispielsweise bei Abbruch der Übertragung durch den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p116">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="de2bd-180">Temporäre Dateien und die zugehörigen Uploadsitzungen werden automatisch bereinigt, wenn der über **expirationDateTime** festgelegte Termin abgelaufen ist.</span><span class="sxs-lookup"><span data-stu-id="de2bd-180">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>

### <a name="example"></a><span data-ttu-id="de2bd-181">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de2bd-181">Example</span></span>

<span data-ttu-id="de2bd-182">Die DELETE-Anforderung führt zum sofortigen Ablauf der Uploadsitzung und entfernt alle zuvor hochgeladenen Bytes.</span><span class="sxs-lookup"><span data-stu-id="de2bd-182">The DELETE request will immedately expire the upload session and remove any previously uploaded bytes.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->
```http
DELETE https://tenant-my.sharepoint.com/alkjl1kjklna
```

##### <a name="response"></a><span data-ttu-id="de2bd-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="de2bd-183">Response</span></span> 

<span data-ttu-id="de2bd-184">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="de2bd-184">The following example shows the response.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="de2bd-185">Fortsetzen eines laufenden Uploads</span><span class="sxs-lookup"><span data-stu-id="de2bd-185">Resuming an in-progress upload</span></span>

<span data-ttu-id="de2bd-p117">Wenn während einer Uploadanforderung die Verbindung getrennt wird oder anderweitig ausfällt, bevor die Anforderung abgeschlossen ist, werden alle Bytes in dieser Anforderung ignoriert. Dies kann passieren, wenn die Verbindung zwischen der App und dem Dienst getrennt wird. Tritt ein solcher Fall ein, kann die App die Dateiübertragung trotzdem ab dem letzten vollständig übertragenen Fragment fortsetzen.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p117">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="de2bd-189">Um herauszufinden, welche Bytebereiche bereits empfangen wurden, kann die App den Status der Uploadsitzung anfordern.</span><span class="sxs-lookup"><span data-stu-id="de2bd-189">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="de2bd-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de2bd-190">Example</span></span>
<span data-ttu-id="de2bd-191">Sie können den Status des Uploads anfragen, indem Sie eine GET-Anforderung an `uploadUrl` senden.</span><span class="sxs-lookup"><span data-stu-id="de2bd-191">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->
```
GET https://tenant-my.sharepoint.com/alkjl1kjklna
```

<span data-ttu-id="de2bd-192">Der Server antwortet mit einer Liste der fehlenden Bytebereiche, die noch hochgeladen werden müssen, sowie mit dem Ablauftermin der Uploadsitzung.</span><span class="sxs-lookup"><span data-stu-id="de2bd-192">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 200 OK

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="de2bd-193">Hochladen von verbleibenden Daten</span><span class="sxs-lookup"><span data-stu-id="de2bd-193">Upload remaining data</span></span>
<span data-ttu-id="de2bd-194">Die App weiß jetzt, ab wo der Upload gestartet werden soll. Führen Sie nun die Schritte im Abschnitt [Hochladen von Bytes in die Uploadsitzung](#upload-bytes-to-the-upload-session) durch, um den Upload fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="de2bd-194">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>


## <a name="best-practices"></a><span data-ttu-id="de2bd-195">Bewährte Methoden</span><span class="sxs-lookup"><span data-stu-id="de2bd-195">Best practices</span></span>

* <span data-ttu-id="de2bd-196">Setzen Sie alle Uploads fort bzw. starten Sie alle Uploads neu, die wegen eines Verbindungsabbruchs oder einem 5xx-Fehler fehlschlagen, beispielsweise:</span><span class="sxs-lookup"><span data-stu-id="de2bd-196">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="de2bd-197">Verwenden Sie einen Exponential Backoff-Algorithmus, wenn beim Fortsetzen oder Neusenden einer Uploadanforderung 5xx-Serverfehler auftreten.</span><span class="sxs-lookup"><span data-stu-id="de2bd-197">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="de2bd-198">Bei anderen Fehlern sollten Sie keinen Exponential Backoff-Algorithmus verwenden, sondern stattdessen die Anzahl der Wiederholungsversuche beschränken.</span><span class="sxs-lookup"><span data-stu-id="de2bd-198">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="de2bd-199">Sollte bei fortsetzbaren Uploads der Fehler `404 Not Found` auftreten, starten Sie den gesamten Upload neu.</span><span class="sxs-lookup"><span data-stu-id="de2bd-199">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span>
* <span data-ttu-id="de2bd-200">Verwenden Sie fortsetzbare Dateiübertragungen für Dateien, die größer als 10 MiB sind (10 \* 1.024 \* 1.024 Byte).</span><span class="sxs-lookup"><span data-stu-id="de2bd-200">Use resumable file transfers for files larger than 10 MiB (10 \* 1024 \* 1024 bytes).</span></span>
* <span data-ttu-id="de2bd-p118">Die optimale Dateigröße für stabile Highspeedverbindungen ist 10 MiB. Bei langsameren oder weniger zuverlässigen Verbindungen liefern kleinere Fragmentgrößen eventuell bessere Ergebnisse. Die empfohlene Fragmentgröße liegt zwischen 5 und 10 MiB.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p118">A fragment size of 10 MiB for stable high speed connections is optimal. For slower or less reliable connections you may get better results from a smaller fragment size. The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="de2bd-p119">Verwenden Sie eine Fragmentgröße, die ein Vielfaches von 320 KiB ist (320 \* 1.024 Byte). Wenn Sie eine Fragmentgröße verwenden, die kein Vielfaches von 320 KiB ist, können Übertragungen großer Dateien nach Upload des letzten Fragments fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="de2bd-p119">Use a fragment size that is a multiple of 320 KiB (320 \* 1024 bytes). Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last fragment is uploaded.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
