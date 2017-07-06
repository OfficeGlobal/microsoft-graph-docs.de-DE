# <a name="create-page"></a>Seite erstellen

Dient zum Erstellen einer neuen OneNote-Seite im Standardabschnitt des Standardnotizbuchs.

Um eine Seite in einem anderen Abschnitt des Standardnotizbuchs zu erstellen, können Sie den Abfrageparameter `sectionName` verwenden.  Beispiel: `../onenote/pages?sectionName=My%20section`

Der `POST /onenote/pages`-Vorgang wird nur verwendet, um Seiten im Standardnotizbuch des aktuellen Benutzers zu erstellen. Wenn andere Notizbücher Ihr Ziel sind, können Sie [Seiten in einem angegebenen Abschnitt erstellen](../api/section_post_pages.md).           
## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:  

Notes.Create, Notes.ReadWrite oder Notes.ReadWrite.All

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
```

## <a name="request-headers"></a>Anforderungsheader  
| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |
| Content-Type | string | `text/html` oder `application/xhtml+xml` für den HTML-Inhalt, auch für den erforderlichen Teil „Präsentation“ von mehrteiligen Anforderungen. Mehrteilige Anforderungen verwenden den Inhaltstyp `multipart/form-data; boundary=your-boundary`. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext den HTML-Inhalt für die Seite an.

Der Text kann HTML-Code enthalten, der direkt im Anforderungstext platziert ist, oder er kann ein mehrteiliges Nachrichtenformat enthalten, wie im Beispiel gezeigt. Wenn Sie Binärdaten senden, müssen Sie eine mehrteilige Anforderung senden.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein neues [page](../resources/page.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.

Im Pfad `../onenote/pages` können Sie den Abfrageparameter `sectionName` verwenden, um eine Seite in einem bestimmten Abschnitt des Standardnotizbuchs zu erstellen. Beispiel: `../onenote/pages?sectionName=My%20section`. Wenn der Abschnitt nicht vorhanden ist (oder umbenannt wurde), erstellt die API einen neuen Abschnitt.

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Content-length: 312
Content-type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with <i>rendered</i> images and an <b>attached</b> file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an online source:</p>
    <img src="http://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as binary data:</p>
    <img src="name:imageBlock1" alt="an image on the page" width="300" />
    <p>Here's a file attachment:</p>
    <object data-attachment="FileName.pdf" data="name:fileBlock1" type="application/pdf" />
  </body>
</html>

--MyPartBoundary198374
Content-Disposition:form-data; name="imageBlock1"
Content-Type:image/jpeg

... binary image data ...

--MyPartBoundary198374
Content-Disposition:form-data; name="fileBlock1"
Content-Type:application/pdf

... binary file data ...

--MyPartBoundary198374--
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "content": "content-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->