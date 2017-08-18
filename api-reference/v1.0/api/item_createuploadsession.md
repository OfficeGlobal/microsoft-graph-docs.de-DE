# <a name="upload-large-files-with-an-upload-session"></a>Große Dateien mit einer Uploadsitzung hochladen

Wenn Sie eine Uploadsitzung erstellen, kann Ihre App Dateien bis zur maximal zulässigen Dateigröße hochladen. Eine Uploadsitzung erlaubt es der App, Bereiche einer Datei in sequenziellen API-Anfragen hochzuladen. Bricht die Verbindung während des Uploads ab, kann die Übertragung so anschließend fortgesetzt werden.

Sie müssen zwei Schritte durchführen, um eine Datei mit einer Uploadsitzung hochzuladen:

1. [Erstellen einer Uploadsitzung](#create-an-upload-session)
2. [Hochladen von Bytes in die Uploadsitzung](#upload-bytes-to-the-upload-session)

## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:

* Files.ReadWrite
* Files.ReadWrite.All
* Sites.ReadWrite.All

> **Hinweis**: Die Anwendungsberechtigung „Files.ReadWrite.All“ wird für diese API noch nicht unterstützt. Vollständige Unterstützung soll in Kürze folgen. 

## <a name="create-an-upload-session"></a>Erstellen einer Uploadsitzung

Um eine große Datei hochladen zu können, muss die App zuerst eine neue Uploadsitzung anfordern. Es wird dann ein temporärer Speicherort erstellt, an dem die Bytes der Datei gespeichert werden, bis sie vollständig hochgeladen ist. Sobald das letzte Byte der Datei hochgeladen wurde, ist die Uploadsitzung abgeschlossen, und die endgültige Datei wird im Zielordner angezeigt.

### <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root:/{path-to-item}:/createUploadSession
POST /me/drive/items/{parent-item-id}:/{filename}:/createUploadSession
```

### <a name="request-body"></a>Anforderungstext
Es ist kein Anforderungstexts erforderlich. Allerdings können Sie einen Anforderungstext definieren, um zusätzliche Daten zu der hochzuladenden Datei anzugeben.

Beispielsweise können Sie im Anforderungstext die Eigenschaft „conflictBehavior“ definieren, um festzulegen, wie vorgegangen werden soll, wenn der Dateiname bereits anderweitig in Verwendung ist.

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


### <a name="response"></a>Antwort
Die Antwort auf diese Anforderung enthält die Details der neu erstellten Ressource des Typs [uploadSession](../resources/uploadsession.md), einschließlich der zum Upload der Dateiteile verwendeten URL. 

### <a name="example"></a>Beispiel

<!-- {
  "blockType": "request",
  "name": "driveItem_createUploadSession"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createUploadSession
```

##### <a name="response"></a>Antwort 

Das folgende Beispiel zeigt die Antwort.

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

## <a name="upload-bytes-to-the-upload-session"></a>Hochladen von Bytes in die Uploadsitzung

Zum Hochladen der Datei oder eines Teils der Datei sendet die App eine PUT-Anfrage an den Wert **uploadUrl**, der ihr in der **createUploadSession**-Antwort übermittelt wurde. Sie können die gesamte Datei hochladen oder die Datei in Fragmente aufteilen, vorausgesetzt, die maximale Bytezahl pro Anforderung bleibt unter 60 MiB. Die Dateifragmente müssen sequenziell in der richtigen Reihenfolge hochgeladen werden. Werden die Fragmente in der falschen Reihenfolge hochgeladen, tritt ein Fehler auf.

**Hinweis:** Wenn die App eine Datei in mehrere Fragmente aufteilt, **MUSS** die Größe jedes Fragments ein Vielfaches von 320 KiB sein. Bei Fragmentgrößen, die sich nicht ohne Rest durch 320 teilen lassen, treten beim Commit einiger Dateien Fehler auf.

### <a name="example"></a>Beispiel

In diesem Beispiel werden die ersten 26 Byte einer 128-Byte-Datei hochgeladen. Der Header **Content-Length** definiert die Größe der aktuellen Anforderung. Der Header **Content-Range** gibt den Bytebereich in der Gesamtdatei an, den diese Anforderung repräsentiert. Die Gesamtlänge der Datei muss bekannt sein, bevor Sie das erste Fragment der Datei hochladen können.

<!-- { "blockType": "request", "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->
```
PUT https://tenant-my.sharepoint.com/alkjl1kjklna
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

**Wichtig:** Die App muss sicherstellen, dass die im Header **Content-Range** angegebene Gesamtdateigröße bei allen Anforderungen identisch ist. Wird für ein Fragment eine andere Dateigröße deklariert, schlägt die betreffende Anforderung fehl.

##### <a name="response"></a>Antwort

Das folgende Beispiel zeigt die Antwort.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

Die App kann mithilfe des Werts **nextExpectedRanges** bestimmen, wo das nächste Fragment beginnen soll. Eventuell werden mehrere Bereichen angegeben. Sie stehen für Teile der Datei, die der Server noch nicht empfangen hat. Dies ist nützlich, wenn eine Übertragung nach einer Unterbrechung fortgesetzt werden soll und der Client den Dienststatus nicht kennt.

Halten Sie sich bei der Festlegung der Fragmentgröße immer an die unten beschriebenen bewährten Methoden. Gehen Sie nicht davon aus, dass **nextExpectedRanges** richtig dimensionierte Bereiche für ein Uploadfragment zurückgeben wird. Die Eigenschaft **nextExpectedRanges** gibt Dateibereiche an, die noch nicht empfangen wurden. Sie ist nicht als Muster für den Dateiupload zu verstehen.

**Hinweise:**

* Die Eigenschaft `nextExpectedRanges` listet nicht immer alle fehlenden Bereiche auf.
* Wird ein Segment geschrieben, gibt sie den nächsten Bereich zurück, ab dem begonnen wird (z. B. „523-“).
* Schlägt der Schreibvorgang fehl, weil der Client ein Fragment gesendet hat, das der Server bereits empfangen hat, antwortet der Server mit `HTTP 416 Requested Range Not Satisfiable`. Sie können den [Uploadstatus anfordern](#resuming-an-in-progress-upload), um eine detailliertere Liste der fehlenden Bereiche zu erhalten.
* Einschließlich des Autorisierungsheaders bei der Ausgabe von `PUT` kann der Aufruf zu einer `HTTP 401 Unauthoized`-Antwort führen. Der Autorisierungsheader und das Bearertoken sollten nur gesendet werden, wenn `POST` während des ersten Schritts ausgegeben wird. Beim Ausgeben von `PUT` sollte es nicht eingeschlossen werden.   


## <a name="completing-a-file"></a>Vervollständigen einer Datei

Sobald der Server das letzte Fragment einer Datei empfängt, antwortet er mit `HTTP 201 Created` oder `HTTP 200 OK`. Der Antworttext enthält auch die Standardeigenschaft, die für das **DriveItem** festgelegt wurde, das die vervollständigte Datei repräsentiert.

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
**Hinweis:** Die Elementantwort ist aus Gründen der Dokumentationsübersichtlichkeit abgeschnitten.

## <a name="cancel-an-upload-session"></a>Abbrechen einer Uploadsitzung

Wenn Sie eine Uploadsitzung abbrechen möchten, senden Sie eine DELETE-Anforderung an die Upload-URL. Das bereinigt die temporäre Datei, in der die bisher hochgeladenen Daten gespeichert sind. Verwenden Sie diese Vorgehensweise in Szenarios, in denen der Upload abgebrochen wird, beispielsweise bei Abbruch der Übertragung durch den Benutzer.

Temporäre Dateien und die zugehörigen Uploadsitzungen werden automatisch bereinigt, wenn der über **expirationDateTime** festgelegte Termin abgelaufen ist.

### <a name="example"></a>Beispiel

Die DELETE-Anforderung führt zum sofortigen Ablauf der Uploadsitzung und entfernt alle zuvor hochgeladenen Bytes.

<!-- { "blockType": "request", "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->
```http
DELETE https://tenant-my.sharepoint.com/alkjl1kjklna
```

##### <a name="response"></a>Antwort 

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

<!-- { "blockType": "request", "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->
```
GET https://tenant-my.sharepoint.com/alkjl1kjklna
```

Der Server antwortet mit einer Liste der fehlenden Bytebereiche, die noch hochgeladen werden müssen, sowie mit dem Ablauftermin der Uploadsitzung.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->
```http
HTTP/1.1 200 OK

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a>Hochladen von verbleibenden Daten
Die App weiß jetzt, ab wo der Upload gestartet werden soll. Führen Sie nun die Schritte im Abschnitt [Hochladen von Bytes in die Uploadsitzung](#upload-bytes-to-the-upload-session) durch, um den Upload fortzusetzen.


## <a name="best-practices"></a>Bewährte Methoden

* Setzen Sie alle Uploads fort bzw. starten Sie alle Uploads neu, die wegen eines Verbindungsabbruchs oder einem 5xx-Fehler fehlschlagen, beispielsweise:
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* Verwenden Sie einen Exponential Backoff-Algorithmus, wenn beim Fortsetzen oder Neusenden einer Uploadanforderung 5xx-Serverfehler auftreten.
* Bei anderen Fehlern sollten Sie keinen Exponential Backoff-Algorithmus verwenden, sondern stattdessen die Anzahl der Wiederholungsversuche beschränken.
* Sollte bei fortsetzbaren Uploads der Fehler `404 Not Found` auftreten, starten Sie den gesamten Upload neu.
* Verwenden Sie fortsetzbare Dateiübertragungen für Dateien, die größer als 10 MiB sind (10 \* 1.024 \* 1.024 Byte).
* Die optimale Dateigröße für stabile Highspeedverbindungen ist 10 MiB. Bei langsameren oder weniger zuverlässigen Verbindungen liefern kleinere Fragmentgrößen eventuell bessere Ergebnisse. Die empfohlene Fragmentgröße liegt zwischen 5 und 10 MiB.
* Verwenden Sie eine Fragmentgröße, die ein Vielfaches von 320 KiB ist (320 \* 1.024 Byte). Wenn Sie eine Fragmentgröße verwenden, die kein Vielfaches von 320 KiB ist, können Übertragungen großer Dateien nach Upload des letzten Fragments fehlschlagen.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
