---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Wiederaufnehmbarer Dateien-Upload
ms.openlocfilehash: 14b9047f84b5390aea2f5285660e6c04a6bc3149
ms.sourcegitcommit: ebac77d2ca32438e552831de0258fe5e86fa225a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/17/2018
ms.locfileid: "26564758"
---
# <a name="upload-large-files-with-an-upload-session"></a>Hochladen großer Dateien mit einer Uploadsitzung

Wenn Sie eine Uploadsitzung erstellen, kann Ihre App Dateien bis zur maximal zulässigen Dateigröße hochladen. Eine Uploadsitzung erlaubt es der App, Bereiche einer Datei in sequenziellen API-Anfragen hochzuladen. Bricht die Verbindung während des Uploads ab, kann die Übertragung so anschließend fortgesetzt werden.

Sie müssen zwei Schritte durchführen, um eine Datei mit einer Uploadsitzung hochzuladen:

1. [Erstellen einer Uploadsitzung](#create-an-upload-session)
2. [Hochladen von Bytes in die Uploadsitzung](#upload-bytes-to-the-upload-session)

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Files.ReadWrite, Files.ReadWrite.All    |
|Anwendung | Sites.ReadWrite.All |

## <a name="create-an-upload-session"></a>Erstellen einer Uploadsitzung

Um eine große Datei hochladen zu können, muss die App zuerst eine neue Uploadsitzung anfordern. Es wird dann ein temporärer Speicherort erstellt, an dem die Bytes der Datei gespeichert werden, bis sie vollständig hochgeladen ist. Sobald das letzte Byte der Datei hochgeladen wurde, ist die Uploadsitzung abgeschlossen, und die endgültige Datei wird im Zielordner angezeigt.

### <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a>Anforderungstext

Es ist kein Anforderungstexts erforderlich.
Sie können jedoch angeben einer `item` -Eigenschaft im Textkörper Anforderung zusätzliche Daten über die hochgeladene Datei bereitstellen.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } -->
```json
{
  "@microsoft.graph.conflictBehavior": "rename | fail | replace",
  "description": "description",
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "name": "filename.txt"
}
```

Beispielsweise können Sie im Anforderungstext die Eigenschaft „conflictBehavior“ definieren, um festzulegen, wie vorgegangen werden soll, wenn der Dateiname bereits anderweitig in Verwendung ist.

<!-- { "blockType": "ignored" } -->
```json
{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename"
  }
}
```

### <a name="optional-request-headers"></a>Optionale Anforderungsheader

| Name       | Wert | Beschreibung                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| *if-match* | etag  | Wenn dieser Anforderungsheader enthalten ist und das angegebene Etag (oder CTag) nicht mit dem aktuellen Etag des Elements übereinstimmt, wird der Fehler `412 Precondition Failed` zurückgegeben. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft             | Typ               | Beschreibung
|:---------------------|:-------------------|:---------------------------------
| description          | Zeichenfolge             | Stellt eine für den Benutzer sichtbare Beschreibung des Elements bereit. Lese-/Schreibzugriff. Nur auf OneDrive Personal
| fileSystemInfo       | [fileSystemInfo][] | Informationen zum Dateisystem des Clients. Lese-/Schreibzugriff.
| name                 | Zeichenfolge             | Der Name des Elements (Dateiname und Erweiterung). Lese-/Schreibzugriff.

### <a name="request"></a>Anforderung

Die Antwort auf diese Anforderung enthält die Details der neu erstellten Ressource des Typs [uploadSession](../resources/uploadsession.md), einschließlich der zum Upload der Dateiteile verwendeten URL. 

<!-- { "blockType": "request", "name": "upload-fragment-create-session", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/root:/{item-path}:/createUploadSession
Content-Type: application/json

{
  "item": {
    "@odata.type": "microsoft.graph.driveItemUploadableProperties",
    "@microsoft.graph.conflictBehavior": "rename",
    "name": "largefile.dat"
  }
}
```

### <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, liefert die Antwort auf diese Anforderung die Details dazu, wohin die verbleibenden Anforderungen als [UploadSession](../resources/uploadSession.md)-Ressource gesendet werden sollen.

Diese Ressource gibt Details zu dem Ort an, an dem der Bytebereich hochgeladen werden sollte und wann die Uploadsitzung abläuft.

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

## <a name="upload-bytes-to-the-upload-session"></a>Hochladen von Bytes in die Uploadsitzung

Zum Hochladen der Datei oder eines Teils der Datei sendet die App eine PUT-Anfrage an den Wert **uploadUrl**, der ihr in der **createUploadSession**-Antwort übermittelt wurde.
Sie können die gesamte Datei hochladen oder die Datei in Fragmente aufteilen, vorausgesetzt, die maximale Bytezahl pro Anforderung bleibt unter 60 MiB.

Die Fragmente der Datei müssen in Reihenfolge nacheinander hochgeladen werden.
Werden die Fragmente in der falschen Reihenfolge hochgeladen, tritt ein Fehler auf.

**Hinweis:** Wenn die App eine Datei in mehrere Fragmente aufteilt, **MUSS** die Größe jedes Fragments ein Vielfaches von 320 KiB (327.680 Byte) sein. Bei Fragmentgrößen, die sich nicht ohne Rest durch 320 KiB teilen lassen, treten beim Übergeben einiger Dateien Fehler auf.

### <a name="example"></a>Beispiel

In diesem Beispiel lädt die App die ersten 26 Byte einer 128-Byte-Datei hoch.

* Der Header **Content-Length** definiert die Größe der aktuellen Anforderung.
* Der Header **Content-Range** gibt den Bytebereich in der Gesamtdatei an, den diese Anforderung repräsentiert.
* Die Gesamtlänge der Datei muss bekannt sein, bevor Sie das erste Fragment der Datei hochladen können.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

**Wichtig:** Die App muss sicherstellen, dass die im Header **Content-Range** angegebene Gesamtdateigröße bei allen Anforderungen identisch ist.
Wird für einen Bytebereich eine andere Dateigröße deklariert, schlägt die betreffende Anforderung fehl.

### <a name="response"></a>Antwort

Wenn die Anforderung abgeschlossen ist, antwortet der Server mit `202 Accepted`, wenn es weitere Bytebereiche, die hochgeladen werden müssen.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

Die App kann mithilfe des Werts **nextExpectedRanges** bestimmen, wo der nächste Bytebereich beginnen soll.
Eventuell werden mehrere Bereiche angegeben. Sie stehen für Teile der Datei, die der Server noch nicht empfangen hat. Dies ist nützlich, wenn eine Übertragung nach einer Unterbrechung fortgesetzt werden soll und der Client den Dienststatus nicht kennt.

Halten Sie sich bei der Festlegung der Größe der Bytebereiche immer an die unten beschriebenen bewährten Methoden. Gehen Sie nicht davon aus, dass **nextExpectedRanges** richtig dimensionierte Bytebereiche für einen Upload zurückgibt.
Die Eigenschaft **nextExpectedRanges** gibt Dateibereiche an, die noch nicht empfangen wurden. Sie ist nicht als Muster für den Dateiupload der App zu verstehen.

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

## <a name="remarks"></a>Hinweise

* Die Eigenschaft `nextExpectedRanges` listet nicht immer alle fehlenden Bereiche auf.
* Wird ein Segment geschrieben, gibt sie den nächsten Bereich zurück, ab dem begonnen wird (z. B. „523-“).
* Schlägt der Schreibvorgang fehl, weil der Client ein Fragment gesendet hat, das der Server bereits empfangen hat, antwortet der Server mit `HTTP 416 Requested Range Not Satisfiable`. Sie können den [Uploadstatus anfordern](#resuming-an-in-progress-upload), um eine detailliertere Liste der fehlenden Bereiche zu erhalten.
* Wenn Sie den Autorisierungsheader in den `PUT`-Aufruf einschließen, wird möglicherweise eine Antwort des Typs `HTTP 401 Unauthorized` zurückgegeben. Der Autorisierungsheader und das Bearertoken sollten nur mit dem `POST`-Aufruf im Rahmen von Schritt 1 gesendet werden. Der Autorisierungsheader sollte nicht in den `PUT`-Aufruf eingeschlossen werden.

## <a name="completing-a-file"></a>Vervollständigen einer Datei

Sobald der Server den letzten Bytebereich einer Datei empfängt, antwortet er mit `HTTP 201 Created` oder `HTTP 200 OK`.
Der Antworttext enthält auch die Standardeigenschaft, die für das **DriveItem** festgelegt wurde, das die vervollständigte Datei repräsentiert.

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

## <a name="handling-upload-conflicts"></a>Umgang mit Upload-Konflikten

Wenn ein Konflikt auftritt, nachdem die Datei hochgeladen wurde (während der Uploadsitzung wurde beispielsweise ein Element mit demselben Namen erstellt), wird ein Fehler zurückgegeben, wenn der letzte Bytebereich hochgeladen wurde.

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

## <a name="cancel-the-upload-session"></a>Abbrechen der Uploadsitzung

Wenn Sie eine Uploadsitzung abbrechen möchten, senden Sie eine DELETE-Anforderung an die Upload-URL. Das bereinigt die temporäre Datei, in der die bisher hochgeladenen Daten gespeichert sind. Verwenden Sie diese Vorgehensweise in Szenarios, in denen der Upload abgebrochen wird, beispielsweise bei Abbruch der Übertragung durch den Benutzer.

Temporäre Dateien und die zugehörigen Uploadsitzungen werden automatisch bereinigt, wenn der über **expirationDateTime** festgelegte Termin abgelaufen ist.
Temporäre Dateien werden eventuell nicht sofort gelöscht, nachdem die Ablaufzeit verstrichen ist.

### <a name="request"></a>Anforderung

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a>Antwort

Das folgende Beispiel zeigt die Antwort.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a>Fortsetzen eines laufenden Uploads

Wenn während einer Uploadanforderung die Verbindung getrennt wird oder anderweitig ausfällt, bevor die Anforderung abgeschlossen ist, werden alle Bytes in dieser Anforderung ignoriert. Dies kann passieren, wenn die Verbindung zwischen der App und dem Dienst getrennt wird. Tritt ein solcher Fall ein, kann die App die Dateiübertragung trotzdem ab dem letzten vollständig übertragenen Fragment fortsetzen.

Um herauszufinden, welche Bytebereiche bereits empfangen wurden, kann die App den Status der Uploadsitzung anfordern.

### <a name="example"></a>Beispiel

Sie können den Status des Uploads anfragen, indem Sie eine GET-Anforderung an `uploadUrl` senden.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

Der Server antwortet mit einer Liste der fehlenden Bytebereiche, die noch hochgeladen werden müssen, sowie mit dem Ablauftermin der Uploadsitzung.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a>Hochladen von verbleibenden Daten

Die App weiß jetzt, ab wo der Upload gestartet werden soll. Führen Sie nun die Schritte im Abschnitt [Hochladen von Bytes in die Uploadsitzung](#upload-bytes-to-the-upload-session) durch, um den Upload fortzusetzen.

## <a name="handle-upload-errors"></a>Behandeln von Fehlern beim Upload

Wenn der letzte Bytebereich einer Datei hochgeladen wird, kann ein Fehler auftreten. Dies kann an einem Namenskonflikt liegen oder daran, dass eine Kontingenteinschränkung überschritten wurde.
Die Uploadsitzung wird bis zur Ablaufzeit beibehalten. Dadurch kann Ihre App den Upload wiederherstellen, indem ein ausdrücklicher Commit der Uploadsitzung durchgeführt wird.

Um ausdrücklich einen Commit für die Uploadsitzung durchzuführen, muss Ihre App eine PUT-Anforderung mit einer neuen **driveItem**-Ressource durchführen, die für den Commit der Uploadsitzung verwendet wird.
Diese neue Anforderung sollte die Quelle der Fehler korrigieren, die den ursprünglichen Uploadfehler verursacht hat.

Um anzugeben, dass Ihre App einen Commit zu einer bestehenden Uploadsitzung durchführt, muss die PUT-Anforderung die `@microsoft.graph.sourceUrl`-Eigenschaft mit dem Wert Ihrer Uploadsitzungs-URL enthalten.

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

**Hinweis:** Sie können den `@microsoft.graph.conflictBehavior`- und `if-match`-Header wie erwartet in diesem Aufruf verwenden.

### <a name="http-response"></a>HTTP-Antwort

Wenn mithilfe der neuen Metadaten ein Commit für die Datei durchgeführt werden kann, wird die Fehlerantwort `HTTP 201 Created` oder `HTTP 200 OK` mit den Elementmetadaten für die hochgeladene Datei zurückgegeben.

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

## <a name="best-practices"></a>Bewährte Methoden

* Setzen Sie alle Uploads fort bzw. starten Sie alle Uploads neu, die wegen eines Verbindungsabbruchs oder einem 5xx-Fehler fehlschlagen, beispielsweise:
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* Verwenden Sie einen Exponential Backoff-Algorithmus, wenn beim Fortsetzen oder Neusenden einer Uploadanforderung 5xx-Serverfehler auftreten.
* Bei anderen Fehlern sollten Sie keinen Exponential Backoff-Algorithmus verwenden, sondern stattdessen die Anzahl der Wiederholungsversuche beschränken.
* Sollte bei fortsetzbaren Uploads der Fehler `404 Not Found` auftreten, starten Sie den gesamten Upload neu. Dies bedeutet, dass die Upload-Sitzung nicht mehr vorhanden ist.
* Verwenden Sie fortsetzbare Dateiübertragungen für Dateien, die größer als 10 MiB sind (10.485.760 Byte).
* Die optimale Größe eines Bytebereichs für stabile Highspeedverbindungen ist 10 MiB. Bei langsameren oder weniger zuverlässigen Verbindungen liefern kleinere Fragmentgrößen eventuell bessere Ergebnisse. Die empfohlene Fragmentgröße liegt zwischen 5 und 10 MiB.
* Verwenden Sie eine Bytebereichsgröße, die ein Vielfaches von 320 KiB ist (327.680 Byte) ist. Wenn Sie eine Fragmentgröße verwenden, die kein Vielfaches von 320 KiB ist, können Übertragungen großer Dateien nach Upload des letzten Bytebereichs fehlschlagen.

## <a name="error-responses"></a>Fehlerantworten

Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].

[error-response]: ../../../concepts/errors.md
[item-resource]: ../resources/driveitem.md
[fileSystemInfo]: ../resources/filesysteminfo.md

<!-- {
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/driveitem_createuploadsession.md:
      Found potential enums in resource example that weren't defined in a table:(rename,fail,replace) are in resource, but () are in table"
  ],
  "section": "documentation"
} -->
