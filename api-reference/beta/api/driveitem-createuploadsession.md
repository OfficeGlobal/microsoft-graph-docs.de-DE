---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Wiederaufnehmbarer Dateien-Upload
ms.openlocfilehash: 09f76b4427df446b2f063827029473a11dba6341
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058746"
---
# <a name="upload-large-files-with-an-upload-session"></a><span data-ttu-id="4b297-102">Hochladen großer Dateien mit einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="4b297-102">Upload large files with an upload session</span></span>

> <span data-ttu-id="4b297-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4b297-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b297-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b297-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b297-p102">Wenn Sie eine Uploadsitzung erstellen, kann Ihre App Dateien bis zur maximal zulässigen Dateigröße hochladen. Eine Uploadsitzung erlaubt es der App, Bereiche einer Datei in sequenziellen API-Anfragen hochzuladen. Bricht die Verbindung während des Uploads ab, kann die Übertragung so anschließend fortgesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="4b297-p102">Create an upload session to allow your app to upload files up to the maximum file size. An upload session allows your app to upload ranges of the file in sequential API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="4b297-107">Sie müssen zwei Schritte durchführen, um eine Datei mit einer Uploadsitzung hochzuladen:</span><span class="sxs-lookup"><span data-stu-id="4b297-107">To upload a file using an upload session, there are two steps:</span></span>

1. [<span data-ttu-id="4b297-108">Erstellen einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="4b297-108">Create an upload session</span></span>](#create-an-upload-session)
2. [<span data-ttu-id="4b297-109">Hochladen von Bytes in die Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="4b297-109">Upload bytes to the upload session</span></span>](#upload-bytes-to-the-upload-session)

## <a name="permissions"></a><span data-ttu-id="4b297-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4b297-110">Permissions</span></span>

<span data-ttu-id="4b297-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b297-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b297-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b297-113">Permission type</span></span>      | <span data-ttu-id="4b297-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b297-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b297-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b297-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4b297-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b297-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b297-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b297-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b297-118">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b297-118">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b297-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b297-119">Application</span></span> | <span data-ttu-id="4b297-120">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b297-120">Sites.ReadWrite.All</span></span> |

## <a name="create-an-upload-session"></a><span data-ttu-id="4b297-121">Erstellen einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="4b297-121">Create an upload session</span></span>

<span data-ttu-id="4b297-122">Um eine große Dateien hochladen beginnen, muss Ihre app zunächst eine neue Sitzung Upload anfordern.</span><span class="sxs-lookup"><span data-stu-id="4b297-122">To begin a large file upload, your app must first request a new upload session.</span></span>
<span data-ttu-id="4b297-123">Dadurch wird einen temporärer Speicherort, in dem die Bytes der Datei gespeichert wird, bis die vollständige Datei hochgeladen wurde, erstellt.</span><span class="sxs-lookup"><span data-stu-id="4b297-123">This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded.</span></span>
<span data-ttu-id="4b297-124">Nachdem das letzte Byte der Datei hochgeladen wurde die Sitzung Upload abgeschlossen ist, und die endgültige Datei wird im Zielordner angezeigt.</span><span class="sxs-lookup"><span data-stu-id="4b297-124">Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>
<span data-ttu-id="4b297-125">Alternativ können Sie letzten Erstellung der Datei im Ziel zurückstellen, bis Sie explizit stellen Sie eine Anforderung zum Abschließen der Hochladevorgang durch Festlegen der `deferCommit` -Eigenschaft in der Argumente der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b297-125">Alternatively, you can defer final creation of the file in the destination until you explicitly make a request to complete the upload, by setting the `deferCommit` property in the request arguments.</span></span>

### <a name="http-request"></a><span data-ttu-id="4b297-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b297-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="4b297-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b297-127">Request body</span></span>

<span data-ttu-id="4b297-128">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4b297-128">No request body is required.</span></span>
<span data-ttu-id="4b297-129">Sie können jedoch Eigenschaften im Textkörper Anforderung zusätzliche Daten über die hochgeladene Datei bereitstellen und Anpassen der Semantik des Vorgangs hochladen angeben.</span><span class="sxs-lookup"><span data-stu-id="4b297-129">However, you can specify properties in the request body providing additional data about the file being uploaded and customizing the semantics of the upload operation.</span></span>

<span data-ttu-id="4b297-130">Beispielsweise die `item` -Eigenschaft können die folgenden Parameter festlegen:<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } --></span><span class="sxs-lookup"><span data-stu-id="4b297-130">For example, the `item` property allows setting the following parameters: <!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } --></span></span>
```json
{
  "@microsoft.graph.conflictBehavior": "rename | fail | overwrite",
  "description": "description",
  "name": "filename.txt"
}
```

<span data-ttu-id="4b297-131">Im folgende Beispiel steuert das Verhalten, wenn der Dateiname bereits vergeben ist und auch gibt an, dass die endgültige Datei nicht erstellt werden soll, bis eine explizite Abschluss angefordert wird:</span><span class="sxs-lookup"><span data-stu-id="4b297-131">The following example controls the behavior if the filename is already taken, and also specifies that the final file should not be created until an explicit completion request is made:</span></span>

<!-- { "blockType": "ignored" } -->
```json
{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename"
  },
  "deferCommit": true
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="4b297-132">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b297-132">Optional request headers</span></span>

| <span data-ttu-id="4b297-133">Name</span><span class="sxs-lookup"><span data-stu-id="4b297-133">Name</span></span>       | <span data-ttu-id="4b297-134">Wert</span><span class="sxs-lookup"><span data-stu-id="4b297-134">Value</span></span> | <span data-ttu-id="4b297-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b297-135">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4b297-136">*if-match*</span><span class="sxs-lookup"><span data-stu-id="4b297-136">*if-match*</span></span> | <span data-ttu-id="4b297-137">etag</span><span class="sxs-lookup"><span data-stu-id="4b297-137">etag</span></span>  | <span data-ttu-id="4b297-138">Wenn dieser Anforderungsheader enthalten ist und das angegebene Etag (oder CTag) nicht mit dem aktuellen Etag des Elements übereinstimmt, wird der Fehler `412 Precondition Failed` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b297-138">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` error response is returned.</span></span> |

## <a name="parameters"></a><span data-ttu-id="4b297-139">Parameter</span><span class="sxs-lookup"><span data-stu-id="4b297-139">Parameters</span></span>

| <span data-ttu-id="4b297-140">Parameter</span><span class="sxs-lookup"><span data-stu-id="4b297-140">Parameter</span></span>            | <span data-ttu-id="4b297-141">Typ</span><span class="sxs-lookup"><span data-stu-id="4b297-141">Type</span></span>                          | <span data-ttu-id="4b297-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b297-142">Description</span></span>
|:---------------------|:------------------------------|:---------------------------------
| <span data-ttu-id="4b297-143">item</span><span class="sxs-lookup"><span data-stu-id="4b297-143">item</span></span>                 | <span data-ttu-id="4b297-144">driveItemUploadableProperties</span><span class="sxs-lookup"><span data-stu-id="4b297-144">driveItemUploadableProperties</span></span> | <span data-ttu-id="4b297-145">Daten zu der hochzuladenden Datei</span><span class="sxs-lookup"><span data-stu-id="4b297-145">Data about the file being uploaded</span></span>
| <span data-ttu-id="4b297-146">deferCommit</span><span class="sxs-lookup"><span data-stu-id="4b297-146">deferCommit</span></span>          | <span data-ttu-id="4b297-147">Boolesch</span><span class="sxs-lookup"><span data-stu-id="4b297-147">Boolean</span></span>                       | <span data-ttu-id="4b297-148">Wenn es sich bei Festlegung auf "true", endgültige Erstellen der Datei im Ziel eine explizite Anforderung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="4b297-148">If set to true, final creation of the file in the destination will require an explicit request.</span></span> <span data-ttu-id="4b297-149">Nur für OneDrive für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="4b297-149">Only on OneDrive for Business.</span></span>

## <a name="item-properties"></a><span data-ttu-id="4b297-150">Elementeigenschaften</span><span class="sxs-lookup"><span data-stu-id="4b297-150">Item properties</span></span>

| <span data-ttu-id="4b297-151">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b297-151">Property</span></span>             | <span data-ttu-id="4b297-152">Typ</span><span class="sxs-lookup"><span data-stu-id="4b297-152">Type</span></span>               | <span data-ttu-id="4b297-153">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b297-153">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="4b297-154">description</span><span class="sxs-lookup"><span data-stu-id="4b297-154">description</span></span>          | <span data-ttu-id="4b297-155">String</span><span class="sxs-lookup"><span data-stu-id="4b297-155">String</span></span>             | <span data-ttu-id="4b297-156">Enthält eine Benutzer sichtbaren Beschreibung des Elements.</span><span class="sxs-lookup"><span data-stu-id="4b297-156">Provides a user-visible description of the item.</span></span> <span data-ttu-id="4b297-157">Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="4b297-157">Read-write.</span></span> <span data-ttu-id="4b297-158">Nur auf OneDrive persönlich.</span><span class="sxs-lookup"><span data-stu-id="4b297-158">Only on OneDrive Personal.</span></span>
| <span data-ttu-id="4b297-159">name</span><span class="sxs-lookup"><span data-stu-id="4b297-159">name</span></span>                 | <span data-ttu-id="4b297-160">String</span><span class="sxs-lookup"><span data-stu-id="4b297-160">String</span></span>             | <span data-ttu-id="4b297-p108">Der Name des Elements (Dateiname und Erweiterung). Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="4b297-p108">The name of the item (filename and extension). Read-write.</span></span>

### <a name="request"></a><span data-ttu-id="4b297-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b297-163">Request</span></span>

<span data-ttu-id="4b297-164">Die Antwort auf diese Anforderung enthält die Details der neu erstellten Ressource des Typs [uploadSession](../resources/uploadsession.md), einschließlich der zum Upload der Dateiteile verwendeten URL.</span><span class="sxs-lookup"><span data-stu-id="4b297-164">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

<!-- { "blockType": "request", "name": "upload-fragment-create-session", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drive/root:/{item-path}:/createUploadSession
Content-Type: application/json

{
  "item": {
    "@odata.type": "microsoft.graph.driveItemUploadableProperties",
    "@microsoft.graph.conflictBehavior": "rename",
    "name": "largefile.dat"
  }
}
```

### <a name="response"></a><span data-ttu-id="4b297-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b297-165">Response</span></span>

<span data-ttu-id="4b297-166">Wenn der Vorgang erfolgreich war, liefert die Antwort auf diese Anforderung die Details dazu, wohin die verbleibenden Anforderungen als [UploadSession](../resources/uploadsession.md)-Ressource gesendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4b297-166">The response to this request, if successful, will provide the details for where the remainder of the requests should be sent as an [UploadSession](../resources/uploadsession.md) resource.</span></span>

<span data-ttu-id="4b297-167">Diese Ressource gibt Details zu dem Ort an, an dem der Bytebereich hochgeladen werden sollte und wann die Uploadsitzung abläuft.</span><span class="sxs-lookup"><span data-stu-id="4b297-167">This resource provides details about where the byte range of the file should be uploaded and when the upload session expires.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession",
       "optionalProperties": [ "nextExpectedRanges" ]  } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z"
}
```

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="4b297-168">Hochladen von Bytes in die Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="4b297-168">Upload bytes to the upload session</span></span>

<span data-ttu-id="4b297-169">Zum Hochladen der Datei oder eines Teils der Datei sendet die App eine PUT-Anfrage an den Wert **uploadUrl**, der ihr in der **createUploadSession**-Antwort übermittelt wurde.</span><span class="sxs-lookup"><span data-stu-id="4b297-169">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>
<span data-ttu-id="4b297-170">Sie können die gesamte Datei hochladen oder die Datei in Fragmente aufteilen, vorausgesetzt, die maximale Bytezahl pro Anforderung bleibt unter 60 MiB.</span><span class="sxs-lookup"><span data-stu-id="4b297-170">You can upload the entire file, or split the file into multiple byte ranges, as long as the maximum bytes in any given request is less than 60 MiB.</span></span>

<span data-ttu-id="4b297-171">Die Fragmente der Datei müssen in Reihenfolge nacheinander hochgeladen werden.</span><span class="sxs-lookup"><span data-stu-id="4b297-171">The fragments of the file must be uploaded sequentially in order.</span></span>
<span data-ttu-id="4b297-172">Werden die Fragmente in der falschen Reihenfolge hochgeladen, tritt ein Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="4b297-172">Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="4b297-173">**Hinweis:** Wenn die App eine Datei in mehrere Fragmente aufteilt, **MUSS** die Größe jedes Fragments ein Vielfaches von 320 KiB (327.680 Byte) sein.</span><span class="sxs-lookup"><span data-stu-id="4b297-173">**Note:** If your app splits a file into multiple byte ranges, the size of each byte range **MUST** be a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="4b297-174">Bei Fragmentgrößen, die sich nicht ohne Rest durch 320 KiB teilen lassen, treten beim Übergeben einiger Dateien Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="4b297-174">Using a fragment size that does not divide evenly by 320 KiB will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="4b297-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b297-175">Example</span></span>

<span data-ttu-id="4b297-176">In diesem Beispiel lädt die App die ersten 26 Byte einer 128-Byte-Datei hoch.</span><span class="sxs-lookup"><span data-stu-id="4b297-176">In this example, the app is uploading the first 26 bytes of a 128 byte file.</span></span>

* <span data-ttu-id="4b297-177">Der Header **Content-Length** definiert die Größe der aktuellen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b297-177">The **Content-Length** header specifies the size of the current request.</span></span>
* <span data-ttu-id="4b297-178">Der Header **Content-Range** gibt den Bytebereich in der Gesamtdatei an, den diese Anforderung repräsentiert.</span><span class="sxs-lookup"><span data-stu-id="4b297-178">The **Content-Range** header indicates the range of bytes in the overall file that this request represents.</span></span>
* <span data-ttu-id="4b297-179">Die Gesamtlänge der Datei muss bekannt sein, bevor Sie das erste Fragment der Datei hochladen können.</span><span class="sxs-lookup"><span data-stu-id="4b297-179">The total length of the file is known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="4b297-180">**Wichtig:** Die App muss sicherstellen, dass die im Header **Content-Range** angegebene Gesamtdateigröße bei allen Anforderungen identisch ist.</span><span class="sxs-lookup"><span data-stu-id="4b297-180">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests.</span></span>
<span data-ttu-id="4b297-181">Wird für einen Bytebereich eine andere Dateigröße deklariert, schlägt die betreffende Anforderung fehl.</span><span class="sxs-lookup"><span data-stu-id="4b297-181">If a byte range declares a different file size, the request will fail.</span></span>

### <a name="response"></a><span data-ttu-id="4b297-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b297-182">Response</span></span>

<span data-ttu-id="4b297-183">Wenn die Anforderung abgeschlossen ist, antwortet der Server mit `202 Accepted`, wenn es weitere Bytebereiche, die hochgeladen werden müssen.</span><span class="sxs-lookup"><span data-stu-id="4b297-183">When the request is complete, the server will respond with `202 Accepted` if there are more byte ranges that need to be uploaded.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="4b297-184">Die App kann mithilfe des Werts **nextExpectedRanges** bestimmen, wo der nächste Bytebereich beginnen soll.</span><span class="sxs-lookup"><span data-stu-id="4b297-184">Your app can use the **nextExpectedRanges** value to determine where to start the next byte range.</span></span>
<span data-ttu-id="4b297-185">Eventuell werden mehrere Bereiche angegeben. Sie stehen für Teile der Datei, die der Server noch nicht empfangen hat.</span><span class="sxs-lookup"><span data-stu-id="4b297-185">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="4b297-186">Dies ist nützlich, wenn eine Übertragung nach einer Unterbrechung fortgesetzt werden soll und der Client den Dienststatus nicht kennt.</span><span class="sxs-lookup"><span data-stu-id="4b297-186">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="4b297-187">Halten Sie sich bei der Festlegung der Größe der Bytebereiche immer an die unten beschriebenen bewährten Methoden.</span><span class="sxs-lookup"><span data-stu-id="4b297-187">You should always determine the size of your byte ranges according to the best practices below.</span></span> <span data-ttu-id="4b297-188">Gehen Sie nicht davon aus, dass **nextExpectedRanges** richtig dimensionierte Bytebereiche für einen Upload zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="4b297-188">Do not assume that **nextExpectedRanges** will return reanges of proper size for a byte range to upload.</span></span>
<span data-ttu-id="4b297-189">Die Eigenschaft **nextExpectedRanges** gibt Dateibereiche an, die noch nicht empfangen wurden. Sie ist nicht als Muster für den Dateiupload der App zu verstehen.</span><span class="sxs-lookup"><span data-stu-id="4b297-189">The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how your app should upload the file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": [
  "12345-55232",
  "77829-99375"
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="4b297-190">Hinweise</span><span class="sxs-lookup"><span data-stu-id="4b297-190">Remarks</span></span>

* <span data-ttu-id="4b297-191">Die Eigenschaft `nextExpectedRanges` listet nicht immer alle fehlenden Bereiche auf.</span><span class="sxs-lookup"><span data-stu-id="4b297-191">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="4b297-p115">Wird ein Segment geschrieben, gibt sie den nächsten Bereich zurück, ab dem begonnen wird (z. B. „523-“).</span><span class="sxs-lookup"><span data-stu-id="4b297-p115">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="4b297-p116">Schlägt der Schreibvorgang fehl, weil der Client ein Fragment gesendet hat, das der Server bereits empfangen hat, antwortet der Server mit `HTTP 416 Requested Range Not Satisfiable`. Sie können den [Uploadstatus anfordern](#resuming-an-in-progress-upload), um eine detailliertere Liste der fehlenden Bereiche zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="4b297-p116">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="4b297-p117">Wenn Sie den Autorisierungsheader in den `PUT`-Aufruf einschließen, wird möglicherweise eine Antwort des Typs `HTTP 401 Unauthorized` zurückgegeben. Der Autorisierungsheader und das Bearertoken sollten nur mit dem `POST`-Aufruf im Rahmen von Schritt 1 gesendet werden. Der Autorisierungsheader sollte nicht in den `PUT`-Aufruf eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="4b297-p117">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthorized` response. The Authorization header and bearer token should only be sent when issuing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>

## <a name="completing-a-file"></a><span data-ttu-id="4b297-199">Vervollständigen einer Datei</span><span class="sxs-lookup"><span data-stu-id="4b297-199">Completing a file</span></span>

<span data-ttu-id="4b297-200">Wenn `deferCommit` ist, false oder nicht festgelegt ist, und klicken Sie dann automatisch der Hochladevorgang abgeschlossen ist, bei der letzten Bytebereich der Datei zum Hochladen URL ABGELEGT wird.</span><span class="sxs-lookup"><span data-stu-id="4b297-200">If `deferCommit` is false or unset, then the upload is automatically completed when the final byte range of the file is PUT to the upload URL.</span></span>
<span data-ttu-id="4b297-201">Wenn `deferCommit` true ist, wird nach der letzten Bytebereich der Datei zum Hochladen URL aktiviert wird, der Hochladevorgang explizit durch eine endgültige POST-Anforderung an den Upload abgeschlossen sein muss, Url mit Nulllänge Inhalt.</span><span class="sxs-lookup"><span data-stu-id="4b297-201">If `deferCommit` is true, then after the final byte range of the file is PUT to the upload URL, the upload should be explicitly completed by a final POST request to the upload url with zero-length content.</span></span>

<span data-ttu-id="4b297-202">Wenn der Hochladevorgang abgeschlossen ist, wird der Server mit der letzten Anforderung Antworten ein `HTTP 201 Created` oder `HTTP 200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4b297-202">When the upload is completed, the server will respond to the final request with an `HTTP 201 Created` or `HTTP 200 OK`.</span></span>
<span data-ttu-id="4b297-203">Der Antworttext enthält auch die Standardeigenschaft, die für das **DriveItem** festgelegt wurde, das die vervollständigte Datei repräsentiert.</span><span class="sxs-lookup"><span data-stu-id="4b297-203">The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "files.readwrite" } -->

```
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
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


<!-- { "blockType": "request", "opaqueUrl": true, "name": "commit-upload", "scopes": "files.readwrite" } -->

```
POST https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 0
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

## <a name="handling-upload-conflicts"></a><span data-ttu-id="4b297-204">Umgang mit Upload-Konflikten</span><span class="sxs-lookup"><span data-stu-id="4b297-204">Handling upload conflicts</span></span>

<span data-ttu-id="4b297-205">Wenn ein Konflikt auftritt, nachdem die Datei hochgeladen wurde (während der Uploadsitzung wurde beispielsweise ein Element mit demselben Namen erstellt), wird ein Fehler zurückgegeben, wenn der letzte Bytebereich hochgeladen wurde.</span><span class="sxs-lookup"><span data-stu-id="4b297-205">If a conflict occurs after the file is uploaded (for example, an item with the same name was created during the upload session), an error is returned when the last byte range is uploaded.</span></span>

```http
HTTP/1.1 409 Conflict
Content-Type: application/json

{
  "error":
  {
    "code": "upload_name_conflict",
    "message": "Another file exists with the same name as the uploaded session. You can redirect the upload session to use a new filename by calling PUT with the new metadata and @microsoft.graph.sourceUrl attribute.",
  }
}
```

## <a name="cancel-the-upload-session"></a><span data-ttu-id="4b297-206">Abbrechen der Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="4b297-206">Cancel the upload session</span></span>

<span data-ttu-id="4b297-p120">Wenn Sie eine Uploadsitzung abbrechen möchten, senden Sie eine DELETE-Anforderung an die Upload-URL. Das bereinigt die temporäre Datei, in der die bisher hochgeladenen Daten gespeichert sind. Verwenden Sie diese Vorgehensweise in Szenarios, in denen der Upload abgebrochen wird, beispielsweise bei Abbruch der Übertragung durch den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="4b297-p120">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="4b297-210">Temporäre Dateien und die zugehörigen Uploadsitzungen werden automatisch bereinigt, wenn der über **expirationDateTime** festgelegte Termin abgelaufen ist.</span><span class="sxs-lookup"><span data-stu-id="4b297-210">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>
<span data-ttu-id="4b297-211">Temporäre Dateien werden eventuell nicht sofort gelöscht, nachdem die Ablaufzeit verstrichen ist.</span><span class="sxs-lookup"><span data-stu-id="4b297-211">Temporary files may not be deleted immedately after the expiration time has elapsed.</span></span>

### <a name="request"></a><span data-ttu-id="4b297-212">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b297-212">Request</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a><span data-ttu-id="4b297-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b297-213">Response</span></span>

<span data-ttu-id="4b297-214">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="4b297-214">The following example shows the response.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="4b297-215">Fortsetzen eines laufenden Uploads</span><span class="sxs-lookup"><span data-stu-id="4b297-215">Resuming an in-progress upload</span></span>

<span data-ttu-id="4b297-p122">Wenn während einer Uploadanforderung die Verbindung getrennt wird oder anderweitig ausfällt, bevor die Anforderung abgeschlossen ist, werden alle Bytes in dieser Anforderung ignoriert. Dies kann passieren, wenn die Verbindung zwischen der App und dem Dienst getrennt wird. Tritt ein solcher Fall ein, kann die App die Dateiübertragung trotzdem ab dem letzten vollständig übertragenen Fragment fortsetzen.</span><span class="sxs-lookup"><span data-stu-id="4b297-p122">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="4b297-219">Um herauszufinden, welche Bytebereiche bereits empfangen wurden, kann die App den Status der Uploadsitzung anfordern.</span><span class="sxs-lookup"><span data-stu-id="4b297-219">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="4b297-220">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b297-220">Example</span></span>

<span data-ttu-id="4b297-221">Sie können den Status des Uploads anfragen, indem Sie eine GET-Anforderung an `uploadUrl` senden.</span><span class="sxs-lookup"><span data-stu-id="4b297-221">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

<span data-ttu-id="4b297-222">Der Server antwortet mit einer Liste der fehlenden Bytebereiche, die noch hochgeladen werden müssen, sowie mit dem Ablauftermin der Uploadsitzung.</span><span class="sxs-lookup"><span data-stu-id="4b297-222">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="4b297-223">Hochladen von verbleibenden Daten</span><span class="sxs-lookup"><span data-stu-id="4b297-223">Upload remaining data</span></span>

<span data-ttu-id="4b297-224">Die App weiß jetzt, ab wo der Upload gestartet werden soll. Führen Sie nun die Schritte im Abschnitt [Hochladen von Bytes in die Uploadsitzung](#upload-bytes-to-the-upload-session) durch, um den Upload fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="4b297-224">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>

## <a name="handle-upload-errors"></a><span data-ttu-id="4b297-225">Behandeln von Fehlern beim Upload</span><span class="sxs-lookup"><span data-stu-id="4b297-225">Handle upload errors</span></span>

<span data-ttu-id="4b297-226">Wenn der letzte Bytebereich einer Datei hochgeladen wird, kann ein Fehler auftreten.</span><span class="sxs-lookup"><span data-stu-id="4b297-226">When the last byte range of a file is uploaded, it is possible for an error to occur.</span></span> <span data-ttu-id="4b297-227">Dies kann an einem Namenskonflikt liegen oder daran, dass eine Kontingenteinschränkung überschritten wurde.</span><span class="sxs-lookup"><span data-stu-id="4b297-227">This can be due to a name conflict or quota limitation being exceeded.</span></span>
<span data-ttu-id="4b297-228">Die Uploadsitzung wird bis zur Ablaufzeit beibehalten. Dadurch kann Ihre App den Upload wiederherstellen, indem ein ausdrücklicher Commit der Uploadsitzung durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="4b297-228">The upload session will be preserved until the expiration time, which allows your app to recover the upload by explicitly committing the upload session.</span></span>

<span data-ttu-id="4b297-229">Um ausdrücklich einen Commit für die Uploadsitzung durchzuführen, muss Ihre App eine PUT-Anforderung mit einer neuen **driveItem**-Ressource durchführen, die für den Commit der Uploadsitzung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="4b297-229">To explicitly commit the upload session, your app must make a PUT request with a new **driveItem** resource that will be used when committing the upload session.</span></span>
<span data-ttu-id="4b297-230">Diese neue Anforderung sollte die Quelle der Fehler korrigieren, die den ursprünglichen Uploadfehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="4b297-230">This new request should correct the source of error that generated the original upload error.</span></span>

<span data-ttu-id="4b297-231">Um anzugeben, dass Ihre App einen Commit zu einer bestehenden Uploadsitzung durchführt, muss die PUT-Anforderung die `@microsoft.graph.sourceUrl`-Eigenschaft mit dem Wert Ihrer Uploadsitzungs-URL enthalten.</span><span class="sxs-lookup"><span data-stu-id="4b297-231">To indicate that your app is committing an existing upload session, the PUT request must include the `@microsoft.graph.sourceUrl` property with the value of your upload session URL.</span></span>

<!-- { "blockType": "ignored", "name": "explicit-upload-commit", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PUT /me/drive/root:/{path_to_parent}
Content-Type: application/json
If-Match: {etag or ctag}

{
  "name": "largefile.vhd",
  "@microsoft.graph.conflictBehavior": "rename",
  "@microsoft.graph.sourceUrl": "{upload session URL}"
}
```

<span data-ttu-id="4b297-232">**Hinweis:** Sie können den `@microsoft.graph.conflictBehavior`- und `if-match`-Header wie erwartet in diesem Aufruf verwenden.</span><span class="sxs-lookup"><span data-stu-id="4b297-232">**Note:** You can use the `@microsoft.graph.conflictBehavior` and `if-match` headers as expected in this call.</span></span>

### <a name="http-response"></a><span data-ttu-id="4b297-233">HTTP-Antwort</span><span class="sxs-lookup"><span data-stu-id="4b297-233">HTTP response</span></span>

<span data-ttu-id="4b297-234">Wenn mithilfe der neuen Metadaten ein Commit für die Datei durchgeführt werden kann, wird die Fehlerantwort `HTTP 201 Created` oder `HTTP 200 OK` mit den Elementmetadaten für die hochgeladene Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b297-234">If the file can be committed using the new metadata, an `HTTP 201 Created` or `HTTP 200 OK` response will be returned with the Item metadata for the uploaded file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

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

## <a name="best-practices"></a><span data-ttu-id="4b297-235">Bewährte Methoden</span><span class="sxs-lookup"><span data-stu-id="4b297-235">Best practices</span></span>

* <span data-ttu-id="4b297-236">Setzen Sie alle Uploads fort bzw. starten Sie alle Uploads neu, die wegen eines Verbindungsabbruchs oder einem 5xx-Fehler fehlschlagen, beispielsweise:</span><span class="sxs-lookup"><span data-stu-id="4b297-236">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="4b297-237">Verwenden Sie einen Exponential Backoff-Algorithmus, wenn beim Fortsetzen oder Neusenden einer Uploadanforderung 5xx-Serverfehler auftreten.</span><span class="sxs-lookup"><span data-stu-id="4b297-237">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="4b297-238">Bei anderen Fehlern sollten Sie keinen Exponential Backoff-Algorithmus verwenden, sondern stattdessen die Anzahl der Wiederholungsversuche beschränken.</span><span class="sxs-lookup"><span data-stu-id="4b297-238">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="4b297-239">Sollte bei fortsetzbaren Uploads der Fehler `404 Not Found` auftreten, starten Sie den gesamten Upload neu.</span><span class="sxs-lookup"><span data-stu-id="4b297-239">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span> <span data-ttu-id="4b297-240">Dies bedeutet, dass die Upload-Sitzung nicht mehr vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="4b297-240">This indicates the upload session no longer exists.</span></span>
* <span data-ttu-id="4b297-241">Verwenden Sie fortsetzbare Dateiübertragungen für Dateien, die größer als 10 MiB sind (10.485.760 Byte).</span><span class="sxs-lookup"><span data-stu-id="4b297-241">Use resumable file transfers for files larger than 10 MiB (10,485,760 bytes).</span></span>
* <span data-ttu-id="4b297-242">Die optimale Größe eines Bytebereichs für stabile Highspeedverbindungen ist 10 MiB.</span><span class="sxs-lookup"><span data-stu-id="4b297-242">A byte range size of 10 MiB for stable high speed connections is optimal.</span></span> <span data-ttu-id="4b297-243">Bei langsameren oder weniger zuverlässigen Verbindungen liefern kleinere Fragmentgrößen eventuell bessere Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="4b297-243">For slower or less reliable connections you may get better results from a smaller fragment size.</span></span> <span data-ttu-id="4b297-244">Die empfohlene Fragmentgröße liegt zwischen 5 und 10 MiB.</span><span class="sxs-lookup"><span data-stu-id="4b297-244">The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="4b297-245">Verwenden Sie eine Bytebereichsgröße, die ein Vielfaches von 320 KiB ist (327.680 Byte) ist.</span><span class="sxs-lookup"><span data-stu-id="4b297-245">Use a byte range size that is a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="4b297-246">Wenn Sie eine Fragmentgröße verwenden, die kein Vielfaches von 320 KiB ist, können Übertragungen großer Dateien nach Upload des letzten Bytebereichs fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="4b297-246">Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last byte range is uploaded.</span></span>

## <a name="error-responses"></a><span data-ttu-id="4b297-247">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="4b297-247">Error responses</span></span>

<span data-ttu-id="4b297-248">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="4b297-248">See the [Error Responses][error-response] topic for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "section": "documentation"
} -->
