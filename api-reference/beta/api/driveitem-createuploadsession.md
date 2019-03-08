---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Fort Setz barer Dateiupload
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b0495a0c63400d6476c1ad9312e708b9ac880e42
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482392"
---
# <a name="upload-large-files-with-an-upload-session"></a><span data-ttu-id="4ff9e-102">Hochladen großer Dateien mit einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="4ff9e-102">Upload large files with an upload session</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ff9e-p101">Wenn Sie eine Uploadsitzung erstellen, kann Ihre App Dateien bis zur maximal zulässigen Dateigröße hochladen. Eine Uploadsitzung erlaubt es der App, Bereiche einer Datei in sequenziellen API-Anfragen hochzuladen. Bricht die Verbindung während des Uploads ab, kann die Übertragung so anschließend fortgesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-p101">Create an upload session to allow your app to upload files up to the maximum file size. An upload session allows your app to upload ranges of the file in sequential API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="4ff9e-105">Sie müssen zwei Schritte durchführen, um eine Datei mit einer Uploadsitzung hochzuladen:</span><span class="sxs-lookup"><span data-stu-id="4ff9e-105">To upload a file using an upload session, there are two steps:</span></span>

1. [<span data-ttu-id="4ff9e-106">Erstellen einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="4ff9e-106">Create an upload session</span></span>](#create-an-upload-session)
2. [<span data-ttu-id="4ff9e-107">Hochladen von Bytes in die Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="4ff9e-107">Upload bytes to the upload session</span></span>](#upload-bytes-to-the-upload-session)

## <a name="permissions"></a><span data-ttu-id="4ff9e-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4ff9e-108">Permissions</span></span>

<span data-ttu-id="4ff9e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ff9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ff9e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4ff9e-111">Permission type</span></span>      | <span data-ttu-id="4ff9e-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4ff9e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ff9e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4ff9e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4ff9e-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ff9e-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ff9e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4ff9e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ff9e-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ff9e-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ff9e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4ff9e-117">Application</span></span> | <span data-ttu-id="4ff9e-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ff9e-118">Sites.ReadWrite.All</span></span> |

## <a name="create-an-upload-session"></a><span data-ttu-id="4ff9e-119">Erstellen einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="4ff9e-119">Create an upload session</span></span>

<span data-ttu-id="4ff9e-120">Um eine große Datei hochladen zu können, muss die App zuerst eine neue Uploadsitzung anfordern.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-120">To begin a large file upload, your app must first request a new upload session.</span></span>
<span data-ttu-id="4ff9e-121">Es wird dann ein temporärer Speicherort erstellt, an dem die Bytes der Datei gespeichert werden, bis sie vollständig hochgeladen ist.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-121">This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded.</span></span>
<span data-ttu-id="4ff9e-122">Sobald das letzte Byte der Datei hochgeladen wurde, ist die Uploadsitzung abgeschlossen, und die endgültige Datei wird im Zielordner angezeigt.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-122">Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>
<span data-ttu-id="4ff9e-123">Alternativ können Sie die endgültige Erstellung der Datei im Ziel verschieben, bis Sie explizit eine Anforderung zum Abschließen des Uploads vornehmen, indem Sie die `deferCommit` Eigenschaft in den Anforderungs Argumenten festlegen.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-123">Alternatively, you can defer final creation of the file in the destination until you explicitly make a request to complete the upload, by setting the `deferCommit` property in the request arguments.</span></span>

### <a name="http-request"></a><span data-ttu-id="4ff9e-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ff9e-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="4ff9e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4ff9e-125">Request body</span></span>

<span data-ttu-id="4ff9e-126">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-126">No request body is required.</span></span>
<span data-ttu-id="4ff9e-127">Sie können jedoch Eigenschaften im Anforderungstext angeben, die zusätzliche Daten über die hochzuladende Datei bereitstellen und die Semantik des Upload-Vorgangs anpassen.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-127">However, you can specify properties in the request body providing additional data about the file being uploaded and customizing the semantics of the upload operation.</span></span>

<span data-ttu-id="4ff9e-128">Die `item` -Eigenschaft kann beispielsweise die folgenden Parameter festlegen:<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } --></span><span class="sxs-lookup"><span data-stu-id="4ff9e-128">For example, the `item` property allows setting the following parameters: <!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } --></span></span>
```json
{
  "@microsoft.graph.conflictBehavior": "rename | fail | overwrite",
  "description": "description",
  "name": "filename.txt"
}
```

<span data-ttu-id="4ff9e-129">Das folgende Beispiel steuert das Verhalten, wenn der Dateiname bereits verwendet wird, und gibt außerdem an, dass die endgültige Datei erst erstellt werden soll, wenn eine explizite Vervollständigungs Anforderung ausgeführt wird:</span><span class="sxs-lookup"><span data-stu-id="4ff9e-129">The following example controls the behavior if the filename is already taken, and also specifies that the final file should not be created until an explicit completion request is made:</span></span>

<!-- { "blockType": "ignored" } -->
```json
{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename"
  },
  "deferCommit": true
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="4ff9e-130">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4ff9e-130">Optional request headers</span></span>

| <span data-ttu-id="4ff9e-131">Name</span><span class="sxs-lookup"><span data-stu-id="4ff9e-131">Name</span></span>       | <span data-ttu-id="4ff9e-132">Wert</span><span class="sxs-lookup"><span data-stu-id="4ff9e-132">Value</span></span> | <span data-ttu-id="4ff9e-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ff9e-133">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4ff9e-134">*if-match*</span><span class="sxs-lookup"><span data-stu-id="4ff9e-134">*if-match*</span></span> | <span data-ttu-id="4ff9e-135">etag</span><span class="sxs-lookup"><span data-stu-id="4ff9e-135">etag</span></span>  | <span data-ttu-id="4ff9e-136">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) nicht mit dem aktuellen ETag des Elements übereinstimmt, `412 Precondition Failed` wird eine Fehlerantwort zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-136">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` error response is returned.</span></span> |

## <a name="parameters"></a><span data-ttu-id="4ff9e-137">Parameter</span><span class="sxs-lookup"><span data-stu-id="4ff9e-137">Parameters</span></span>

| <span data-ttu-id="4ff9e-138">Parameter</span><span class="sxs-lookup"><span data-stu-id="4ff9e-138">Parameter</span></span>            | <span data-ttu-id="4ff9e-139">Typ</span><span class="sxs-lookup"><span data-stu-id="4ff9e-139">Type</span></span>                          | <span data-ttu-id="4ff9e-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ff9e-140">Description</span></span>
|:---------------------|:------------------------------|:---------------------------------
| <span data-ttu-id="4ff9e-141">item</span><span class="sxs-lookup"><span data-stu-id="4ff9e-141">item</span></span>                 | <span data-ttu-id="4ff9e-142">driveItemUploadableProperties</span><span class="sxs-lookup"><span data-stu-id="4ff9e-142">driveItemUploadableProperties</span></span> | <span data-ttu-id="4ff9e-143">Daten zu der hochzuladenden Datei</span><span class="sxs-lookup"><span data-stu-id="4ff9e-143">Data about the file being uploaded</span></span>
| <span data-ttu-id="4ff9e-144">deferCommit</span><span class="sxs-lookup"><span data-stu-id="4ff9e-144">deferCommit</span></span>          | <span data-ttu-id="4ff9e-145">Boolesch</span><span class="sxs-lookup"><span data-stu-id="4ff9e-145">Boolean</span></span>                       | <span data-ttu-id="4ff9e-146">Bei Festlegung auf "true" erfordert die endgültige Erstellung der Datei im Ziel eine explizite Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-146">If set to true, final creation of the file in the destination will require an explicit request.</span></span> <span data-ttu-id="4ff9e-147">Nur bei OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-147">Only on OneDrive for Business.</span></span>

## <a name="item-properties"></a><span data-ttu-id="4ff9e-148">Elementeigenschaften</span><span class="sxs-lookup"><span data-stu-id="4ff9e-148">Item properties</span></span>

| <span data-ttu-id="4ff9e-149">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4ff9e-149">Property</span></span>             | <span data-ttu-id="4ff9e-150">Typ</span><span class="sxs-lookup"><span data-stu-id="4ff9e-150">Type</span></span>               | <span data-ttu-id="4ff9e-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ff9e-151">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="4ff9e-152">description</span><span class="sxs-lookup"><span data-stu-id="4ff9e-152">description</span></span>          | <span data-ttu-id="4ff9e-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4ff9e-153">String</span></span>             | <span data-ttu-id="4ff9e-154">Stellt eine für den Benutzer sichtbare Beschreibung des Elements bereit.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-154">Provides a user-visible description of the item.</span></span> <span data-ttu-id="4ff9e-155">Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-155">Read-write.</span></span> <span data-ttu-id="4ff9e-156">Nur auf OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-156">Only on OneDrive Personal.</span></span>
| <span data-ttu-id="4ff9e-157">name</span><span class="sxs-lookup"><span data-stu-id="4ff9e-157">name</span></span>                 | <span data-ttu-id="4ff9e-158">String</span><span class="sxs-lookup"><span data-stu-id="4ff9e-158">String</span></span>             | <span data-ttu-id="4ff9e-p107">Der Name des Elements (Dateiname und Erweiterung). Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-p107">The name of the item (filename and extension). Read-write.</span></span>

### <a name="request"></a><span data-ttu-id="4ff9e-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ff9e-161">Request</span></span>

<span data-ttu-id="4ff9e-162">Die Antwort auf diese Anforderung enthält die Details der neu erstellten Ressource des Typs [uploadSession](../resources/uploadsession.md), einschließlich der zum Upload der Dateiteile verwendeten URL.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-162">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

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

### <a name="response"></a><span data-ttu-id="4ff9e-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ff9e-163">Response</span></span>

<span data-ttu-id="4ff9e-164">Wenn der Vorgang erfolgreich war, liefert die Antwort auf diese Anforderung die Details dazu, wohin die verbleibenden Anforderungen als [UploadSession](../resources/uploadsession.md)-Ressource gesendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-164">The response to this request, if successful, will provide the details for where the remainder of the requests should be sent as an [UploadSession](../resources/uploadsession.md) resource.</span></span>

<span data-ttu-id="4ff9e-165">Diese Ressource gibt Details zu dem Ort an, an dem der Bytebereich hochgeladen werden sollte und wann die Uploadsitzung abläuft.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-165">This resource provides details about where the byte range of the file should be uploaded and when the upload session expires.</span></span>

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

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="4ff9e-166">Hochladen von Bytes in die Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="4ff9e-166">Upload bytes to the upload session</span></span>

<span data-ttu-id="4ff9e-167">Zum Hochladen der Datei oder eines Teils der Datei sendet die App eine PUT-Anfrage an den Wert **uploadUrl**, der ihr in der **createUploadSession**-Antwort übermittelt wurde.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-167">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>
<span data-ttu-id="4ff9e-168">Sie können die gesamte Datei hochladen oder die Datei in Fragmente aufteilen, vorausgesetzt, die maximale Bytezahl pro Anforderung bleibt unter 60 MiB.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-168">You can upload the entire file, or split the file into multiple byte ranges, as long as the maximum bytes in any given request is less than 60 MiB.</span></span>

<span data-ttu-id="4ff9e-169">Die Fragmente der Datei müssen sequenziell in der richtigen Reihenfolge hochgeladen werden.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-169">The fragments of the file must be uploaded sequentially in order.</span></span>
<span data-ttu-id="4ff9e-170">Werden die Fragmente in der falschen Reihenfolge hochgeladen, tritt ein Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-170">Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="4ff9e-171">**Hinweis:** Wenn die App eine Datei in mehrere Fragmente aufteilt, **MUSS** die Größe jedes Fragments ein Vielfaches von 320 KiB (327.680 Byte) sein.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-171">**Note:** If your app splits a file into multiple byte ranges, the size of each byte range **MUST** be a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="4ff9e-172">Bei Fragmentgrößen, die sich nicht ohne Rest durch 320 KiB teilen lassen, treten beim Übergeben einiger Dateien Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-172">Using a fragment size that does not divide evenly by 320 KiB will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="4ff9e-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ff9e-173">Example</span></span>

<span data-ttu-id="4ff9e-174">In diesem Beispiel lädt die App die ersten 26 Byte einer 128-Byte-Datei hoch.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-174">In this example, the app is uploading the first 26 bytes of a 128 byte file.</span></span>

* <span data-ttu-id="4ff9e-175">Der Header **Content-Length** definiert die Größe der aktuellen Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-175">The **Content-Length** header specifies the size of the current request.</span></span>
* <span data-ttu-id="4ff9e-176">Der Header **Content-Range** gibt den Bytebereich in der Gesamtdatei an, den diese Anforderung repräsentiert.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-176">The **Content-Range** header indicates the range of bytes in the overall file that this request represents.</span></span>
* <span data-ttu-id="4ff9e-177">Die Gesamtlänge der Datei muss bekannt sein, bevor Sie das erste Fragment der Datei hochladen können.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-177">The total length of the file is known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="4ff9e-178">**Wichtig:** Die App muss sicherstellen, dass die im Header **Content-Range** angegebene Gesamtdateigröße bei allen Anforderungen identisch ist.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-178">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests.</span></span>
<span data-ttu-id="4ff9e-179">Wird für einen Bytebereich eine andere Dateigröße deklariert, schlägt die betreffende Anforderung fehl.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-179">If a byte range declares a different file size, the request will fail.</span></span>

### <a name="response"></a><span data-ttu-id="4ff9e-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ff9e-180">Response</span></span>

<span data-ttu-id="4ff9e-181">Wenn die Anforderung abgeschlossen ist, antwortet der Server mit `202 Accepted`, wenn es weitere Bytebereiche, die hochgeladen werden müssen.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-181">When the request is complete, the server will respond with `202 Accepted` if there are more byte ranges that need to be uploaded.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="4ff9e-182">Die App kann mithilfe des Werts **nextExpectedRanges** bestimmen, wo der nächste Bytebereich beginnen soll.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-182">Your app can use the **nextExpectedRanges** value to determine where to start the next byte range.</span></span>
<span data-ttu-id="4ff9e-183">Eventuell werden mehrere Bereiche angegeben. Sie stehen für Teile der Datei, die der Server noch nicht empfangen hat.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-183">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="4ff9e-184">Dies ist nützlich, wenn eine Übertragung nach einer Unterbrechung fortgesetzt werden soll und der Client den Dienststatus nicht kennt.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-184">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="4ff9e-185">Halten Sie sich bei der Festlegung der Größe der Bytebereiche immer an die unten beschriebenen bewährten Methoden.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-185">You should always determine the size of your byte ranges according to the best practices below.</span></span> <span data-ttu-id="4ff9e-186">Gehen Sie nicht davon aus, dass **nextExpectedRanges** richtig dimensionierte Bytebereiche für einen Upload zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-186">Do not assume that **nextExpectedRanges** will return reanges of proper size for a byte range to upload.</span></span>
<span data-ttu-id="4ff9e-187">Die Eigenschaft **nextExpectedRanges** gibt Dateibereiche an, die noch nicht empfangen wurden. Sie ist nicht als Muster für den Dateiupload der App zu verstehen.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-187">The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how your app should upload the file.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="4ff9e-188">HinwBemerkungeneise</span><span class="sxs-lookup"><span data-stu-id="4ff9e-188">Remarks</span></span>

* <span data-ttu-id="4ff9e-189">Die Eigenschaft `nextExpectedRanges` listet nicht immer alle fehlenden Bereiche auf.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-189">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="4ff9e-p114">Wird ein Segment geschrieben, gibt sie den nächsten Bereich zurück, ab dem begonnen wird (z. B. „523-“).</span><span class="sxs-lookup"><span data-stu-id="4ff9e-p114">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="4ff9e-p115">Schlägt der Schreibvorgang fehl, weil der Client ein Fragment gesendet hat, das der Server bereits empfangen hat, antwortet der Server mit `HTTP 416 Requested Range Not Satisfiable`. Sie können den [Uploadstatus anfordern](#resuming-an-in-progress-upload), um eine detailliertere Liste der fehlenden Bereiche zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-p115">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="4ff9e-p116">Wenn Sie den Autorisierungsheader in den `PUT`-Aufruf einschließen, wird möglicherweise eine Antwort des Typs `HTTP 401 Unauthorized` zurückgegeben. Der Autorisierungsheader und das Bearertoken sollten nur mit dem `POST`-Aufruf im Rahmen von Schritt 1 gesendet werden. Der Autorisierungsheader sollte nicht in den `PUT`-Aufruf eingeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-p116">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthorized` response. The Authorization header and bearer token should only be sent when issuing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>

## <a name="completing-a-file"></a><span data-ttu-id="4ff9e-197">Vervollständigen einer Datei</span><span class="sxs-lookup"><span data-stu-id="4ff9e-197">Completing a file</span></span>

<span data-ttu-id="4ff9e-198">`deferCommit` Ist false oder nicht festgelegt, wird der Upload automatisch abgeschlossen, wenn der letzte Byte-Umfang der Datei der Upload-URL zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-198">If `deferCommit` is false or unset, then the upload is automatically completed when the final byte range of the file is PUT to the upload URL.</span></span>
<span data-ttu-id="4ff9e-199">Wenn `deferCommit` der Wert true ist, sollte der Upload nach dem letzten Byte-Umfang der Datei auf die Upload-URL übertragen werden, und das Hochladen sollte explizit durch eine abschließende Post-Anforderung an die Upload-URL mit dem Inhalt der leeren Länge abgeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-199">If `deferCommit` is true, then after the final byte range of the file is PUT to the upload URL, the upload should be explicitly completed by a final POST request to the upload url with zero-length content.</span></span>

<span data-ttu-id="4ff9e-200">Nach Abschluss des Uploads antwortet der Server auf die endgültige Anforderung mit einem `HTTP 201 Created` oder. `HTTP 200 OK`</span><span class="sxs-lookup"><span data-stu-id="4ff9e-200">When the upload is completed, the server will respond to the final request with an `HTTP 201 Created` or `HTTP 200 OK`.</span></span>
<span data-ttu-id="4ff9e-201">Der Antworttext enthält auch die Standardeigenschaft, die für das **DriveItem** festgelegt wurde, das die vervollständigte Datei repräsentiert.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-201">The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

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

## <a name="handling-upload-conflicts"></a><span data-ttu-id="4ff9e-202">Umgang mit Upload-Konflikten</span><span class="sxs-lookup"><span data-stu-id="4ff9e-202">Handling upload conflicts</span></span>

<span data-ttu-id="4ff9e-203">Wenn ein Konflikt auftritt, nachdem die Datei hochgeladen wurde (während der Uploadsitzung wurde beispielsweise ein Element mit demselben Namen erstellt), wird ein Fehler zurückgegeben, wenn der letzte Bytebereich hochgeladen wurde.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-203">If a conflict occurs after the file is uploaded (for example, an item with the same name was created during the upload session), an error is returned when the last byte range is uploaded.</span></span>

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

## <a name="cancel-the-upload-session"></a><span data-ttu-id="4ff9e-204">Abbrechen der Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="4ff9e-204">Cancel the upload session</span></span>

<span data-ttu-id="4ff9e-p119">Wenn Sie eine Uploadsitzung abbrechen möchten, senden Sie eine DELETE-Anforderung an die Upload-URL. Das bereinigt die temporäre Datei, in der die bisher hochgeladenen Daten gespeichert sind. Verwenden Sie diese Vorgehensweise in Szenarios, in denen der Upload abgebrochen wird, beispielsweise bei Abbruch der Übertragung durch den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-p119">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="4ff9e-208">Temporäre Dateien und die zugehörigen Uploadsitzungen werden automatisch bereinigt, wenn der über **expirationDateTime** festgelegte Termin abgelaufen ist.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-208">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>
<span data-ttu-id="4ff9e-209">Temporäre Dateien werden eventuell nicht sofort gelöscht, nachdem die Ablaufzeit verstrichen ist.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-209">Temporary files may not be deleted immedately after the expiration time has elapsed.</span></span>

### <a name="request"></a><span data-ttu-id="4ff9e-210">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ff9e-210">Request</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a><span data-ttu-id="4ff9e-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ff9e-211">Response</span></span>

<span data-ttu-id="4ff9e-212">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-212">The following example shows the response.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="4ff9e-213">Fortsetzen eines laufenden Uploads</span><span class="sxs-lookup"><span data-stu-id="4ff9e-213">Resuming an in-progress upload</span></span>

<span data-ttu-id="4ff9e-p121">Wenn während einer Uploadanforderung die Verbindung getrennt wird oder anderweitig ausfällt, bevor die Anforderung abgeschlossen ist, werden alle Bytes in dieser Anforderung ignoriert. Dies kann passieren, wenn die Verbindung zwischen der App und dem Dienst getrennt wird. Tritt ein solcher Fall ein, kann die App die Dateiübertragung trotzdem ab dem letzten vollständig übertragenen Fragment fortsetzen.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-p121">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="4ff9e-217">Um herauszufinden, welche Bytebereiche bereits empfangen wurden, kann die App den Status der Uploadsitzung anfordern.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-217">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="4ff9e-218">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ff9e-218">Example</span></span>

<span data-ttu-id="4ff9e-219">Sie können den Status des Uploads anfragen, indem Sie eine GET-Anforderung an `uploadUrl` senden.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-219">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

<span data-ttu-id="4ff9e-220">Der Server antwortet mit einer Liste der fehlenden Bytebereiche, die noch hochgeladen werden müssen, sowie mit dem Ablauftermin der Uploadsitzung.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-220">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="4ff9e-221">Hochladen von verbleibenden Daten</span><span class="sxs-lookup"><span data-stu-id="4ff9e-221">Upload remaining data</span></span>

<span data-ttu-id="4ff9e-222">Die App weiß jetzt, ab wo der Upload gestartet werden soll. Führen Sie nun die Schritte im Abschnitt [Hochladen von Bytes in die Uploadsitzung](#upload-bytes-to-the-upload-session) durch, um den Upload fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-222">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>

## <a name="handle-upload-errors"></a><span data-ttu-id="4ff9e-223">Behandeln von Fehlern beim Upload</span><span class="sxs-lookup"><span data-stu-id="4ff9e-223">Handle upload errors</span></span>

<span data-ttu-id="4ff9e-224">Wenn der letzte Bytebereich einer Datei hochgeladen wird, kann ein Fehler auftreten.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-224">When the last byte range of a file is uploaded, it is possible for an error to occur.</span></span> <span data-ttu-id="4ff9e-225">Dies kann an einem Namenskonflikt liegen oder daran, dass eine Kontingenteinschränkung überschritten wurde.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-225">This can be due to a name conflict or quota limitation being exceeded.</span></span>
<span data-ttu-id="4ff9e-226">Die Uploadsitzung wird bis zur Ablaufzeit beibehalten. Dadurch kann Ihre App den Upload wiederherstellen, indem ein ausdrücklicher Commit der Uploadsitzung durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-226">The upload session will be preserved until the expiration time, which allows your app to recover the upload by explicitly committing the upload session.</span></span>

<span data-ttu-id="4ff9e-227">Um ausdrücklich einen Commit für die Uploadsitzung durchzuführen, muss Ihre App eine PUT-Anforderung mit einer neuen **driveItem**-Ressource durchführen, die für den Commit der Uploadsitzung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-227">To explicitly commit the upload session, your app must make a PUT request with a new **driveItem** resource that will be used when committing the upload session.</span></span>
<span data-ttu-id="4ff9e-228">Diese neue Anforderung sollte die Quelle der Fehler korrigieren, die den ursprünglichen Uploadfehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-228">This new request should correct the source of error that generated the original upload error.</span></span>

<span data-ttu-id="4ff9e-229">Um anzugeben, dass Ihre App einen Commit zu einer bestehenden Uploadsitzung durchführt, muss die PUT-Anforderung die `@microsoft.graph.sourceUrl`-Eigenschaft mit dem Wert Ihrer Uploadsitzungs-URL enthalten.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-229">To indicate that your app is committing an existing upload session, the PUT request must include the `@microsoft.graph.sourceUrl` property with the value of your upload session URL.</span></span>

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

<span data-ttu-id="4ff9e-230">**Hinweis:** Sie können den `@microsoft.graph.conflictBehavior`- und `if-match`-Header wie erwartet in diesem Aufruf verwenden.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-230">**Note:** You can use the `@microsoft.graph.conflictBehavior` and `if-match` headers as expected in this call.</span></span>

### <a name="response"></a><span data-ttu-id="4ff9e-231">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ff9e-231">Response</span></span>

<span data-ttu-id="4ff9e-232">Wenn mithilfe der neuen Metadaten ein Commit für die Datei durchgeführt werden kann, wird die Fehlerantwort `HTTP 201 Created` oder `HTTP 200 OK` mit den Elementmetadaten für die hochgeladene Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-232">If the file can be committed using the new metadata, an `HTTP 201 Created` or `HTTP 200 OK` response will be returned with the Item metadata for the uploaded file.</span></span>

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

## <a name="best-practices"></a><span data-ttu-id="4ff9e-233">Bewährte Methoden</span><span class="sxs-lookup"><span data-stu-id="4ff9e-233">Best practices</span></span>

* <span data-ttu-id="4ff9e-234">Setzen Sie alle Uploads fort bzw. starten Sie alle Uploads neu, die wegen eines Verbindungsabbruchs oder einem 5xx-Fehler fehlschlagen, beispielsweise:</span><span class="sxs-lookup"><span data-stu-id="4ff9e-234">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="4ff9e-235">Verwenden Sie einen Exponential Backoff-Algorithmus, wenn beim Fortsetzen oder Neusenden einer Uploadanforderung 5xx-Serverfehler auftreten.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-235">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="4ff9e-236">Bei anderen Fehlern sollten Sie keinen Exponential Backoff-Algorithmus verwenden, sondern stattdessen die Anzahl der Wiederholungsversuche beschränken.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-236">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="4ff9e-237">Sollte bei fortsetzbaren Uploads der Fehler `404 Not Found` auftreten, starten Sie den gesamten Upload neu.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-237">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span> <span data-ttu-id="4ff9e-238">Dies bedeutet, dass die Upload-Sitzung nicht mehr vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-238">This indicates the upload session no longer exists.</span></span>
* <span data-ttu-id="4ff9e-239">Verwenden Sie fortsetzbare Dateiübertragungen für Dateien, die größer als 10 MiB sind (10.485.760 Byte).</span><span class="sxs-lookup"><span data-stu-id="4ff9e-239">Use resumable file transfers for files larger than 10 MiB (10,485,760 bytes).</span></span>
* <span data-ttu-id="4ff9e-240">Die optimale Größe eines Bytebereichs für stabile Highspeedverbindungen ist 10 MiB.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-240">A byte range size of 10 MiB for stable high speed connections is optimal.</span></span> <span data-ttu-id="4ff9e-241">Bei langsameren oder weniger zuverlässigen Verbindungen liefern kleinere Fragmentgrößen eventuell bessere Ergebnisse.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-241">For slower or less reliable connections you may get better results from a smaller fragment size.</span></span> <span data-ttu-id="4ff9e-242">Die empfohlene Fragmentgröße liegt zwischen 5 und 10 MiB.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-242">The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="4ff9e-243">Verwenden Sie eine Bytebereichsgröße, die ein Vielfaches von 320 KiB ist (327.680 Byte) ist.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-243">Use a byte range size that is a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="4ff9e-244">Wenn Sie eine Fragmentgröße verwenden, die kein Vielfaches von 320 KiB ist, können Übertragungen großer Dateien nach Upload des letzten Bytebereichs fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="4ff9e-244">Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last byte range is uploaded.</span></span>

## <a name="error-responses"></a><span data-ttu-id="4ff9e-245">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="4ff9e-245">Error responses</span></span>

<span data-ttu-id="4ff9e-246">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="4ff9e-246">See the [Error Responses][error-response] topic for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-createuploadsession.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
