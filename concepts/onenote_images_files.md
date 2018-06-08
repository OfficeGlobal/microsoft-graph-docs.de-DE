
# <a name="add-images-videos-and-files-to-onenote-pages"></a>Hinzufügen von Bildern, Videos und Dateien zu OneNote-Seiten

*__Gilt für:__ Heimanwender-Notizbücher in OneDrive | Unternehmensnotizbücher in Office 365*

Sie können Elemente der Typen **img**, **object** und **iframe** verwenden, um bei der [Erstellung](onenote-create-page.md) oder [Aktualisierung](onenote_update_page.md) von OneNote-Seiten Bilder, Videos und Dateien zur Seite hinzuzufügen. 

- Verwenden Sie **img**, um ein Bild auf der Seite zu rendern.
- Verwenden Sie **iframe**, um ein Video in die Seite einzubetten.
- Verwenden Sie **object**, um der Seite eine Dateianlage hinzuzufügen.


<a name="images"></a>
## <a name="adding-images"></a>Hinzufügen von Bildern

Bilder können mittels URL-Verweis oder durch das Senden von Rohdaten hinzugefügt werden. Microsoft Graph unterstützt die folgenden Methoden zum Hinzufügen von Bildern, Logos und Fotos zu OneNote-Seiten: 

[Hinzufügen öffentlicher Bilder aus dem Internet](#add-a-public-image-from-the-web)  
Verwenden Sie `img` mit `src="http://image-url"`, und geben Sie die URL eines öffentlich zugänglichen Bilds an. Das Bild wird auf der OneNote-Seite gerendert.</p>
[Hinzufügen von Bildern mithilfe von Binärdaten](#add-an-image-using-binary-data)</p>
Verwenden Sie `img` mit `src="name:image-block-name"`, und senden Sie die Bilddatei in einem Datenteil einer mehrteiligen Anforderung. Das Bild wird auf der OneNote-Seite gerendert.</p>
[Hinzufügen von Webseitenmomentaufnahmen](#add-a-webpage-snapshot)</p>
Verwenden Sie `img` mit `data-render-src="http://webpage-url"`, und geben Sie die URL einer Webseite an. Auf der OneNote-Seite wird eine Momentaufnahme der gesamten Webseite gerendert.</p>
[Hinzufügen von HTML-basiert gerenderten Bildern](#add-an-image-rendered-from-html)</p>
Verwenden Sie `img` mit `data-render-src="name:html-block-name"`, und senden Sie HTML-Code in einem Datenteil einer mehrteiligen Anforderung. Der HTML-Code wird auf der OneNote-Seite als Bild gerendert.</p>
[Hinzufügen von Bildern von PDF-Inhalten](#add-images-of-pdf-file-contents)</p>
Verwenden Sie `<img data-render-src="name:part-name" />`, und senden Sie die PDF-Datei in einem Datenteil einer mehrteiligen Anforderung. Jede PDF-Seite wird auf der OneNote-Seite als separates Bild gerendert.</p>
[Hinzufügen von Bilddateien als Dateianlage](#add-an-image-file-as-an-attachment)</p>
Verwenden Sie `object` mit `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"`, und senden Sie eine Bilddatei in einem Datenteil einer mehrteiligen Anforderung. Der OneNote-Seite wird eine Dateianlage hinzugefügt, und es wird ein Dateisymbol angezeigt.</p>

> **Hinweis:** Zum Abrufen von Bildern auf einer OneNote-Seite müssen Sie zunächst die [Seiteninhalte per GET-Anforderung abrufen](onenote-get-content.md#page-html-content). Das gibt die URLs der Bildressourcen auf der Seite zurück. Dann senden Sie separat [eine GET-Anforderung je Bildressource](onenote-get-content.md#image-or-other-file-resource).


**Bildattribute** 

Elemente des Typs **img** können optional Attribute der Typen **alt**, **height** und **width** enthalten sowie die Formatattribute **max-width** und **max-height**.

**Bildmedientypen**

Microsoft Graph unterstützt die Bildtypen TIFF, PNG, GIF, JPEG und BMP. Soll ein anderes Bildformat ohne vorherige Konvertierung dargestellt werden, müssen Sie [die Binärdaten senden](#add-an-image-using-binary-data), in einer mehrteiligen Anforderung. Base64 muss nicht verwendet werden, und auch eine anderweitige Codierung der gesendeten Binärdaten ist nicht erforderlich.

> **Hinweis:** Die API erkennt den ursprünglichen Eingabebildtyp und gibt ihn als Attribut **data-fullres-src-type** im [Ausgabe-HTML-Code](onenote_input_output_html.md#output-html) zurück. Daneben gibt die API auch den Bildtyp des optimierten Bilds zurück, in **data-src-type**.
 
Unter [Einschränkungen](#size-limitations-for-post-pages-requests) sind alle Einschränkungen aufgeführt, die bei der Erstellung von Seiten mit Medien gelten.


<a name="image-img-url-src"></a>
### <a name="add-a-public-image-from-the-web"></a>Hinzufügen öffentlicher Bilder aus dem Internet

Geben Sie im Eingabe-HTML-Code Ihrer Anforderung `<img src="http://..." />` an, und setzen Sie die URL eines öffentlich verfügbaren Bilds im Attribut **src**.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Public URL</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image from the web.</p>
    <img src="http://..." width="300"/>
  </body>
</html>

--MyAppPartBoundary--  
```

<a name="image-img-binary-src"></a>
### <a name="add-an-image-using-binary-data"></a>Hinzufügen von Bildern mithilfe von Binärdaten

Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<img src="name:part-name" />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der die binären Bilddaten enthält. Senden Sie die Binärdaten in unveränderter Form: Verwenden Sie weder Base64 noch eine andere Form der Codierung.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Image binary data</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the uploaded image.</p>
    <img src="name:image-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="MyAppPictureId"
Content-Type: image/jpeg

... image binary data ...

--MyAppPartBoundary--  
```


<a name="image-img-url-data-render-src"></a>
### <a name="add-a-webpage-snapshot"></a>Hinzufügen von Webseitenmomentaufnahmen

Sie können mit Microsoft Graph Momentaufnahmen ganzer Webseiten erstellen und in neue Seiten einfügen. Diese Methode ist nützlich, um Webseiten zu archivieren oder komplexe Webseiten mit Features abzubilden, die OneNote nicht unterstützt (beispielsweise bestimmte CSS-Formatierungen).  

Geben Sie im Eingabe-HTML-Code Ihrer Anforderung `<img src="http://..." />` an, und setzen Sie die URL der einzufügenden Webseite im Attribut **src**.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Webpage capture</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image of the webpage.</p>
    <img data-render-src="http://www.onenote.com" width="200"/>
  </body>
</html>

--MyAppPartBoundary--  
```


<a name="image-img-binary-data-render-src"></a>
### <a name="add-an-image-rendered-from-html"></a>Hinzufügen von HTML-basiert gerenderten Bildern
Wenn Sie den HTML-Code als Datenblock übergeben, dürfen darin weder aktive Inhalte enthalten sein, die Benutzeranmeldeinformationen erfordern, noch vorab geladene Browser-Plug-Ins. Das Modul, das Microsoft Graph verwendet, um die HTML-Seite als Bild zu rendern, kann Benutzer nicht anmelden und enthält keine Plug-Ins wie Adobe Flash oder Apple QuickTime. Das bedeutet außerdem: Dynamisch geladene Inhalte, beispielsweise in einem AJAX-Skript, werden nicht angezeigt, wenn zum Abrufen der Daten Benutzeranmeldeinformationen oder Cookies erforderlich sind.

Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<img data-render-src="name:part-name" />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der den HTML-Code enthält.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: HTML block</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the block of HTML as an image.</p>
    <img data-render-src="name:html-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="html-block-name"
Content-Type: text/html

<html>
<body>
<h1>This HTML will render as an image</h1>
<p><b>Don't</b> try to embed another <i>data-render-src</i> type-image inside the HTML part--
it won't work. Instead, use URL-based real images like this:</p>
<img src="http://cdn.onenote.net/1664161560_Images/OneNote.ico" />
</body>
</html>

--MyAppPartBoundary--  
```


<a name="image-object"></a>
### <a name="add-an-image-file-as-an-attachment"></a>Hinzufügen von Bilddateien als Anlage

Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der die binären Bilddaten enthält. Senden Sie die Binärdaten in unveränderter Form: Verwenden Sie weder Base64 noch eine andere Form der Codierung.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Binary image data as file attachment</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page contains the image as a file attachment.</p>
    <object data-attachment="image-file.jpg" data="name:image-block-name" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```

Weitere Informationen zu Dateimedientypen finden Sie unter [diesem Link](#file-media-types).



<a name="videos"></a>
## <a name="adding-videos"></a>Hinzufügen von Videos

Wenn Sie Videos in OneNote-Seiten einbetten möchten, können Sie `<iframe data-original-src="http://..." />` im Eingabe-HTML-Code verwenden. 

**Unterstützte Videowebsites**

- Dailymotion
- Office Mix
- Sway
- Sketchfab
- TED
- YouTube
- Vimeo
- Vine

**„iframe“-Attribute**

**data-original-src**</p>
Erforderlich. URL des Videos.<br />Beispiel: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</p>
**width**</p>
Optional. Breite des „iframe“-Elements, in dem das Video enthalten ist. Der Standardwert ist 480.<br />Beispiel: `width="300"`</p>
**height**</p>
Optional. Höhe des „iframe“-Elements, in dem das Video enthalten ist. Der Standardwert ist 360.<br />Beispiel: `height="300"`</p>

**Beispiel**

Geben Sie im Eingabe-HTML-Code Ihrer Anforderung `<iframe data-original-src="http://..." />` an, und setzen Sie die URL des Videos im Attribut **data-original-src**.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
    <head>
        <title>A page with an embedded video</title>
    </head>
    <body>
        <iframe data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" width="340" height="280"/>
    </body>
</html>

--MyAppPartBoundary--
```


<a name="files"></a>
## <a name="adding-files"></a>Hinzufügen von Dateien

Zum Hinzufügen von Dateianlagen zu OneNote-Seiten verwenden Sie ein Element des Typs **object** im Eingabe-HTML-Code. Wenn Sie eine PDF-Datei hinzufügen möchten, können Sie die einzelnen PDF-Seiten mithilfe eines Elements des Typs **img** als Bild rendern. 

[Hinzufügen von Dateianlagen](#add-a-file-attachment)</p>
Verwenden Sie `<object .../>`, und senden Sie die Datei in einem Datenteil einer mehrteiligen Anforderung. Der OneNote-Seite wird eine Dateianlage hinzugefügt, die als Dateisymbol angezeigt wird.</p>
[Hinzufügen von Bildern von PDF-Inhalten](#add-images-of-pdf-file-contents)</p>
Verwenden Sie `<img data-render-src="name:part-name" />`, und senden Sie eine PDF-Datei in einem Datenteil einer mehrteiligen Anforderung. Jede PDF-Seite wird auf der OneNote-Seite als separates Bild gerendert.</p>

**Dateiattribute**

Elemente des Typs **object** erfordern die folgenden Attribute:

**data-attachment**</p>
Name und Dateierweiterung der Datei, die auf der OneNote-Seite angezeigt werden soll<br />Beispiel: `data-attachment="filename.docx"`</p>
**data**</p>
Name des Textteils in der mehrteiligen Anforderung, der die binären Dateidaten enthält. Microsoft Graph bietet keine Unterstützung für die Übergabe von URL-Verweisen in diesem Attribut.<br />Beispiel: `data="name:part-name"`</p>
**type**</p>
Medientyp der Datei. Er legt fest, welches Dateisymbol auf der Seite angezeigt werden soll und welche Anwendung gestartet wird, sobald der Benutzer die Datei auf dem Gerät über OneNote aktiviert.<br />Beispiel: `type="application/pdf"`</p>


<a name="file-media-types"></a>

### <a name="file-media-types"></a>Dateimedientypen  
Microsoft Graph verwendet für angefügte Dateien vordefinierte Dateitypensymbole. Erkennt die API den Dateityp nicht, wird ein generisches Symbol verwendet. Nachfolgend sind verschiedene häufig vorkommende Dateitypen aufgeführt, die von der API erkannt werden:

- application/pdf  
- application/vnd.openxmlformats-officedocument.wordprocessingml.document  
- application/vnd.openxmlformats-officedocument.presentationml.presentation
- application/vnd.openxmlformats-officedocument.spreadsheetml.sheet
- image/png
- image/jpeg
- image/gif
- audio/wav
- video/mp4
- application/msword
- application/mspowerpoint
- application/excel

Unter [Einschränkungen](#size-limitations-for-post-pages-requests) sind alle Einschränkungen aufgeführt, die bei der Erstellung von Seiten mit Medien gelten.


<a name="file-object"></a>
### <a name="add-a-file-attachment"></a>Hinzufügen von Dateianlagen

Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der die binären Dateidaten enthält. Senden Sie die Binärdaten in unveränderter Form: Verwenden Sie weder Base64 noch eine andere Form der Codierung.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image file attachment</title>
  </head>
  <body>
    <p>This is an image file attachment.</p>
    <object data-attachment="Logo.jpg" data="name:logo1-file" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```


<a name="file-binary-data-render-src"></a>
### <a name="add-images-of-pdf-file-contents"></a>Hinzufügen von Bildern von PDF-Inhalten

Geben Sie im Eingabe-HTML-Code im Teil **Presentation** Ihrer Anforderung `<img data-render-src="name:part-name" ... />` an. Dabei ist *part-name* der eindeutige Bezeichner des Datenteils in Ihrer [mehrteiligen Anforderung](onenote-create-page.md#example-request), der die binären Dateidaten enthält. Senden Sie die Binärdaten in unveränderter Form: Verwenden Sie weder Base64 noch eine andere Form der Codierung.

```
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with images of the pages of a PDF file</title>
  </head>
  <body>
    <p>The pages of this PDF file render as images.</p>
    <img data-render-src="name:file-part" alt="PDF file as images" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="file-part"
Content-Type: application/pdf

... binary file data ...

--MyAppPartBoundary--  
```


<a name="size-limits"></a>
## <a name="size-limitations-for-post-pages-requests"></a>Größenbeschränkungen bei Anforderungen des Typs „Post pages“

Für das Senden von Bild- und Dateidaten gelten folgende Einschränkungen: <!--TODO: check these-->

- Die maximal zulässige Gesamtgröße von POST-Anforderungen liegt bei etwa 70 MB, einschließlich Bildern, Dateien und anderer Daten. Das tatsächlich Limit hängt von der Downstreamcodierung ab, daher ist keine feste Bytezahl als Höchstgrenze gesetzt. Anforderungen, die das Limit überschreiten, geben möglicherweise unzuverlässige Ergebnisse zurück.

- Die maximal zulässige Größe pro Datenteil liegt bei 25 MB, einschließlich des Headers des jeweiligen Teils. Datenteile, die dieses Limit überschreiten, werden von Microsoft Graph abgelehnt. 

- Die maximal zulässige Anzahl von Bildern pro Seite beträgt 150. Bei Verwendung des Attributs `src="http://..."` ignoriert die API alle Tags des Typs **img**, die über dieses Limit hinausgehen.

- Die maximal zulässige Anzahl von Datenteilen pro POST-Anforderung liegt bei 6, einschließlich des zwingend erforderlichen Teils **Presentation**.

- Jede Anforderung darf bis zu 5 Elemente des Typs **img** enthalten, die **data-render-src** verwenden, sowie 1 Element des Typs **object**, das **data-render-src** verwendet. Alle weiteren Bild- und Dateiverweise werden ignoriert.

- Die maximal zulässige Anzahl von Bildern pro POST-Anforderung liegt bei 30, unabhängig von der Methode, über die sie an die API gesendet werden. Alle weiteren Bilder werden ignoriert. Wenn Sie eine Webseite mit vielen Bildern abbilden möchten, empfiehlt sich die [Erstellung einer Momentaufnahme der gesamten Seite](#add-a-webpage-snapshot).


## <a name="when-to-use-html-versus-data-render-src"></a>Anwendungsfälle: HTML vs. *data-render-src* 
Ob Sie den HTML-Code direkt auf der OneNote-Seite einfügen oder das Attribut **data-render-src** verwenden sollten, hängt von verschiedenen Faktoren ab. Berücksichtigen Sie bei Ihrer Entscheidung Folgendes:

- Komplexer HTML-Code sollte per **data-render-src** an das Renderingmodul gesendet werden. Eine manuelle Anpassung des HTML-Codes an die Anforderungen von Microsoft Graph empfiehlt sich nicht. Dies gilt auch für HTML-Code mit nicht unterstützten Tags.

- Für akkurates Seitenrendering unter Beibehaltung des Layouts und Designs der Seite empfiehlt sich die Verwendung des Renderingmoduls per **data-render-src**.

- Bei direkt bearbeitbarem Text sollte der HTML-Code direkt auf der Seite eingefügt werden. Gerenderte Bilder werden zwar von einem System für optische Zeichenerkennung (OCR, Optical Character Recognition) gescannt, dieses System liefert jedoch keine gleichwertigen Ergebnisse.

- Momentaufnahmen bestimmter Zeitpunkte zu Verlaufs- oder Archivierungszwecken sollten mithilfe der Methode „data-render-src“ angefertigt werden.

- **data-render-src** eignet sich hervorragend, um einem Webseitendesign Überarbeitungshinweise hinzuzufügen. Mit den Freihandfunktionen von OneNote können Sie Änderungen auf dem Bild markieren oder wichtige Bereiche hervorheben. Ist die betreffende Webseite ein Bild, gestaltet sich das sehr viel einfacher.

- Sehr große Bilder oder Bilder in Formaten, die OneNote nicht direkt unterstützt, lassen sich mit dem Attribut **data-render-src** mitunter einfacher als Miniaturansicht anzeigen und konvertieren, als dies mit eigenem Code möglich wäre. Selbst wenn das Bild auch online verfügbar ist: Wenn Sie die Daten in die POST-Anforderung einbetten, steht die Seitenabbildung OneNote-Benutzern manchmal schneller zur Verfügung, da zur Erstellung der OneNote-Seite insgesamt weniger Roundtrips nötig sind.

Manchmal können Sie am einfachsten herausfinden, welche Methode für Ihre Benutzer die beste ist, indem sie während der App-Entwicklung beide Varianten testen.


<a name="permissions"></a>
## <a name="permissions"></a>Berechtigungen

Zum Erstellen oder Aktualisieren von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern. Wählen Sie die niedrigste Stufe, die erforderlich ist, damit Ihre App korrekt funktioniert.

**Berechtigungen für _POST pages_**

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All 

**Berechtigungen für _PATCH pages_**

- Notes.ReadWrite
- Notes.ReadWrite.All

Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie im Artikel zum Thema [OneNote-Berechtigungsbereiche](permissions_reference.md#notes-permissions).


<a name="see-also"></a>
## <a name="additional-resources"></a>Weitere Ressourcen

- [Integrieren mit OneNote](integrate_with_onenote.md)
- [OneNote-Entwicklerblog](http://go.microsoft.com/fwlink/?LinkID=390183)
- [Fragen zur OneNote-Entwicklung auf Stack Overflow](http://go.microsoft.com/fwlink/?LinkID=390182)
- [GitHub-Repositorys für OneNote](http://go.microsoft.com/fwlink/?LinkID=390178)  
