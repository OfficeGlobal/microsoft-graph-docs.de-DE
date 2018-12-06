---
title: Erstellen von OneNote-Seiten
description: " Enterprise-Notizbücher in Office 365"
ms.openlocfilehash: 73ff77b16aaf5927bf28d009ca8ee1274f954c06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092345"
---
# <a name="create-onenote-pages"></a>Erstellen von OneNote-Seiten

**Gilt für**: Heimanwender-Notizbücher in OneDrive | Unternehmensnotizbücher in Office 365

Zum Erstellen einer OneNote-Seite senden Sie eine POST-Anforderung an einen *pages*-Endpunkt. Beispiel:

`POST ../notes/sections/{id}/pages`

<br/>

Senden Sie den HTML-Code, der die Seite definiert, im Nachrichtentext. Wenn die Anforderung erfolgreich ist, gibt Microsoft Graph den HTTP-Statuscode 201 zurück.


> **Hinweis:** Informationen zu den POST-Anforderungen, mit denen Sie Abschnitte, Abschnittsgruppen und Notizbücher erstellen können, finden Sie in der [interaktiven REST-Referenz](https://dev.onenote.com/docs).


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>Erstellen des Anforderungs-URI

Um den URI der POST-Anforderung zu erstellen, beginnen Sie mit der Stamm-URL des Diensts:

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

Fügen Sie dann den *pages*-Endpunkt an:

- **Erstellen einer Seite in einem beliebigen Abschnitt (angegeben durch den Abschnittsnamen)**<br/><br/>`.../pages?sectionName=DefaultSection`

- **Erstellen einer Seite in einem beliebigen Abschnitt (angegeben durch die ID)**<br/><br/>`.../sections/{section-id}/pages` 

Wenn Sie Seiten im persönlichen Notizbuch des Benutzers erstellen, bietet Microsoft Graph auch Endpunkte, die Sie zum Erstellen von Seiten im Standardnotizbuch verwenden können:

- **Erstellen einer Seite im Standardabschnitt des Standardnotizbuchs**<br/><br/>`../pages` 



Ihr vollständiger Anforderungs-URI gleicht einem der folgenden Beispiele:

- `https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?sectionName=Homework`

Hier erfahren Sie mehr über die [Stamm-URL des Diensts](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).

<a name="post-pages-section-name"></a>

### <a name="using-the-sectionname-url-parameter"></a>Verwenden des URL-Parameters *sectionName*

Die folgenden Regeln gelten bei Verwendung des *sectionName*-Parameters zum Erstellen einer Seite in einem benannten Abschnitt im Standardnotizbuch:

- Nur auf Abschnitte auf oberster Ebene kann verwiesen werden (keine Abschnitte in Abschnittsgruppen).

- Ist im Standardnotizbuch kein Abschnitt mit dem angegebenen Namen vorhanden, wird er von der API erstellt. Die folgenden Zeichen sind für Abschnittsnamen nicht zulässig: `? * \ / : < > | & # " % ~`

- Beim Abgleich von Abschnittsnamen wird die Groß-und Kleinschreibung nicht beachtet, aber beim Erstellen von Abschnitten bleibt die Groß-/Kleinschreibung erhalten. Somit wird z. B. „Mein neuer Abschnitt“ genau so angezeigt, aber „mein neuer abschnitt“ würde bei nachfolgenden Übermittlungen ebenfalls übereinstimmen.

- Abschnittsnamen müssen URL-codiert sein. Z. B. müssen Leerzeichen als *%20* codiert werden.

- Der *sectionName*-Parameter gilt nur für die Route `../notes/pages` (nicht für `../notes/sections/{id}/pages`).

Da Abschnitte erstellt werden, wenn sie noch nicht vorhanden sind, ist es sicherer, diesen Aufruf mit jeder Seite zu verwenden, die Ihre App erstellt. Benutzer können Abschnitte möglicherweise umbenennen, doch die API erstellt einen neuen Abschnitt mit dem Abschnittsnamen, den Sie angeben. 

> **Hinweis:** Die von der API zurückgegebenen Links für Seiten in einem umbenannten Abschnitt führen weiterhin zu den betreffenden älteren Seiten. 


<a name="message-body"></a>

## <a name="construct-the-message-body"></a>Erstellen des Nachrichtentexts

Der HTML-Code, der Seiteninhalt definiert, wird als *Eingabe-HTML* bezeichnet. Eingabe-HTML unterstützt eine [Teilmenge der Standard-HTML und -CSS](#supported-html-and-css-for-onenote-pages) mit zusätzlichen benutzerdefinierten Attributen. (Benutzerdefinierte Attribute, wie **data-id** und **data-render-src**, werden in [Eingabe- und Ausgabe-HTML](onenote-input-output-html.md) beschrieben.) 

Senden Sie die Eingabe-HTML im Nachrichtentext der POST-Anforderung. Sie können die Eingabe-HTML direkt im Nachrichtentext mit dem Inhaltstyp `application/xhtml+xml` oder `text/html` senden, oder Sie können sie im „Presentation“-Teil einer mehrteiligen Anforderung senden. 

Das folgende Beispiel sendet die Eingabe-HTML direkt im Nachrichtentext.

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: application/xhtml+xml

<!DOCTYPE html>
<html>
  <head>
    <title>A page with a block of HTML</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>This page contains some <i>formatted</i> <b>text</b> and an image.</p>
    <img src="https://..." alt="an image on the page" width="500" />
  </body>
</html>
```

<br/>

Wenn Sie Binärdaten senden, müssen Sie eine [mehrteilige Anforderung](#example-request) verwenden. 

> **Hinweis:** Zur Vereinfachung der Programmierung und Konsistenz in Ihrer App können Sie mehrteilige Anforderungen verwenden, um alle Seiten zu erstellen. Es ist ratsam, eine Bibliothek zu verwenden, um mehrteilige Nachrichten zu erstellen. Dadurch wird das Risiko der Erstellung von fehlerhaften Nutzlasten reduziert.


<a name="input-html-rules"></a>

### <a name="requirements-and-limitations-for-input-html-in-post-pages-requests"></a>Anforderungen und Einschränkungen für Eingabe-HTML in POST-Anforderungen

Beachten Sie beim Senden von Eingabe-HTML diese allgemeinen Anforderungen und Einschränkungen:  

- Die Eingabe-HTML sollte UTF-8-codierter und wohlgeformter XHTML-Code sein. Für alle Container-Starttags müssen die entsprechenden schließenden Tags vorhanden sein. Alle Attributwerte müssen in doppelte oder einzelne Anführungszeichen eingeschlossen werden.  <!--docs say MUST be encoded-->

- JavaScript-Code, hinzugefügte Dateien und CSS werden entfernt. 

- HTML-Formulare werden vollständig entfernt.  

- Microsoft Graph unterstützt eine [Teilmenge der HTML-Elemente](#supported-html-and-css-for-onenote-pages). 

- Microsoft Graph unterstützt eine Teilmenge der allgemeinen HTML-Attribute und eine Reihe von benutzerdefinierten Attributen, z. B. das **data-id**-Attribut, das für das Aktualisieren von Seiten verwendet wird. Unterstützte Attribute finden Sie unter [Eingabe- und Ausgabe-HTML](onenote-input-output-html.md).


<a name="supported-html"></a>

### <a name="supported-html-and-css-for-onenote-pages"></a>Unterstützte HTML und CSS für OneNote-Seiten

Nicht alle Elemente, Attribute und Eigenschaften werden (in HTML4, XHTML, CSS, HTML5 usw.) unterstützt. Stattdessen akzeptiert Microsoft Graph einen eingeschränkten Satz von HTML-Elementen, der der üblichen Verwendung von OneNote besser entspricht. Weitere Informationen finden Sie unter [Unterstützung von HTML-Tags für Seiten](https://dev.onenote.com/docs#/introduction/html-tag-support-for-pages). Wenn ein Tag dort nicht aufgeführt ist, wird es wahrscheinlich ignoriert.

<!--Microsoft Graph only accepts UTF-8 data. Be sure that all requests are encoded that way, and your content-type headers indicate that as well. xx our examples don't show this-->

Die folgende Liste zeigt die grundlegenden Elementtypen, die Microsoft Graph unterstützt:

- `<head>` und `<body>`</p>
- `<title>` und `<meta>`, die den Seitentitel und das Erstellungsdatum festlegen</p>
- `<h1>` bis `<h6>` für Abschnittsüberschriften</p>
- `<p>` für Absätze</p>
- `<ul>`, `<ol>` und `<li>` für Listen und Listenelemente</p>
- `<table>`, `<tr>` und `<td>`, einschließlich geschachtelter Tabellen</p>
- `<pre>` für vorformatierten Text (behält Leerräume und Zeilenumbrüche bei)</p>
- `<b>` und `<i>` für fette und kursive Zeichenformate</p>

Microsoft Graph behält den semantischen Inhalt und die grundlegende Struktur der Eingabe-HTML bei der Seitenerstellung bei, konvertiert jedoch die Eingabe-HTML in die unterstützte Teilmenge von HTML und CSS. Features, die in OneNote nicht vorhanden sind, können nicht übersetzt werden und werden somit möglicherweise in der HTML-Quelldatei nicht erkannt. 


<a name="example"></a>

## <a name="example-request"></a>Beispielanforderung

Dieses Beispiel einer mehrteiligen Anforderung erstellt eine Seite, die Bilder und eine eingebettete Datei enthält. Der erforderliche **Presentation**-Teil enthält die Eingabe-HTML, die die Seite definiert. Der **imageBlock1**-Teil enthält die binären Bilddaten und **fileBlock1** die Binärdateidaten. Datenteile können auch HTML enthalten. In diesem Fall [rendert Microsoft Graph den HTML-Code als Bild](onenote-images-files.md#add-an-image-using-binary-data) auf der OneNote-Seite. 

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with rendered images and an attached file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an <i>online source</i>:</p>
    <img src="https://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as <b>binary data</b>:</p>
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

Weitere Beispiele für die Erstellung von Seiten, die Bilder und andere Dateien enthalten, finden Sie unter [Hinzufügen von Bildern und Dateien](onenote-images-files.md) sowie in unseren [Lernprogrammen](https://docs.microsoft.com/de-DE/previous-versions/office/office-365-api/how-to/onenote-tutorial) und [Beispielen](https://github.com/onenotedev). Außerdem finden Sie Informationen zum [Erstellen absolut positionierter Elemente](onenote-abs-pos.md), [Verwenden von Notiztags](onenote-note-tags.md) und [Extrahieren von Daten](onenote-extract-data.md) für Visitenkarten und Onlinerezept- und Produktlisten.

Microsoft Graph hat in einigen Formaten strenge Anforderungen, z. B. CRLF-Zeilenumbrüche in einem mehrteiligen Nachrichtentext. Um das Risiko fehlerhafter Nutzlasten zu reduzieren, sollten Sie eine Bibliothek verwenden, um mehrteilige Nachrichten zu erstellen. 

Wenn Sie eine Statusmeldung 400 für eine fehlerhafte Nutzlast erhalten, überprüfen Sie die Formatierung der Zeilenumbrüche und Leerräume, und achten Sie auf Codierungsprobleme. Versuchen Sie beispielsweise die Verwendung von `charset=utf-8` (Beispiel: `Content-Type: text/html; charset=utf-8`).

Siehe [Anforderungen und Einschränkungen für Eingabe-HTML](#requirements-and-limitations-for-input-html-in-post-pages-requests) und [Größenbeschränkungen für POST-Anforderungen](onenote-images-files.md#size-limitations-for-post-pages-requests).


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-post-pages-requests"></a>Anforderungs- und Antwortinformationen für *POST pages*-Anforderungen

| Anforderungsdaten | Beschreibung |  
|------|------|  
| Protokoll | Alle Anforderungen verwenden das SSL/TLS HTTPS-Protokoll. |  
| Header „Authorization“ | <p>`Bearer {token}`, wobei `{token}` ein gültiges OAuth 2.0-Zugriffstoken für Ihre registrierte App ist.</p><p>Wenn dies fehlt oder ungültig ist, schlägt die Anforderung mit dem Statuscode 401 fehl. Siehe [Authentifizierung und Berechtigungen](permissions-reference.md).</p> |  
| Header „Content-Type“ | <p>`text/html` oder `application/xhtml+xml` für den HTML-Inhalt, unabhängig davon, ob er direkt im Nachrichtentext oder im erforderlichen „Presentation“-Teil einer mehrteiligen Anforderung gesendet wird.</p><p>Mehrteilige Anfragen sind erforderlich, wenn Binärdaten gesendet werden sollen. Sie verwenden den Inhaltstyp `multipart/form-data; boundary=part-boundary`, wobei `{part-boundary}` eine Zeichenfolge ist, die den Beginn und das Ende jedes Datenteils signalisiert.</p> |  
| Header „Accept“ | `application/json` | 

<br/>

| Antwortdaten | Beschreibung |  
|------|------|  
| Erfolgscode | HTTP-Statuscode 201. |  
| Antworttext | Eine OData-Darstellung der neuen Seite im JSON-Format. |  
| Fehler | Wenn die Anforderung nicht erfüllt wird, gibt die API Fehler im **@api.diagnostics**-Objekt im Antworttext zurück. |  
| Header „Location“ | Die URL der Ressource für die neue Seite. |  
| Header „X-CorrelationId“ | Ein globaler Bezeichner (GUID), über den die Anforderung eindeutig identifiziert wird. Sie können diesen Wert zusammen mit dem Wert des Date-Headers verwenden, um zusammen mit dem Microsoft Support Probleme zu behandeln. |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a>Zusammensetzen der Stamm-URL des Microsoft Graph-Diensts

Die Stamm-URL des Microsoft Graph-Diensts verwendet das folgende Format für alle Aufrufe von Microsoft Graph:

`https://graph.microsoft.com/{version}/me/onenote/`  

Das Segment `version` in der URL ist die Version von Microsoft Graph, die verwendet werden soll. Verwenden Sie `v1.0` für stabilen Produktionscode. Verwenden Sie `beta`, um ein Feature zu testen, das sich in der Entwicklung befindet. Features und Funktionen in der Betaversion ändern sich möglicherweise, sodass Sie es nicht in Ihrem Produktionscode verwenden sollten. 

Verwenden Sie `me` für OneNote-Inhalt, auf den der aktuelle Benutzer zugreifen kann (eigene und freigegebene Inhalte). Verwenden Sie `users/{id}` für OneNote-Inhalte, die der (in der URL) angegebene Benutzer für den aktuellen Benutzer freigegeben hat. Verwenden Sie [Microsoft Graph](https://graph.microsoft.com/v1.0/users), um Benutzer-IDs abzurufen. 


<a name="permissions"></a>

## <a name="permissions"></a>Berechtigungen

Zum Erstellen von OneNote-Seiten müssen Sie die entsprechenden Berechtigungen anfordern. Wählen Sie die niedrigste Berechtigungsstufe, die Ihre App zur Erledigung ihrer Aufgaben benötigt.

Wählen Sie zwischen:

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All

Weitere Informationen zu Berechtigungsbereichen und deren Funktionsweise finden Sie in der [Microsoft Graph-Berechtigungsreferenz](permissions-reference.md).




<a name="see-also"></a>

## <a name="see-also"></a>Siehe auch

- [Hinzufügen von Bildern und Dateien](onenote-images-files.md)
- [Erstellen von absolut positionierten Elementen](onenote-abs-pos.md)  
- [Extrahieren von Daten](onenote-extract-data.md)
- [Verwenden von Notiztags](onenote-note-tags.md)
- [Integrieren in OneNote](integrate-with-onenote.md)
- [OneNote-Entwicklerblog](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Fragen zur OneNote-Entwicklung auf Stack Overflow](https://go.microsoft.com/fwlink/?LinkID=390182)
- [OneNote GitHub-Repos](https://go.microsoft.com/fwlink/?LinkID=390178)  


